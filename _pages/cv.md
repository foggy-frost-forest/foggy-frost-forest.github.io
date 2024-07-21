---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
- M.S. in Harbin Institute of Technology, Shenzhen, 2023.09-now
  - Advisor: Pro. Hutian Bao
- B.S. in Harbin Institute of Technology, Shenzhen, 2019.09-2023.05

Research Experience
======

**Few-Shot Event Extraction**
2022.01-2022.08
- Constructed a deep learning model to extract events and their triggers from target texts with a limited number and variety of reference events. Compared to popular event extraction models, the few-shot event extraction model can quickly adapt to new events continuously emerging in real life.

**Event Causality Identification**
2022.06-2022.12
- Designed a progressive reasoning strategy, enabling the model to infer intra-sentence and inter-sentence event causality from easy to difficult, enhancing the model's causality identification performance.
- Constructed an event relationship graph and an event pair attention graph neural network to adapt the model to the structural characteristics of causal reasoning, thereby improving the model's causal reasoning ability.

**In-Context Learning**
2023.09-2024.01
- Explained the working mechanism of state vectors in contextual learning through the mathematical theory of gradient descent, proposing an optimization algorithm for state vectors. The model completes tasks by reading the task function stored in the state vector without any examples, greatly improving the efficiency of contextual learning.
- Designed a state vector aggregation algorithm based on the divide-and-conquer method, overcoming the limitation on the number of contextual learning examples caused by input length constraints.

**In-Context Alignment**
2024.04-2024.07
- Designed a segmented contextual learning generation framework, using few-shot generation strategies only for the generation of a few prefix words, significantly improving generation speed.
- Developed a contextual vector-assisted generation strategy, using state vectors of aligned contextual examples to directly trigger the model to align with human intentions, eliminating the need for fine-tuning.

Project
======

**Pre-training and Instruction Fine-tuning of Lechee Large Language Model**
2023.03-2024.01
- Deeply involved in the architecture design and pre-training algorithm development for the LiZhi large model. Completed the pre-training of 7B, 11B, and 35B large language models from scratch over more than two months using 2T pre-training corpora and hundreds of CPUs. LiZhi achieved performance on par with or exceeding contemporaneous models of similar scale on multiple Chinese and English datasets.
- Responsible for the instruction fine-tuning of the LiZhi large model, including tasks such as data cleaning, algorithm design, instruction fine-tuning, dialogue system development, and model evaluation.

**Information Accuracy Check and Revision for Large Language Models**
2023.09-now
- This project aims to detect and correct the factual and logical accuracy of large model outputs using multiple sources of evidence, thereby improving the informational accuracy of the model's outputs.
- Responsible for collecting multiple sources of evidence and building a retrieval system using Faiss. Designed a reranking-based evidence fusion algorithm and a chain-of-thought-based error correction algorithm.

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
