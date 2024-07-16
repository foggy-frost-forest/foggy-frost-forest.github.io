---
title: "In-Context Learning State Vector with Inner and Momentum Optimization"
collection: publications
permalink: /publication/2024-04-StateVecto
excerpt: '这篇工作是我们在大模型的能力激发上的首次探索。之前的研究发现上下文学习（ICL）得到的任务函数能够存储于模型的分隔词的表示中，能够在推理时无需样例的情况下直接激发模型完成任务。本篇工作通过推导发现，上下文向量和利用上下文样例进行梯度下降得到的模型参数在数学形式上非常相似。受此启发，我们参考模型平均和梯度优化器的思路，提出了上下文向量的内部优化和动量优化，在几乎不影响速度的前提下极大地提升上下文向量的效果。除此之外，本篇工作提出了基于分治算法的上下文向量聚合方法，能够将大量不同样例的上下文向量聚合为一个上下文向量，突破ICL中模型长度导致的上下文样例数的限制。'
date: 2024-04-17
venue: 'Arxiv'
paperurl: 'https://arxiv.org/pdf/2404.11225'
codeurl: 'https://github.com/HITsz-TMG/ICL-State-Vector'
---

**Abstract**

Large Language Models (LLMs) have exhibited an impressive ability to perform In-Context Learning (ICL) from only a few examples. Recent works have indicated that the functions learned by ICL can be represented through compressed vectors derived from the transformer. However, the working mechanisms and optimization of these vectors are yet to be thoroughly explored. In this paper, we address this gap by presenting a comprehensive analysis of these compressed vectors, drawing parallels to the parameters trained with gradient descent, and introducing the concept of state vector. Inspired by the works on model soup and momentum-based gradient descent, we propose inner and momentum optimization methods that are applied to refine the state vector progressively as test-time adaptation. Moreover, we simulate state vector aggregation in the multiple example setting, where demonstrations comprising numerous examples are usually too lengthy for regular ICL, and further propose a divide-and-conquer aggregation method to address this challenge. We conduct extensive experiments using Llama-2 and GPT-J in both zero-shot setting and few-shot setting. The experimental results show that our optimization method effectively enhances the state vector and achieves the state-of-the-art performance on diverse tasks.
