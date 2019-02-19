## Integrated Genome Browser

As the software data manager for the Integrated Genome Browser/IGB (pronounced 'Ig-Bee'), I am responsible for maintaining IGB's primary quickload repository. Each genome in IGB, and therefore in the repository, requires a minimum two files: a genome assembly reference file (.2bit) and a gene annotations/features file (BED detail/BED14). Oftentimes we create the BED14 file from the refGene.bed file sourced from UCSC Table Browser, an NCBI GenBank accession file, and an Entrez gene info file. 

However, due to the distinct conventions of some research institutions, not all gene model annotations are provided with the same information; information we would typically use to map all the pieces together to curate the BED detail file. Therefore, a novel script is required to convert an atypical annotations file into an IGB-friendly BED detail(BED14) format.

As an example: this Python3 script uses an Ensembl BioMart (.tsv) file and merges it with a UCSC Ensembl (ensGene) BED12 file to generate the BED detail file format, the functional format for visualization in IGB!
