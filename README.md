# Code for the following:
## **1) Whole-genome sequencing and variant identification**<br/>
   - Alignment of whole-genome sequencing reads<br/>
   - Variant calling<br/>
   - Joint genotyping<br/>
   - Variant annotation and effect prediction<br/>
   - Variant filtering<br/>

Sample fastq files can be downloaded at: https://www.ncbi.nlm.nih.gov/sra<br/>
Mmur3.0 refseq can be downloaded at: https://www.ncbi.nlm.nih.gov/datasets/genome/GCF_000165445.2/

All software versions used are below. Please download from their respective github repos. Installation of each is less than 1-5 minutes.<br/>

Whole-genome sequencing read quality assessment: FastQC (v0.11.9)<br/>
Mmur 3.0 genome assembly (accession GCF_000165445.2)<br/>
Alignment and variant identification: Sentieon DNAseq (202112.01) and Burrow-Wheeler Aligner (0.7.17 r1188)<br/>
Alignment quality assessment: QualiMap (v2.2.1)<br/>
Variant annotation and filtering: SnpEff & SnpSift toolbox (v4.5)

Alignment file generated is in BAM format<br/>
Variant calling file generated is in VCF format<br/>
Approx runtime to complete pipeline for a single fastq file (~30x coverage, 3Gb file) is 2 days

**2\) Linkage analysis and LOD score calculation**


