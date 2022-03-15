STN algoritme 
step one normalise data.
step two remove genes which has less than 0.005 pearson correlation to gene i and remove gene i rom the list
step three fit a regression tree with no hyperparameter to the gene i
store in gene i in column i in the adjecency matrix go back to step two until all genes are covered.
when you have the full direct adjecentcy matrix put it into networkx DiGraph or similar algoritmes 
remove all nodes with no degree in and out and save as pajek and gexf file.

