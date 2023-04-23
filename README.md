# Transformer-Network
Applying Transformer Network for Top 5 simple Tag prediction

we aimed to investigate the efficacy of the Transformer Network in tag prediction tasks.The dataset for this study was obtained from the Kaggle website and consisted of
Stack Overflow data. The dataset contained 6,034,195 rows and 4 columns: Id, Title, Body, and Tags. The Id column served as a unique identifier for each question, while
the Title column contained the question’s title, the Body column contained the body of the question, and the Tags column contained the associated tags. For this study, 
only the last three columns were used, and the Id column was removed. Due to the large size of the dataset, only 40,000 rows were selected for analysis. For the first
part, we employed a dataset filtering mechanism to restrict the dataset to rows containing precisely five top simple tags.
The Transformer Network model implemented in this research consists of an encoder and a decoder layer. The encoder layer was composed of two sub-layers:
a multi-head attention layer with 8 heads, and a fully connected neural network. In each sub-layer of the encoder layer, a residual connection and normalization
were used to improve the performance of the model. The decoder layer was similar to the encoder layer, but with two multi-head attention layers instead of one.
One of the attention layers was masked which is necessary to prevent the model from cheating by looking ahead in the output
sequence.
