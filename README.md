# 1-Mutect2_PON

Terra workflow: Somatic-SNVs-Indels-GATK4

Version: 4.1.6.0

Source: github.com/broadinstitute/gatk/mutect2_pon:4.1.6.0

## Description

Create a Mutect2 panel of normals

### Description of inputs

intervals: genomic intervals

ref_fasta, ref_fai, ref_dict: reference genome, index, and dictionary

normal_bams: arrays of normal bams

scatter_count: number of parallel jobs when scattering over intervals

pon_name: the resulting panel of normals is {pon_name}.vcf

m2_extra_args: additional command line parameters for Mutect2.  This should not involve --max-mnp-distance, which the wdl hard-codes to 0 because GenpmicsDBImport can't handle MNPs
