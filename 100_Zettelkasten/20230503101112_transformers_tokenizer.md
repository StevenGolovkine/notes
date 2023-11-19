
---
creation date: 2023-05-03 10:11
last updated: 2023-05-03 10:11
---
# [[20230503101112_transformers_tokenizer]] - Transformers tokenizer
__Tags__: #transformers #tokenizers

---
__Contents__:
Tokenizer converts text inputs to numbers (encoding) in the exaxt same way the model has been pretrained using three steps:
* Splitting inputs into tokens (words, punctuations, ...)
* Mapping tokens to integer
* Add addtional inputs that may be useful for the model

The encoding can be:
* Word-based (split on spaces/punctuations). We obtain vocabularies of size the total number of independent tolens in the corpus. This could lead to a very large vector, e.g. for a complete language as english, there are $500000$ words. There is no notion of related words (run and running are not identify as similar). And, we need a particular token to represent unknown words.
* Character-based (split into characters). Advantages are that the vocabulary is much smaller (more or less $26$ tokens for english) and out-of vocabulary tokens are rare.
* Subword tokenization. Frequently used words are not split but rarely used words should be split (semantic meaning).

Training a tokenizer is a deterministic statistical process that identify the best subwords to pick for a given corpus.

Some algorithms for tokenizers:
* Byte-Pair Encoding tokenization ([[20230503101112_transformers_tokenizer]])
* WordPiece tokenization ([[20230620091655_wordpiece]])
* Unigram tokenization ([[20230620091722_unigram]])

__References__:


