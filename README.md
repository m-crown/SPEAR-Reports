![SPEAR Reports Logo](images/SPEAR_REPORTS.svg)

# SPEAR Reports
SPEAR Reports is a repository of reports produced from the Systematic ProtEin AnnotatoR (SPEAR) tool for lineages and genomes of interest. It also contains a log of the current lineages supplied in SPEAR as a baseline file. This repo is also viewable as a GitHub pages site [here](https://m-crown.github.io/SPEAR-Reports).

## Demo Report
An example SPEAR report for the demo data distributed within SPEAR (currently lineages Alpha, Delta, Omicron, BA.1, BA.1.1 and BA.2) can be found [here](https://m-crown.github.io/SPEAR-Reports/spear_reports/example_vcfs/report.html). 
  
## SPEAR Report Format

SPEAR Reports are composed of four components: a summary of the nucleotide and amino acid mutations found across all samples in the input set; a heatmap displaying residue scores where mutations exist; a table summarising these scores for each sample; and, optionally, an interactive product plot displaying mutated residues and residue scores for each sample. 

### Mutation summaries

The nucleotide changes summary table lists all mutations (point mutations, insertions and deletions), including those in intergenic regions and synonymous mutations, found across all samples, and lists observation count and the percentage of samples each mutation is seen in. 

The amino acid changes table lists all missense, insertion and deletion events, again with counts and percentage of samples these mutations are observed in. 

![https://raw.githubusercontent.com/m-crown/SPEAR-Reports/main/images/mutation_tables.png|mutation tables image](images/mutation_tables.png)

These tables may be useful when discussing new lineages and variants, as they can provide a quick overview of the mutations shared amongst samples in both nucleotide and amino acid space. 

### Heatmaps

The mutated residue heatmaps contain scores as discussed in the main [SPEAR repo](https://github.com/m-crown/SPEAR#scores). These can be used to identify residues contributing to likely immune escape and altered ACE2 binding. The dropdown menu allows for selection of different scoring metrics. The heatmaps are also fully interactive, allowing for zoom onto specific samples/residues and showing residue scores on hover. 

![https://raw.githubusercontent.com/m-crown/SPEAR-Reports/main/images/heatmap.png|SPEAR scores heatmap](images/heatmap.png)

An additional heatmap is linked within the report showcasing mutations across all residues -  this will allow easier comparison between reports. 

### Sample Score Summaries

Table containing summary score values per sample, with highlighted cells where scores exceed that of the selected baseline. The baseline will always be the top row of the table. For an extended discussion of the SPEAR summary scores see [SPEAR Table 4](https://github.com/m-crown/SPEAR/blob/main/docs/Table4.md). The dropdown allows for re-sorting of samples by the available score metrics, in descending order. 

![https://raw.githubusercontent.com/m-crown/SPEAR-Reports/main/images/scores_table.png|SPEAR scores summary table](images/scores_table.png)

### Product Plots

Product plots are produced for all samples passing QC. These plots are available from the main report under the collapsed Product Plots link.    

![https://raw.githubusercontent.com/m-crown/SPEAR-Reports/main/images/product_plots_table.png|SPEAR mutation product plot](images/product_plots_table.png)

These plots show the sample mutations in their relative product/ORF positions. Each mutation is represented by a point, coloured depending on the selected score from the dropdown links in the top left. Subsets of products can be viewed by selecting from the dropdown, allowing for closer inspection in mutation dense regions (e.g. Spike).

![https://raw.githubusercontent.com/m-crown/SPEAR-Reports/main/images/product_plots.png|SPEAR mutation product plot](images/product_plots.png)

## SPEAR Baseline 

Lineages currently in SPEAR baseline set:  

| Lineage   | Date Added | Issue |
| --------- | ---------- | ----- |
| Alpha | 2022-02-06 | [#1](https://github.com/m-crown/SPEAR-Reports-test/issues/1) |
| Delta | 2022-02-06 | [#1](https://github.com/m-crown/SPEAR-Reports-test/issues/1) |
| Omicron | 2022-02-06 | [#1](https://github.com/m-crown/SPEAR-Reports-test/issues/1) |
| BA.1 | 2022-02-06 | [#1](https://github.com/m-crown/SPEAR-Reports-test/issues/1) |
| BA.1.1 | 2022-02-06 | [#1](https://github.com/m-crown/SPEAR-Reports-test/issues/1) |
| BA.2 | 2022-02-06 | [#1](https://github.com/m-crown/SPEAR-Reports-test/issues/1) | 
