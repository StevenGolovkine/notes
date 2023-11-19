
---
creation date: 2023-05-03 10:10
last updated: 2023-05-03 10:10
---
# [[20230503101017_transformers_models]] - Transformers models
__Tags__: #transformers 

---
__Contents__: 

Model gets high-dimensional vectors, created by tokenizers, representing the contextual understanding of that inputs by the Transformers model. This vector usually has three dimensions:
* Batch size: number of sequence processed at the same time. It accepts/expects multiple sentences simulaneously. This is called batching.
* Sequence length: length of the numerical representation of the sequence. It expects same dimensional sentences. This is called padding. We use attention masks, defined as tensors, to ignore parts of the sentence.
* Hidden size: vector dimension of each model input.
From the model, we get hidden states (features). The hidden states are passed to other parts of the model (head). 

Be careful that models are randomly initialized. 
Most of the models can handle $512$ or $1024$ tokens. If we have longer sequences, we have to use larger models or truncate the inputs.

For the Huggingface library:
* Models are described on Huggingface site as card, the pretrained weights are savedd in ``~/.cache/huggingface`.
* The saved models contain two files:
	* `config.json`: attributes to build the model architecture
	* `pytorch_model.bin`: model's weights

__References__:


