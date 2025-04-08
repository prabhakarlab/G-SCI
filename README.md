# G-SCI
Last edit 20250408 TA<br>
The G-SCI Test is a statistical test to detect chromatin QTLs (SNPs that are correlated with chromatin state variation in a population). The test can be applied to any collection of sequencing-based chromatin profiles. For example, it can be applied to ChIP-seq, ATAC-seq, DNase-seq and FAIRE-seq data. To enhance statistical power, the G-SCI test includes both peak height variation and allelic imbalance in the likelihood function. Thanks to this feature, it is possible to detect >1,000 regulatory QTLs even when the cohort is relatively small (30-40 individuals). Another advantage of the approach is that there is no need to provide genotypes for the individuals in the cohort. This is because the G-SCI test extracts genotype information from the chromatin sequencing reads supplied as input to the program.

Download the G-SCI test (<u>GSCI_Test.tar.gz</u>). The software tool we provide assumes that users have already processed the ChIP-seq data (peak calling, peak height normalization and SNP calling). See the README included in the tar file for more details.

Download data for the 516,034 SNPs tested in the paper (<u>gsci_data.txt.gz</u>, 922 MB file). This file is in the input format for the G-SCI test. To reproduce the published results, raw QTL-P-values can be calculated using the command: "gsci_raw gsci_data.txt 0.149188". the value of 0.149188 is from Equation (7) in the <a href='https://doi.org/10.1038/nmeth.3326'>paper</a>.

Download the coordinates (hg19) of the 516,034 SNPs tested in the paper (<u>snp_coords.bed</u>). The first three columns are the 0-based coordinates of the SNP, while columns 4 to 6 are the 0-based coordinates of the H3K27ac ChIP-seq peak containing the SNP.

Download the normalized H3K27ac ChIP-seq peak heights for each of the 57 lymphoblastoid cell lines from the Yoruba panel (<u>peaks_normalized.txt.gz</u>). This is a tab-delimited file, with samples in columns and peaks in rows. The peak coordinates are in hg19, 0-based.

Contact: Ricardo del Rosario (rcdelros@gmail.com or delrosariorc@gis.a-star.edu.sg).

Citation: "Sensitive detection of chromatin-altering polymorphisms reveals autoimmune disease mechanisms", R.C.H. del Rosario*, J. Poschmann*, S.L. Rouam, E. Png, C.C. Khor, M. Hibberd, S. Prabhakar, Nature Methods, doi:10.1038/NMETH.3326.
