# GroomingDetection
Advancing Grooming Detection in Chat Logs: Comparing Traditional Machine Learning and Large Language Models with a Focus on Predator Tone

The implementations are based on the PAN12 dataset used for grooming detection. The traditional SVM machine learning is implemented and compared with an implementation of the newly released LLaMA 3.2 1B model by Meta. Additionally, a sentiment analysis with the DistilBERT model is done to test the SVM and LLama models' ability to detect grooming in different sentiments. 

-------------------------------------------------------------

1. Download PAN12 dataset: https://zenodo.org/records/3713280
2. Install dependencies
   
-------------------------------------------------------------

SentimentAnalysis.ipynb and FilterLanguage.ipynp are for preprocessing and should be run first. They output the files dataset.csv, dataset_eng.csv, dataset_w_sentiments_csv, and groomer_conversations.csv that are used for the implementation of the SVM and LLaMA 3.

LinearSVM.ipynb and RbfSVM.ipynb contain implementations of SVMs that train and test on different sentiments.

LLaMA3_Sentiments.ipynb contains implementation of LLaMA 3.2 1B model which is fine-tuned to different sentiments.

LLaMA3_PredatoryAuthorIdentification contains implementation of LLaMA 3.2 1B model that matches the PAN12 competition.
