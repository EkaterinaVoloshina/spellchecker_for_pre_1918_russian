## The spellchecker for pre-1918 Russian on the data of the journal "Otechestvennye zapiski"

The model is based on [the spellchecker for Google Ngram](https://github.com/kak-to-tak/Google_rusngram_spellcheck).

### Description

This spellchecker contains three parts: the vocabulary, LSTM-model, the rules. First, the model checks with Levenshtein distance if the word is in the vocabulary, and if it is not in the vocabulary, it uses LSTM-model to predict the right sequence of chars. 

LSTM-model shows the accuracy **0.973** for the words that are included in the vocabulary and **0.508** for the words that cannot be found in the vocabulary. The 

### Usage

```python
git clone https://github.com/EkaterinaVoloshina/spellchecker_for_pre_1918_russian
```
