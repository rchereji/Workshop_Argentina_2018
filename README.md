# Workshop - Argentina 2018
To code along with me, please download this repo and install Anaconda (https://www.anaconda.com/download/) and R (https://cloud.r-project.org/).

After installing Anaconda and R, you will need to install a few extra packages. Please follow the following steps:
 
1. Install Bash kernel for Jupyter notebooks. Open a terminal and run:
```
pip install bash_kernel
python -m bash_kernel.install
```
 
2. Install R kernel for Jupiter notebooks. Open R in the terminal (type: R <return>) and run:
```r
install.packages('devtools')
devtools::install_github('IRkernel/IRkernel')
IRkernel::installspec(name = 'ir35', displayname = 'R 3.5')
```
Note: These commands should be run in the terminal, nor in the R GUI or RStudio.
 
3. Install a few extra command line tools (samtools, bowtie2, etc.). Run the following commands in the terminal:
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew install sratoolkit
brew install samtools
brew install bowtie2
brew install wget
brew install tree
```
