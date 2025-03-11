[TOC]


## Multimodal

**ConceptAttention: Diffusion Transformers Learn Highly Interpretable Features** [paper](https://arxiv.org/pdf/2502.04320)

* Mannaully add object token at the end of the prompts improves saliency map, especially for diffusion models.

 

## Efficiency and Optimization

**Fast Inference from Transformers via Speculative Decoding [Speclative decoding](https://arxiv.org/pdf/2211.17192) **

* Use a small model to generate a sequence and feed to a large model in a batch to verify.

**Efficient Memory Management for Large Language Model Serving with PagedAttention [vllm](https://arxiv.org/pdf/2309.06180)**

* Optimize the GPU cache as OS, allowing non-continuous storing for generating and prompts.

**REST: Retrieval-Based Speculative Decoding [REST](https://arxiv.org/pdf/2311.08252)**

* Use a dataset to construct a trie for next generation, avoid small model



## Pretraining




## Fine-tuning



## Prompting and In Context Learning



## Instruct Learning



## Scaling Law



## RLHF



## Knowledge Understanding and Manipulation



## Retrieval Augmented Generation



## Reasoning



## Agent



## Robotics, Embodied AI

