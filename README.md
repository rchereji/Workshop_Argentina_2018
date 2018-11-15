# Workshop - Argentina, November 2018
To code along with me, you will need to install a few required bioinformatics packages on your computer. Unfortunately, these packages cannot run directly in Windows, so it is recommended to use a Mac or a linux computer.

If you are using a Mac or a linux computer, please download this repo and install Anaconda (https://www.anaconda.com/download/) and R (https://cloud.r-project.org/).

After installing Anaconda and R, you will need to install a few extra packages. Please follow these steps:

1. Install a Bash kernel for Jupyter notebooks. Open a terminal and run:
```
pip install bash_kernel
python -m bash_kernel.install
```
 
2. Install an R kernel for Jupiter notebooks. Open R in the terminal (type R and hit return) and run:
```r
install.packages('devtools')
devtools::install_github('IRkernel/IRkernel')
IRkernel::installspec(name = 'ir35', displayname = 'R 3.5')
```
Note: These commands should be run in the terminal, not in the R GUI or RStudio - in which case you may get an error message.
 
3. Install a few extra command line tools (samtools, bowtie2, etc.). Run the following commands in the terminal:
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew install sratoolkit
brew install samtools
brew install bowtie2
brew install wget
brew install tree
```

If you are using a PC, the easiest way to use the bioinformatics tools described in this workshop is to install a linux virtual machine.  
You can install VirtualBox from https://www.virtualbox.org/ and then download and install the latest version of Ubuntu from https://www.ubuntu.com/download/desktop  
After installing Ubuntu inside a virtual machine, please install all other software as described above.

Once you installed all the packages as described above, you can launch the Jupyter app by typing `jupyter notebook` in the terminal (see detailed instructions here: https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/execute.html). Inside the Jupyter app, navigate to the folder where you have downloaded a copy of this GitHub repo, and launch the provided Jupyter notebooks.
