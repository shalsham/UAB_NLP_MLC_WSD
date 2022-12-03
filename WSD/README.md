# WSD Attempt
# The Dataset
National Library of Medicine Word Sense Disambiguation (NLM-WSD)
# Version 1
This version focused on applying an LSTM and a BiLSTM to get an encoding representing CUI. It was trained using a cloze deletion prediction test where the ambiguous word was masked and the model attempted to guess the specific CUI. Despite attempts to adjust the model, it does not appear to learn and overfits the data.

# Version 2
This model focused on using a new method for presenting the data where data was passed to the network in the form $[CLS] w_1, w_2, ..., w_{k-1}, w_k [SEP] CUI [SEP]$ the labels were boolean values indicating if the presented CUI matched the sample document. This method has the benefit of reducing the complexity of the output and allows me to create a larger data set by mixing positive and negative examples. When applying LSTM, a BiLSTM, and a Bert transformer they were not succesful in learning.

# Reflections
I feel that although using the LSTM and BiLSTM are older simpler models their lack of documentation and the age of it made this approach too challenging. I believe I would have been better served starting with a transformer model and dedicating more time to that approach. This would have allowed me to find more up to date documentation and I would have been able to dedicate more time to this approach. 
I suspect that my models were failing in the learning phase as I meticulously inspected the data and the manipulations, but I relied heavily on outside packages I am not comfortable with based on online examples to make the model and the training mechanism. 
I think the labeling approach in Version 2 was better than in version 1 as it massively simplifies the problem to a simple True False problem, but the model failed to learn and had nonesense loss and accuracy.
