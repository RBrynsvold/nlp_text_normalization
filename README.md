# nlp_text_normalization
Compare bag-of-words, binary bag-of-words and TF-IDF.


(Shane, Rachel) What is text normalization?  /   Compare bag-of-words, binary bag-of-words and TF-IDF.

Text normalization is the procress of transforming text into a canonical form it may not have had before.

Could involte:
*  case changing – John → john
*  removing accents – résumé → resume
* stemming/lemmatization (reducing a word to its base form)  running → run,
  <stem>argued, arguing, argue → argu (need not be a word)
<lemma> argued, arguing, argue → argue

stemming – follows a crude algorithm that changes parts of the word based on patterns
mapping:  “ing” - > “”  starting → start, ring→ r

lemmatizing – uses an algorthm based on the language to reduce words to a more basic structure:
starting → start;  am, are, is → be


bag-of-words – counts occurrences of a word in a document

binary bag of words – marks if a word is present or not 

tf-idf – term frequency-inverse document frequency – similar to bag of word, but word frequency is replaced by a weighting that accounts for word frequency and how rare the word is in the dataset


















This will weight different words that appear the same number of times in a document based on how often the words appear in the whole dataset.

Example.  Document 17 contains the words “taco” and “rabbit” 3 times.
There are 1400 documents in the data set and “taco” appears 570 times in the data set and “rabbit” appears 12 times in the data set.
word
Tfword, 17
log(1400 / dfword)
Wword, 17
“taco”
3
0.8986
2.696
“rabbit”
3
4.7593
14.278


The more documents a word appears in, the less useful it is for a signal.

