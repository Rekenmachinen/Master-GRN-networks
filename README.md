# Master-Gene Regulatory networks STN and GRN2boost
This Github is the code form my master thesis.
1) In the Thesis i'm trying to make a new simpler Gene Regulatory networks methods.
2) benchmarking it aginst GRN2boost[1] without a transcription factor list.
3) Make prediction for essential genes and the Regulation in the system based on the network structure.
4) Get an inside to WNT-signalling network through the networks. 
5) get a feeling for how the diffrent days Regulation hierarchy is from the Graph property Distribution.


The data is from a mice in Vivo day 6.5 to 9.5 single celled Rna seqs data and in vitro expreiment is also pressent from day 3-6 but not used as much in the thesis.
The validation of the methods was done on WNT-signalling pathway study of Humans [2]. 
This is becasue mice wnt-signalling network doesn't have specific pathway studies yet so the Validation should be taken litely.
The human WNT-signalling network is way more complex so some pathways will not be the same and way more pathways exist.
after benchmarking it becomes clear while GRNboost2 is used in the field it is a very fast implimentaition and the accurecy without a TF list is still better than random.
The method i created STN is very slow compaired to GRN2boost and in some networks a bit better we don't preciesly know why some of the day the TP is zeros but there can be two reasons this , One The WNT siggnalling network has simpli not been devolvempt yet a bit naiv, and two The STN method can't capture any of the patterns theis days and make small but wrong prediction of TFs in the system.

# refenceses 
[1] https://doi.org/10.1093/bioinformatics/bty916
[2] https://doi.org/10.1371/journal.pone.0144014
[3]
