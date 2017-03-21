# Human Microbiome Project Commmunity Profiling Datasets

## About the Human Microbiome Project

The [Human Microbiome Project](http://hmpdacc.org/overview/about.php) is a large-scale sequencing project in which "300 healthy individuals were each sampled at 5 major body sites (oral, airways, skin, gut, vagina) and up to three timepoints. Each body site consisted of a number of body subsites, for a total of 15 to 18 samples per individual per timepoint" ([HMP Data Tour Guide](http://hmpdacc.org/resources/tour.php)). Diseased individuals were also sampled in [15 demonstration projects](http://hmpdacc.org/health/projectdemos.php).

The project produced three main types of data: ~1000 reference genomes assembled from many individual samples, whole-genome shotgun (WGS) sequences, and 16S sequence data. 

## HMSCP - Shotgun Community Profiling

This dataset was produced by mapping WGS data to the reference genomes and determining which strains were present and in what amounts for each sample. I think the best thing to work with would be the abundance tables provided - for each sample, this is a file called `samplename_abundance_table.tsv`.

This is the first line of the abundance table for `SRS011061_abundance_table.tsv`. [Depth and breadth of coverage](http://www.danielecook.com/calculate-depth-coverage-bam-file/) and total reference bases are the columns we'd probably use for analysis. 

| Reference Name | Group | Depth | Breadth | Total reference bases |
| -------------- | ----- | ----- | --------| ---------------------|
| Bacteroides cellulosilyticus DSM 14838 | Bacteria | 172.5137357744 | 78.2996901105 | 726268 |

There are options for what data to include: it could be [all data](http://hmpdacc.org/HMSCP/all/), [data from the 300 healthy subjects](http://hmpdacc.org/HMSCP/healthy/), or [just published data](http://hmpdacc.org/HMSCP/) collected prior to June 2011. The disease data isn't presented in the same format, although it would be possible to work with for students who are willing to deal with WGS data directly and do the reference genome mapping themselves.

## HMSMCP - Shotgun MetaPHIAn Community Profiling

[This dataset](http://hmpdacc.org/HMSMCP/all/) is a single table with inferred relative abundances for all samples at once, computed using MetaPHIAn. The table is saved in this folder as `HMP.ab.txt`

## 16S Community Profiling

The 16S region is a short region of DNA that codes for a portion of the ribosome. The 16S region contains several highly variable regions that are often used to assign organisms to Operational Taxonomic Units (OTUs). Two methods of 16S community profiling were used: [Mothur (HMMCP)](http://hmpdacc.org/HMMCP/all/), and [QIIME (HMQCP)](http://hmpdacc.org/HMQCP/all/). As before we can include all data, data from just healthy subjects, or published data. 

## Resources

* [Data browser](http://hmpdacc.org/resources/data_browser.php) with tabs for published data, healthy subject data, demo data (special disease projects), and all data. 

* [Metadata for all samples](http://hmpdacc.org/catalog/grid.php?dataset=metagenomic). [DNA Nexus](http://sra.dnanexus.com/samples/SRS011061) seems to have one extra piece of metadata, namely gender. I'm not sure if this is legit though.

* [HMP dataset documentation](http://hmpdacc.org/resources/dataset_documentation.php) 

* [How to pair 16S and WGS data](http://hmpdacc.org/resources/metagenomics_sequencing_analysis.php)

* We could [request access](https://www.ncbi.nlm.nih.gov/projects/gap/cgi-bin/study.cgi?study_id=phs000228.v3.p1) to additional metadata. This link also has study inclusion/exclusion criteria.





