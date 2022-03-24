Read a recently published proteomic paper (Mapping the proteo-genomic convergence of human diseases (science.abj1541.pdf)) and complete the following tasks/questions.

(Tips: ask google if you are not sure of R coding, terminologies. If you are not sure of the answer to some questions, write down your best guess and approaches you’ve taken try to get the answer to this question)

-1. Look into the supplementary tables (science.abj1541_tables_s1_to_s9.xlsx) to find for a protein called SP-D, how many independent cis-pQTLs and trans-pQTLs it has. What’s the difference between a cis-pQTL and a trans-pQTL?

-2. Load a partial GWAS summary statistics for a protein from the above paper (res_invn_X10361_25_Fenland_MA_auto_chrX_filtered_1pc.0.1MAF.0.05p.short.txt.gz) into your R studio, and answer the following questions.
How many SNPs are in this file?
How many genome-wide significant SNPs (p value < 5 x 10-8) are in this file?
Plot a manhattan plot to visualize genome-wide significant loci. (tips, use r package “qqman”: https://r-graph-gallery.com/101_Manhattan_plot.html) How many genome-wide significant loci are in this file? For each of the genome-wide significant loci, what is the most significant SNP?

-3. Now that you have identified N? genome-wide significant loci for this protein GWAS. We know that this protein is called OAS1. How many of these genome-wide significant loci are in cis (SNPs in these loci are called “cis-pQTL”), and how many of these loci are in trans? Which of those most significant SNPs (from question 2) is the cis-pQTL?
(tips: refer the cis/trans definitions in the paper, and you can use UCSC genome browser https://genome.ucsc.edu/cgi-bin/hgGateway, to check where your genome-wide significant SNPs for these loci located).

-4. Take the cis-pQTL for OAS1 from question 3. Now we want to know if this cis-pQTL happens to also associate with some disease outcomes, say, COVID-19. Check this cis-pQTL in an iterative browser of COVID-19 GWAS: https://app.covid19hg.org/, select phenotype A2 (Critically ill COVID-19). What do you find?
(tips: COVID-19 GWAS browser searches by SNP position, however, the position of a SNP is based on the version of human reference genome. For the SNP with the same RS ID, the positions on the hg19 reference and the hg38 reference are not the same. Hg19 and hg38 are the most commonly used reference, and you need to be careful about it when searching in the UCSC genome browser too.
The proteomic paper and GWAS uses the hg19 reference, and HGI browser uses the hg38 reference.)
