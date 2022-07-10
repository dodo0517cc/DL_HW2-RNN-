# DL_HW2 (News classification)

## Objective

Classify the news

## Text preprocessing

1. NLTK tokenizer

NLTK includes many corpus that can help us to tokenize the words well. If we use white space to tokenize the text, we might reach a worse result, cause splitting on white space can also split what should be regarded as a single token or the words that are sometimes written as a single word and sometimes space separated. Furthermore, it cannot replace in English abbreviations and periods with periods.

2. Remove the numbers and punctuations, and also turn the words into lowercase. 

3. Remove the stop words like ‘to’, ‘me’ etc. to leave the more important words in the sentence.

## RNN

1. Choose GLOVE to be my initial embedding.

GLOVE have already counted the number of times a word appears in the document , and counted the probability of two words appearing together to determine their similarity, that is, the vector distance between words, the shorter the distance, the more phase is similar. So if we use pretrained embedding that are pretrained by large corpus, instead of random initialization can reach a better result.

2. Use Bidirectional LSTM instead of RNN

3. Output for 5 categories (sport/entertainment/politics/tech/business)

4. Kaggle Score 0.882 (37/86)

## Transformer

1. BERT

2. Kaggle Score 0.950 (4/77)
