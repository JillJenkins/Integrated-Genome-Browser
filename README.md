# Integrated-Genome-Browser

As the software development data manager for the Integrated Genome Browser ('Ig-Bee'), I am responsible for maintaining the primary Quickload data repository. Each genome in IGB, and therefore in the repository, requires at least two files: a gene assembly reference file (.2bit) and annotations/gene features file (BED detail). 

Due to the distinct conventions of research institutions, not all gene annotations are provided in the same format. Therefore, a novel script is sometimes required to convert an atypical file type/format into an IGB- friendly BED detail(BED14) format.  

As an example: this script will use an Ensembl BioMart (.tsv) file, merge it with an UCSC Ensembl BED12 file to generate a BED14 file format, which is the preferred file format for IGB! 
