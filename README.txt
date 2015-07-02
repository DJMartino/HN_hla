HealthNuts HLA imputation output, version 2, from MCRI Statistical Genetics
===========================================================================

Damjan Vukcevic <damjan.vukcevic@mcri.edu.au>
22 Apr 2015


Overview
--------

These imputation output files are based on the second version of SNP genotype
data provided to MCRI Statistical Genetics by David Martino, by a download link
sent by email on 3 Feb 2015.

The most raw version of the output is in the file `HN2.hla.csv`.  This is then
processed and combined with the original data to give files in PLINK format,
called `HN2.merged.*`.


Brief description of the files
------------------------------

HN2.hla.csv
    The most raw output provided.  Imputed HLA alleles and associated posterior
    probabilities.  All other files are derived from this one and use a calling
    threshold of 0.7 on the posteriors.

HN2.hla.ped
    A PLINK file with just the HLA calls.  Used as part of the post-processing,
    and is probably not too useful on its own.

HN2.hla.txt
    The HLA calls in PLINK covariate format.

HN2.hlaVariants.bed
HN2.hlaVariants.bim
HN2.hlaVariants.bim.b36.backup
HN2.hlaVariants.fam
HN2.hlaVariants.log
    The derived amino acid and SNP types based on the imputed HLA types.
    These are in PLINK format.

HN2.merged.bed
HN2.merged.bim
HN2.merged.fam
HN2.merged.log
    The HLA calls and derived types, merged with (a processed version of) the
    original SNP data provided.  These are in PLINK format.

HN2.merged.dosage.log
HN2.merged.dosage.raw.gz
    `HN2.merged` converted into dosage format.
