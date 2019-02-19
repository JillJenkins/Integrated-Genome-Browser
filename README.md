## Integrated Genome Browser

As the software data manager for the Integrated Genome Browser ('Ig-Bee'), I am responsible for maintaining IGB's primary Quickload repository. Each genome in IGB, and therefore in the repository, requires at least two files: a gene assembly reference file (.2bit) and annotations or gene features file (BED detail/BED14). 

Due to the distinct conventions of research institutions, not all gene annotations are provided in the same format. Therefore, a novel script is sometimes required to convert an atypical file type/format into an IGB- friendly BED detail(BED14) format.  

As an example: this Python3 script takes in an Ensembl BioMart (.tsv) file and merges it with an UCSC Ensembl (ensGene) BED12 file to generate the BED14 file format; which is the preferred format for IGB visualization! 
