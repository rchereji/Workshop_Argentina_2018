To download the raw sequencing reads necessary for this workshop (fastq files from GEO database, accession number SRR3649298), please install `sratoolkit`,
```
brew install sratoolkit
```
then run the following command in the terminal:
```
fastq-dump --accession SRR3649298 --split-files --gzip
```
