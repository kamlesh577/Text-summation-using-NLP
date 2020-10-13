# Text-summation-using-NLP
This repository uses NLP to summarize article.


Text summarization alludes to the procedure of shortening long bits of text. The expectation is to make a reasonable and familiar text having just the central matters plot in the record. 


![DoJVXM9V4AAFj1s](https://user-images.githubusercontent.com/38343027/92320529-b942f380-f03f-11ea-99bf-325dd681ab88.jpg)




Automatic text summarization is a common problem in machine learning and natural language processing (NLP).


 # Need for text summarization?
 
Impelled by the advanced mechanical developments, information is to this century what oil was to the past one. Today, our reality is dropped by the social event and scattering of huge information. 

Truth be told, the International Data Corporation (IDC) ventures that the aggregate sum of computerized information flowing every year around the globe would grow from 4.4 zettabytes in 2013 to hit 180 zettabytes in 2025. That is a great deal of data! 

With such a major measure of information circling in the computerized space, there is a need to have AI algorithm that can naturally abbreviate longer messages and convey exact meaning that can easily  summaries that can fluently pass the intended messages. 

Besides, applying text summarization reduces reading time, accelerates the process of researching for information, and increases the amount of information that can fit in an area.


<img width="735" alt="text-rank" src="https://user-images.githubusercontent.com/38343027/92320769-8f8acc00-f041-11ea-8e37-7cf4b6e64b93.png">


# Main approaches to automatic summarization?


There are two main types of how to summarize text in NLP:

# Extraction-based summarization

The extractive text summarization technique involves pulling keyphrases from the source document and combining them to make a summary. The extraction is made according to the defined metric without making any changes to the texts.
Here is an example:
Source text: Joseph and Mary rode on a donkey to attend the annual event in Jerusalem. In the city, Mary gave birth to a child named Jesus.
Extractive summary: Joseph and Mary attend event Jerusalem. Mary birth Jesus.
As you can see above, the words in bold have been extracted and joined to create a summary — although sometimes the summary can be grammatically strange.

# Abstraction-based summarization
The abstraction technique entails paraphrasing and shortening parts of the source document. When abstraction is applied for text summarization in deep learning problems, it can overcome the grammar inconsistencies of the extractive method.
The abstractive text summarization algorithms create new phrases and sentences that relay the most useful information from the original text — just like humans do.
Therefore, abstraction performs better than extraction. However, the text summarization algorithms required to do abstraction are more difficult to develop; that’s why the use of extraction is still popular.
Here is an example:
Abstractive summary: Joseph and Mary came to Jerusalem where Jesus was born.


# How does a text summarization algorithm work?


Typically, here is how using the extraction-based approach to summarize texts can work:
1. Introduce a method to extract the merited keyphrases from the source document. For example, you can use part-of-speech tagging, words sequences, or other linguistic patterns to identify the keyphrases.

2. Gather text documents with positively-labeled keyphrases. The keyphrases should be compatible to the stipulated extraction technique. To increase accuracy, you can also create negatively-labeled keyphrases.

3. Train a binary machine learning classifier to make the text summarization. Some of the features you can use include:
Length of the keyphrase
Frequency of the keyphrase
The most recurring word in the keyphrase
Number of characters in the keyphrase

4. Finally, in the test phrase, create all the keyphrase words and sentences and carry out classification for them.




# Introduction to Sequence-to-Sequence (Seq2Seq) Modeling

We can build a Seq2Seq model on any problem which involves sequential information. This includes Sentiment classification, Neural Machine Translation, and Named Entity Recognition – some very common applications of sequential information.

There are two major components of a Seq2Seq model:

   1.  Encoder: A stack of several recurrent units (LSTM or GRU cells for better performance) where each accepts a single element of the input sequence, collects information for that element and propagates it forward.
   
   2.  Decoder: A stack of several recurrent units where each predicts an output y_t at a time step t.
Each recurrent unit accepts a hidden state from the previous unit and produces and output as well as its own hidden state.

# Use Cases of the Sequence to Sequence Model

A sequence to sequence model lies behind numerous systems which you face on a daily basis. For instance, seq2seq model powers applications like Google Translate, voice-enabled devices and online chatbots. 


# Limitations of the Encoder – Decoder Architecture
As useful as this encoder-decoder architecture is, there are certain limitations that come with it.

The encoder converts the entire input sequence into a fixed length vector and then the decoder predicts the output sequence. This works only for short sequences since the decoder is looking at the entire input sequence for the prediction
Here comes the problem with long sequences. It is difficult for the encoder to memorize long sequences into a fixed length vecto
