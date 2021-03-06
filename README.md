README
=============
## DNAzip: Fast and Deep Compression for Raw and Compressed Sequencing Data

### Download and Install: 
**Requirements:** <br>
`Python 2.7.*` <br>
`bz2file` <br>


```Bash
## Linux or Macox command line
(sudo) pip install bz2file
git clone git@github.com:adamtongji/DNAzip.git
export $PATH=/your/path/to/DNAzip/
chmod 777 /your/path/to/DNAzip/DNAzip
```
### Main arguments:
usage: DNAzip <-f file> <-d> [-o output prefix] [options] <br>

Example: <br>
`DNAzip -f ./example/ecoli.fasta -t fasta -o ecoli_fasta `<br>
`DNAzip -f ./example/sample.fastq -t fastq -o sample_fastq `<br>

### optional arguments: 
|  Parameter   |  Introduction |
| :---------- | :-------- |
|  -h, --help    |        show this help message and exit 
|  -v, --verbose  |       increase ouput verbosity.
|  -q, --quiet   |        No output log file.
|  -t FILE_TYPE, --type FILE_TYPE |  fasta or fastq
|  -f INPUT_FILE, --file INPUT_FILE |   input filename
|  -o OUTPUT_FILE, --output OUTPUT_FILE |  Output filename prefix(Default:noname)
|  -d, --decode   |       extract from the compressed file
|  -w OUT_WIDTH, --width OUT_WIDTH |  Define width of outputfile. Default:0(no limits)
|  -l LEVEL, --level LEVEL |  Compression level. Default:6
|  --version     |        show program's version number and exit
