Language Representation

This respository contains the code base for the Programming assignment given by Precog. I have attempted the Language Representation Task which covers constructing co-occurence matrix from a chosen dataset, converting them into dense embeddings and evaluating them against neural embeddings, cross-lingual alignment, and analysing harmful associations in static and contextual embeddings. 

Tasks Completeted
    Part 1 - Dense Representations
        Constructed co-occurence matrix - determined the most appropriate window size
        Dimensionality reduction - computed the most suitable dimension in reduced space
        Evaluate the quality of embeddings - Evaluated embeddings across 3 tasks/methods: Word similarity, Analogy reasoning, Clustering and Visualization
        Neural Embeddings - Evaluated Glove embeddings using same methodology as before and compared the results with that of co-occurrence based embeddings
    Part 2 - Cross-Lingual Alignment 
        Used pre-trained fasttext embeddings for both Hindi and English.
        Used Procrustes alignment to learn transformation for projecting Hindi embeddings and English embedding space
        Evaluated the alignment quantitatively using MUSE dataset. Also used a self-generated dataset for this evaluation
    Part 3 - Harmful Associations (Bonus)
        Analysed harmful associations in both static and contextual embeddings. 
        Used Glove 300 dimensional embeddings for static analysis. Quantitative analysis was done using the WEAT test. 
        Used Bert-base-uncased for contextual analysis and qualified my analysis using Causal Language Modeling. Generated sentence likelihood scores for different sentence to assess the stereotype present in contextual embeddings

Directory Structure
- Part 1, Part 2 and Part 3 folder contain the code for their parts respectively. Each ipynb file in the folder has been naamed descriptively to identify the portion it contains. 
- Rest of the folders contain data for different tasks
- Some folders such as models, embeddings and others which are large in size have not been uploaded due to Github restrictions. These have been mentioned in .gitignore file
- requirements.txt contains the packages and their versions installed in the environment used for this assignment. 

To generate the results:
- install all the packages as per requirements.txt
- run all the cell of the ipynb file for which you want to generate results
- NOTE - some files may have dependencies on files that have not been pushed. This was due to size limitations on pushing big files. 

My approach has been listed in the Report placed in root directory. 

Paper reading folder contains the PPT along with the video for the PPT 
