# CoQA-using-Bi-directional-Transformers-BERT-
Conversational Question Answering (CoQA) Challenge is a challenge aimed at evaluating the ability of the machines to perceive a passage. 
The project focuses on reading comprehension question answering which aims to better understand a passage and answer a set of interconnected questions that follow.
We adopted a bidirectional transformer model for our project. Our BERT-based Implementation achieved an F1 score of 74.6 on the development dataset.


Steps to reproduce the results: 

1) python BERT_Model.py
main_script.py contains the Bert model and the training part. After the execution
a directory named Bert would be created which will contain the predictions file

2) python evaluate-v1.0.py --data-file data/coqa-dev-v1.0.json --pred-file Bert/predictions.json
After the training is complete and the predictions are made, run the evaluate-v1.0 file 
(downloaded from https://stanfordnlp.github.io/coqa/) with the above arguments to get the results. 


Libraries used and other specifications:

CUDA Version 11.2
transformers
torch version 1.4.0
spacy
tqdm
