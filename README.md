# Seq2SeqChatbotWithAttention

#### Problem Description:

Previously, chatbots have been developed using hand-written rules, making models static. With the recent focus in the area of deep learning and natural language processing (NLP), there have been several advancements in the space. For example, Sequence to Sequence (seq2seq) models use recurrent neural networks to solve complex language problems. The general architecture consists of an encoder and a decoder, each being stacks of LSTM or GRU layers. But, Seq2Seq models lack the ability to work with larger sentences because all information from the input sentence is required to be encoded into a fixed length vector, and is sequentially passed until the output is produced. Therefore, knowledge of the input is slowly lost throughout the prediction process.

#### Solution:

To improve the seq2seq model and make it more robust, during training, an attention mechanism is included to gather context for each input word, allowing the decoder to have more information about each part of the input sentence. To generate the next word in the output, the context from the user input and the generated output so far is used to calculate the output with "attention". 
