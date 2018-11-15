To download the raw sequencing reads (fastq files from GEO database, accession number SRR3649298) necessary for this workshop, please install `sratoolkit`,
```
brew install sratoolkit
```
then run the following command in the terminal:
```
fastq-dump --accession SRR3649298 --split-files --gzip
```
