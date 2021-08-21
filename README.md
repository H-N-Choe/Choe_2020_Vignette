# Choe et al (2020) Script Vignette


#### For analyzing differential gene expression in R

You will need [R] and [RStudio], or another R compatible integrated development environment (IDE). 
Samples of the scripts used to analyze differential gene expression in [Choe et al. 2021] have been provided in an .Rmd.
Additional files have been provided in the folder ["Vignette_materials"] to run the .Rmd vignette:
- **Organized** count matrix for [STAR] aligned Male vehicle Area X 
- List of activity dependent genes (ADGs) for all regions
- Prior results for Male E2, Male exemestane, Female vehicle, Female E2, and Female exemestane Area X 
- Ensembl gene lists and biomart objects from [TaeGut 3.2.4] (for reproducibility)

&nbsp;
#### As a resource for independent analysis, we have also included read count matrices for:
  - [STAR] aligned reads
  - [Kallisto] aligned reads
  - Key for Sample-to-library ID 

### These matrices are **COMPLETE** and **RAW** but ***UNORGANIZED!*** &nbsp;&nbsp;&nbsp;Please use the provided key.

&nbsp;
&nbsp;

All RNA-seq reads (available as raw reads on NCBI under SRA accession: [PRJNA698257]) were aligned using assembly [TaeGut 3.2.4]: release 98 (which now obsolete and has been replaced by [bTaeGut1_v1.p]: release 102).

Below are QC results obtained using [MultiQC tools] of the [STAR] aligned reads where each line represents one sample out of 144 total:

&nbsp;
&nbsp;

Read counts: Percentage of read counts that are unique (blue) or duplicated (grey).  
<img src='https://github.com/H-N-Choe/Choe_2020_Vignette/blob/main/images/readcounts.png'>

&nbsp;
&nbsp;

Read assignment: Percentage of reads that were assigned to annotated regions (blue), were un-assigned (grey) or were un-assigned due to ambiguity.  
<img src='https://github.com/H-N-Choe/Choe_2020_Vignette/blob/main/images/readassignment.png'>

&nbsp;
&nbsp;

Loci mapping: Percentage of reads that were uniquely mapped (dark blue), mapped to multiple loci (light blue), mapped to too many loci to be useful (orange), unmapped due to read length (red) or unmapped for other reasons (dark burgundy).  
<img src='https://github.com/H-N-Choe/Choe_2020_Vignette/blob/main/images/locimapping.png'>

&nbsp;
&nbsp;

Phred scores per base: Phred scores across each base position in a read. Green is very good, orange is acceptable, and red is poor.  
<img src='https://github.com/H-N-Choe/Choe_2020_Vignette/blob/main/images/basephred.png'>

&nbsp;
&nbsp;

Phred scores per read: The number of reads with the assigned Phred scores per read. Green is very good, orange is acceptable, and red is poor.  
<img src='https://github.com/H-N-Choe/Choe_2020_Vignette/blob/main/images/readphred.png'>
 
&nbsp;
&nbsp;

"N" content per read: The percentage of N's (ambiguous bases) called at each position.  
<img src='https://github.com/H-N-Choe/Choe_2020_Vignette/blob/main/images/ncontent.png'>
  

&nbsp;
&nbsp;
&nbsp;

If there are any questions, contact [Ha Na Choe, PhD] or [Erich Jarvis, PhD]. 



   ["Vignette_materials"]: <https://github.com/H-N-Choe/Choe_2020_Vignette/tree/main/Vignette_materials>
   [Choe et al. 2021]: <https://doi.org/10.1016/j.yhbeh.2020.104911>
   [TaeGut 3.2.4]: <https://sep2019.archive.ensembl.org/Taeniopygia_guttata/Info/Index>
   [PRJNA698257]: <https://www.ncbi.nlm.nih.gov/bioproject/PRJNA698257/>
   [bTaeGut1_v1.p]: <https://uswest.ensembl.org/Taeniopygia_guttata/Info/Index?db=core>
   [STAR]: <https://github.com/alexdobin/STAR>
   [Kallisto]: <https://pachterlab.github.io/kallisto/about>
   [MultiQC tools]: <https://multiqc.info/>
   [R]: <https://cran.r-project.org/>
   [RStudio]: <https://rstudio.com/>
   [Ha Na Choe, PhD]: <mailto:ha.choe@alumni.duke.edu>
   [Erich Jarvis, PhD]: <mailto:ejarvis@rockefeller.edu>
