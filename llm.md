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

**QLORA: Efficient Finetuning of Quantized LLMs [Q-Lora](https://arxiv.org/pdf/2305.14314)**
* 4-bit NormalFloat Quantization and Double Quantization



## Datasets and Evaluation

**Documenting Large Webtext Corpora: A Case Study on the Colossal Clean Crawled Corpus [C4](https://arxiv.org/pdf/2104.08758)**
* Get website data of s anapshot, and filter some bias tokens

**BLINK : Multimodal Large Language ModelsCan See but Not Perceive [Blink](https://arxiv.org/pdf/2404.12390)**
* Focus on some tasks human can answer with a blink time, rather than normal recognition and caption tasks.

**Judging LLM-as-a-Judge with MT-Bench and Chatbot Arena [paper](https://arxiv.org/pdf/2306.05685)**
* MT-bench(multi-turn question answering), Chatbot Arena(2 answers, which is better)

**Evaluating Large Language Models Trained on Code [Codex](https://arxiv.org/pdf/2107.03374)**
* Supervised fine-tuned python code from github problems, and further fine-tuned on standalong functions



## RLHF
**Training language models to follow instructions with human feedback [RLHF](https://arxiv.org/pdf/2203.02155)**
* reinforcement learning for llm setting

**Direct Preference Optimization: Your Language Model is Secretly a Reward Model [DPO](https://arxiv.org/pdf/2305.18290)**
* Simplify from RLHF, showing the perference can be implicitly written as some kind of rewards. More like a supervised contrastive learning

**RAFT: Reward rAnked FineTuning for Generative Foundation Model Alignment [RAFT](https://arxiv.org/pdf/2304.06767)**
* Some kind of close to DPO, the reward is fixed with perference.



## Knowledge Understanding and Manipulation
**Finding Transformer Circuits with Edge Pruning [paper](https://arxiv.org/pdf/2406.16778)**
* Use edge-pruning method to reduce most of the computation graph

**Does Fine-Tuning LLMs on New Knowledge Encourage Hallucinations [paper](https://arxiv.org/pdf/2405.05904)**
* Train model use large proportion of unknown data may be harmful, but with some maybe known data is helpful.



## Reasoning



## Agent



## Robotics, Embodied AI



## Sampling
**Optimizing Temperature for Language Models with Multi-Sample Inference [paper](https://arxiv.org/pdf/2502.05234)**
* Find that the token level entropy has a spike point of temperature, which is the point the log entropy from concave to convex, meaning quality collapse.


## Attention Sinks
**Efficient Streaming Language Models with Attention Sinks [paper](https://paperswithcode.com/method/attention-sinks)**
* Use initial several tokens (attention sink) and most recent several tokens is good in performance and much faster, can deal with long texts.