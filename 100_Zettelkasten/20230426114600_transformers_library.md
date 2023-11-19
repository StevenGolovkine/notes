
---
creation date: 2023-04-26 11:46
last updated: 2023-04-26 11:46
---
# [[20230426114600_transformers_library]] - The Transformers Python library
__Tags__: #transformers #python

---
__Contents__: This library is based on Pytorch ``nn.Module`` and Tensorflow ``tf.keras.Model``. The main function is ``pipeline``. It consists of three blocks: 
* Tokenizer ([[20230503101112_transformers_tokenizer]])
* Model ([[20230503101017_transformers_models]])
* Post-processing.

**Post-processing**: it converts outputs of the model into something readable (probability, word, ...).

**Fine tuning a pretrained model**: 
* Batching the tokenizer (using map function)
* Padding per batch is usually more efficient (dynamic padding)
* Fine tuning can be quite long (even for small dataset)

__References__:

