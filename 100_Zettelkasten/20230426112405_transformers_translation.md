
---
creation date: 2023-04-26 11:24
last updated: 2023-04-26 11:24
---
# [[20230426112405_transformers_translation]] - Transformers for translation
__Tags__: #natural-language-processing  #translation

---
__Contents__: The training of the model is done as the following:
* Encoder receives inputs (sentence) in some languages. Attention layers use all the words in the sentence.
* Decoder receives the same sentences in the desired languages. Attention layers work sequentially (only used the already seen words).

We can fed the decoder with the all target at once as a speed up trick.

__References__:

