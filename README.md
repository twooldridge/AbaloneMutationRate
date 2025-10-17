# AbaloneMutationRate

This repo contains all code associated with:


T. B. Wooldridge, S. M. Ford, H. C. Conwell, J. Hyde, K. Harris, B. Shapiro, **Direct measurement of the mutation rate and its evolutionary consequences in a critically endangered mollusk**. Mol. Biol. Evol. 42, msae266 (2025).

I've uploaded the code in a series of jupyter notebooks that draw on python, R, bash, etc. These notebooks were run of an HPC configured with `slurm`, which is why you'll see a lot of references to `slurm` commands in my code.

**Table of Contents**

1) `Alignment_Varcalling.ipynb` - This notebook contains everything related to processing the sequenced pedigree data, from QC to variant calling with both GATK and bcftools.
2) `Masking.ipynb` - This contains code for generating mappability and sequencing depth-based masks. These are then applied in the estimation stage.
3) `Estimation.ipynb` - Bulk of the analyses for the paper. In this, you'll find code for:<br>
     a) identifying *de novo* mutations<br>
     b) quanitfying sib mutations<br>
     c) calculating FDR & FNR<br>
     d) obtaining mutation spectra (**Fig. 2**)<br>
     e) plotting the result on a phylogeny of mutation rates (**Fig. 1**)<br>
     f) adding life history context<br>
4) `Phasing.ipynb` - Phasing variants using `whatshap` and attempting to determine which parent they came from with `POOHA`
5) 
