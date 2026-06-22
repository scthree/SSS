# Code for the following:<br/>
(please see Methods from Chang et al 2025 for more details)
https://www.biorxiv.org/content/10.1101/2025.05.28.655959v1

## **1) Whole-genome sequencing and variant identification**<br/>
   - Alignment of whole-genome sequencing reads<br/>
   - Variant calling<br/>
   - Joint genotyping<br/>
   - Variant annotation and effect prediction<br/>
   - Variant filtering<br/>

Software versions are listed below. Please download from their respective github repos. Installation of each is less than 1-5 minutes.<br/>

Whole-genome sequencing read quality assessment: FastQC (v0.11.9)<br/>
Mmur 3.0 genome assembly (accession GCF_000165445.2)<br/>
Alignment and variant identification: Sentieon DNAseq (202112.01) and Burrow-Wheeler Aligner (0.7.17 r1188)<br/>
Alignment quality assessment: QualiMap (v2.2.1)<br/>
Variant annotation and filtering: SnpEff & SnpSift toolbox (v4.5)

Sample fastq files can be downloaded at: https://www.ncbi.nlm.nih.gov/sra<br/>
Mmur3.0 refseq can be downloaded at: https://www.ncbi.nlm.nih.gov/datasets/genome/GCF_000165445.2/

Alignment file generated is in BAM format. Variant calling file generated is in VCF format. Runtime to complete pipeline for a single fastq file (~30x coverage, 3Gb file) is ~2 days.<br/>

Scripts are in the [WGS and variant identification](./WGS%20and%20variant%20identification) folder. 

## **2) Linkage analysis and LOD score calculation**<br/>

- VCF to PLINK2 format conversion: PLINK (v2.0)<br/>
dl: https://www.cog-genomics.org/plink/2.0/<br/>

- Parametric linkage analysis and LOD score calcuation: MERLIN (v1.1.2) and LAMP (v0.0.12)<br/>
dl: https://csg.sph.umich.edu/abecasis/merlin/download/<br/>
dl: https://csg.sph.umich.edu/abecasis/LAMP/download/<br/>

Installation time is less than 1-2 minutes. Simulated datasets can be found in the MERLIN dl link above. Output files are in text format. Runtime to complete pipeline (~1,500 variants) is <2-3 minutes.<br/>

Scripts are in the [Linkage analysis and LOD score calculation](./Linkage%20analysis%20and%20LOD%20score%20calculation) folder.
