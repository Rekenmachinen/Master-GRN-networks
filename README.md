# STN vs GRNboost2
# Coding of a GRN method form my master thesis in Biophyscis
The key goals
1) In the Thesis i'm trying to make a new simpler Gene Regulatory network method.
2) benchmarking it against GRN2boost[1][4] without a transcription factor list.
3) Make prediction for essential genes and the Regulation in the system based on the network structure[3][7].
4) Get an inside to WNT-signaling network through the networks[2][6]. 
5) Getting a feeling for how the different days' Regulation hierarchy is from the Graph property Distribution.


The data is from mice in Vivo day 6.5 to 9.5 single celled Rna seq data and in vitro experiment is also present from day 3-6 but not really used as much in the thesis.
The validation of the methods was done on WNT-signaling pathway study of Humans [2]. 
This is because mice wnt-signaling networks studies doesn't have specific pathways yet so the Validation should be taken lightly[6].
The human WNT-signaling network is way more complex so some pathways will not be the same and way more pathways exist[2].
After benchmarking it becomes clear why GRNboost2 is used in the field. It is a very fast implementation and the accuracy without a TF list is still better than random.
The method i created STN is very slow compared to GRN2boost and in some networks a bit better we don't precisely know why some of the day is zeros but we have some two hypothesis One The WNT signaling network has simpli not been developed yet a bit naive, and two The STN method can't capture any of the patterns theis days and make small but wrong prediction of TFs in the system.


# refenceses 
[1]GRN2boost https://doi.org/10.1093/bioinformatics/bty916

[2]WNT signalling Validation https://doi.org/10.1371/journal.pone.0144014

[3]Essntial database 1 http://essentiality.ls.manchester.ac.uk/

[4]code for GRNboost2 https://github.com/aertslab/arboreto

[5]scikit-learn tree https://scikit-learn/stable/modules/tree.html

[6]Nature paper  used correlation matrix https://doi.org/10.1038/s41581-020-00343-w

[7] essntial database 2 https://doi.org/10.1371/journal.pone.0178273
