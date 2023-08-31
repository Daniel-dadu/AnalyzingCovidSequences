# Exploring Global Patterns and Regional Similarities in SARS-CoV-2 Sequences using R

The objective of this analysis of SARS-CoV-2 sequences from the top 20 countries with the highest reported cases, **conducted using R programming**, was to understand the similarities and differences among these sequences. The analysis aimed to uncover patterns in terms of sequence lengths, the presence of certain nucleotides, and the overall relationships among the variants.

From the graphical representation of the data, it becomes evident that the sequences share similar lengths, ranging between 295,000 and 300,000 bases. The bar graph depicting the number of DNA bases in each variant indicates a high degree of similarity among the sequences, which aligns logically with them all belonging to the same virus.

An interesting observation lies in five variants: Germany, Canada, Mexico, South Africa, and the United Kingdom. These sequences contain nucleotides labeled as "N," which represent any base (A, G, C, or T). Since the occurrences of "N" nucleotides are minimal in these cases, they have negligible impact on the graphs, maintaining the overall visual similarity.

To unveil more pronounced differences among these variants, the study suggests analyzing the outcomes of a global hierarchical analysis of the sequences.

Alignment of sequences using the "AlignSeqs()" function from the DECIPHER library led to the creation of a distance matrix. This matrix is interpreted with lighter colors indicating higher similarity between sequences (diagonal), while darker colors signify lower similarity. The generated phylogenetic tree, based on this matrix, provides a clearer representation of close sequences.

A specific focus on similar variants within the same cluster, such as the case of the Spanish sequence "MW769706.1" and the UK sequence "OD906774.1," suggests a certain relationship among European sequences. Similarly, the case of German sequence "MW822592.1" and French sequence "MW580244.1" implies similarity among European variants.

However, the Mexican sequence "MW884219.1" and the Brazilian sequence "MW592707.1," both in the same cluster, indicate strong similarity between regions. The analysis concludes that variants within the same continent tend to be more alike.

Notably, the Iranian sequence "MW737421.1" demonstrates little similarity with sequences from other countries, implying limited interaction.

Lastly, the U.S. sequence "MZ008250.1" is similar to UK and Spanish variants but not as much to the Peruvian sequence "MW938089.1," both of which are in the same continent. This leads to the conclusion that regional similarity doesn't preclude similarity with variants from other continents. Moreover, geopolitical connections between countries influence these patterns, evident in less-similar variants from geopolitically isolated countries.

In summary, the analysis aimed to identify patterns of similarity and difference among SARS-CoV-2 sequences from various countries, highlighting regional trends and global connections.

Video discussing this: https://youtu.be/YiqoTvCiCmc