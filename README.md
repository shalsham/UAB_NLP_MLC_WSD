# UAB_NLP_MLC_WSD


# BioBert Multi-Label Text Classifier for Hallmarks-of-Cancers(HOC) corpus
# The Dataset
The Hallmarks of Cancer  (*HOC) corpus consists of 1852 PubMed publication abstracts manually annotated by experts according to the Hallmarks of Cancer taxonomy. The taxonomy consists of 37 classes in a hierarchy. Zero or more class labels are assigned to each sentence in the corpus.
# The model
The Multi_label classifier was done in a single jupyter notebook for easy execution.
In this notebook we used BioBERT to do document classification. For more information on BioBert please see the followin link https://huggingface.co/dmis-lab/biobert-v1.1
The data files for this project are 'L6.xlsx' & 'L7.xlsx'
The raw dataset can be found at: https://github.com/sb895/Hallmarks-of-Cancer
# Instructions
To run the code download the notebook, the data files. 
All required installations can be found in the first cell of the notebook followed by the necessary imports

# Execution Note
The Batch size was reduced in this notebook as well the number of epochs to make runnable for most users. 
