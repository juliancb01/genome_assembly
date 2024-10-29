# Genome_Assembly
This repository is for my Masters project (2024-June 2025), related to aim 1 of 3: genome assembly. Any scripts related to DNA data, assembly &amp; analysis of related outputs are contained here. Details of files contained in each folder are described below

(1) read_qc
- For four reads types: novaseq, hifi, ont & hic

(2) assembly_pipeline
- General process follows stages:
    - Stage 1: Hifiasm (~low coverage hifi+ont assembly)
    - Stage 2: FCS (removal of bacterial contaminants present)
    - Stage 3: NextPolish (increasing coverage by including short reads)
    - Stage 3b: Hi-C mapping to stage 3 genome
    - Stage 4: YaHs (Hi-C scaffolding)

(3) assembly_analysis
- Scripts used to analyse resulting assemblies
- sub folder: ITS2 analysis, creating graphs in R to represent major BLAST hits for different ITS2 Symbiodiniaceae sequences & their associated taxa to check for contamination in sequences from within Symbiodiniaceae (as opposed to just bacterial)
- 'coverm_analysis.rmd': generation of contig coverage-length plots for stage 3 assemblies (mean coverage calculated for each contig & each sequencing data type using coverm & seqkit used to provide contig lengths)


