
---
creation date: 2023-06-20 09:16
last updated: 2023-06-20 09:16
---
# [[20230620091612_byte_pair_encoding]] - Byte-Pair Encoding tokenization
__Tags__: #tokenizers #algorithm-theory  

---
__Contents__:
The Byte-Pair encoding tokenizer has been developed to compress text and is used as tokenizer in GPT models. It is based on three steps:
1. Compute the unique set of words in the corpus (may be done at the byte level).
2. Build the vocabulary using all the symbols.
3. Learn "merges" that are rules to nerge two elements of the vocabulary into one.

If a word is not in the base vocabulary, it is replaced by \[UNK\] in the tokenized words.


__References__:



