# PhyloProfile Tool

PhyloProfile Tool is a Shiny(R)-based tool for visualizing the phylogenetic profile of a list of genes.
The profile can be plotted with different taxonomy ranks (species, family, phylum, etc.), which would be useful for analyzing the presence absence of sequences in a large amount of taxa.

Currently, the information represented on the profile are the *Feature Architecture Similarity (FAS) scores*, *percentage of species* that have orthologs with the reference sequences and the *traceability scores* (optional). The *percentage of species* is only available when you group initial taxa into higher taxonomy rank (for example, you need to analyse the profile in phylum level, while your input taxa are in species level). These information can be manually filtered from the plot by changing the corresponding cutoff. Besides, *protein domain architectures* can also be visualized if the necessary info are available (positions of domains. See `data/demo/test.traceability` for example).

# Demo data
In `data/demo/` you can find some test data including a main input file:
>test.main

2 other optional files for plotting protein domain architectures & traceability scores:
>test.architecture

>test.traceability

and a gene list for customized profile plot:
>geneList.txt

# Usage
(1) Clone this git repository to your computer using this command:

>git clone https://github.com/trvinh/phyloprofile

OR

Manually download all the files to your computer and keep the original folder structure.

(2) Install dependent R packages:

>Rscript installPackages.R

(3) Run PhyloProfile tool:

>R -e 'shiny::runApp(,launch.browser=TRUE)'

NOTE: R and Rscript has to be installed on your machine.

# Bugs
Any bug reports or comments, suggestions are highly appreciated

# Contact
Vinh Tran
tran@bio.uni-frankfurt.de
