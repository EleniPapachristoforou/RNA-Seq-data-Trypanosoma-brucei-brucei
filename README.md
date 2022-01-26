# RNA-Seq-data-Trypanosoma-brucei-brucei

Task   

Have to look at some RNA-Seq data that have been generated from Trypanosoma brucei brucei. 
The research lab is particularly interested in whether there are any differences in gene expression levels in two different life cycle stages: "slender" and "stumpy". 
There are three biological replicates for each of the two conditions, and the technology used was paired-end sequencing.  

  

The goal for this task is to write a pipeline programme that, when executed in a Unix terminal, will process the data provided in the directory. 

The pipeline should have the following minimum overall design: 

1. perform a quality check on the paired-end raw sequence data (which are in gzip compressed fastq format using the installed programme fastqc 

2. assess the numbers and quality of the raw sequence data based on the output of fastqc 

3. align the read pairs to the Trypanosoma brucei brucei genome using installed programme bowtie2 , convering the output to indexed "bam" format with  samtools ; the Trypanosoma brucei brucei genome sequence need to be also in the directory

4. generate counts coverage data: the number of reads that align to the regions of the genome that code for genes; this is to be done using the installed programme bedtools and the Tbbgenes.bed "bedfile" that contains the informa on about the gene loca ons in the genome; the bedfile is provided in the directory 

5. generate a plain text tab-delimited output that gives the sta s cal mean (average) of the counts per gene for each group, e.g. gene name, mean for slender samples, mean for stumpy samples. 
