# -23B4213_LLM-
NLP - Natural Language Processing 
It uses 
applications: Alexa, Google Home, Translate
Roadmap of NLP 
Cleaining the Input
Step 1: Text Preprocessing - Tokenisation , Lemmatization , Stemming

Converting our Input text to Vectors
Step 2: Text Preprocessing 2 - BOW, TFIDF , Unigram , Bigrams 

Converting Input Text into Vectors
Step 3: Text Preprocessing 3 - Word2Vec , AvgWord2Vec

Nueral N/w (part of Deep learning)
Step 4: RNN , LSTMRNN , GRURNN

Text Preprocessing - Word Embedding
Transformers 
BERT
                
      Tokenisation In NLP  //Terminilogies used in NLP
Topics:

1) Corpus: Paragraph
2) Documents: Sentences
3) Vocabulary: Unique Words
4) Words: All the words persent in the Corpus will define as separately as words  

What is Tokenisation 
The process of Converting Corpus(Paragraph) or Documents(Sentances) into Tokens ![image](https://github.com/chiefcody/-23B4213_LLM-/assets/163542025/edef07a8-7e29-4052-9fe4-0ac0cd437f94)
or Simply converting paragraphs into Tokens(sentances) 
Words can also b a token /sentances can also b a token ![image](https://github.com/chiefcody/-23B4213_LLM-/assets/163542025/7441621c-55e8-4ef6-9f91-9eb827348b0c)

Vocabulary
When we further we count in the unique number of words in a token ![image](https://github.com/chiefcody/-23B4213_LLM-/assets/163542025/8bd24336-8591-41f1-9904-3a117ab5dd1f)
import 
        1)sent_tokenize      (to convert para into sentances)
        2)word_tokenize     (convert para/sentances into words)  //all characters like ,.are treated separately #Adi's is not splitted
        3)wordpunct_tokenize  (same like word_tokenize but this time Adi's ka 's is treated separtely 
        4)TreebankTokenizer (same as word_tokenize but .(fullstop) is not treated as different entity but taken together ex- " Pune. " BUT w.r.t to last word .(fullstop) is separate

        Stemming
        
It's basically breaking down a word to it's root stem               that affixes to preffixes or suffixes to the roots of the words known as Lemma
#IT's a Classification Problem
#find out whether the comments of Product is a positive or negative review (0/1)
#Reviews --> eaten , eat , eating  (going , go , goes)
 Different Types of stemming techniques
 
1) PorterStemmmer
   
    stemming.stem("sitting")      ![image](https://github.com/chiefcody/-23B4213_LLM-/assets/163542025/b690d4fe-1125-49e4-8b1f-abe2b03e7100)

2) Regexp Stemmer Class
   reg_stemmer.stem('fairly')
    It basically takes a single regular expression and removes any suffix or preffix that matches that expression

3) Snowballs Stemmer
    It's better It's snowballsstemmer.stem('fairly')

Drawback ![image](https://github.com/chiefcody/-23B4213_LLM-/assets/163542025/43f42e8e-028f-4906-b81a-663989258606)

          Wordnet Lemmatizer

Lemmatization technique is like stemming. The output we will get after lemmatization is called
'lemma', which is a root word rather than root stem, the output of stemming. After lemmatization, we will be getting a valid word that means the same thing.
