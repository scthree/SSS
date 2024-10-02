## Code for the following: 
1) Alignment of whole-genome sequencing reads
2) Variant calling
3) Joint genotyping
4) Variant annotation and effect prediction
5) Variant filtering

Sample fastq files can be downloaded at: https://www.ncbi.nlm.nih.gov/sra
Mmur3.0 refseq can be downloaded at: https://www.ncbi.nlm.nih.gov/datasets/genome/GCF_000165445.2/

All software versions used are below
Please download from their respective github repos (and follow dl instructions there)
Installation of each is less than 1-5 minutes
Whole-genome sequencing read quality assessment: FastQC (v0.11.9)
Mmur 3.0 genome assembly (accession GCF_000165445.2)
Alignment and variant identification: Sentieon DNAseq (202112.01) and Burrow-Wheeler Aligner (0.7.17 r1188)
Alignment quality assessment: QualiMap(v2.2.1)
Variant annotation and filtering: SnpEff & SnpSift toolbox (v4.5)

Please see Paper Methods for how to run whole-genome sequencing/alignment/variant calling pipepline
Alignment file generated is in BAM format
Variant calling file generated is in VCF format
Approx runtime to complete pipeline for a single fastq file (~30x coverage, 3Gb file) is 2 days
