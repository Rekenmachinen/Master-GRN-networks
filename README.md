# Master_Bio
This Github is the code form my master thesis.
In the Thesis i'm trying to make a new simpler Gene Regulatory networks methods and I'm benchmarking it aginst GRN2boost without a transcription factor list which is a well test method in Bioinfomatic.
The data is from a mice in Vivo day 6.5 to 9.5 single celled Rna seqs data and in vitro expreiment is also pressent from day 3-6 but not used as much in the thesis.
The validation of the methods was done on WNT-signalling pathway study of Humans. This is becasue mice wnt-signalling network doesn't have specific pathway studies yet so the Validation should be taken litely  since the human WNT-signalling network is way more complex so some pathways will not be the same and way more pathways exist.

STN algoritme 
step one normalise data.
step two remove genes which has less than 0.005 pearson correlation to gene i and remove gene i rom the list
step three fit a regression tree with no hyperparameter to the gene i
store in gene i in column i in the adjecency matrix go back to step two until all genes are covered.
when you have the full direct adjecentcy matrix put it into networkx DiGraph or similar algoritmes 
remove all nodes with no degree in and out and save as pajek and gexf file.

