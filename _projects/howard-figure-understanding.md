---
layout: page
title: Scientific Figure Understanding with DeepSeek-OCR 2
description: Fine-tuning DeepSeek-OCR 2 for scientific figure classification, extraction, summarization, and visual question answering.
importance: 6
category: research
---

**Undergraduate Research • Washington, D.C. • September 2025–April 2026**

Participation in the [Sci-ImageMiner Competition @ ICDAR 2026](https://sites.google.com/view/sci-imageminer/home?authuser=0).\
Research conducted through the [HU Institute for Human-Centered AI](https://sites.google.com/view/hcaiathoward/) — [AI for Positive Change Lab](https://ai4pc.howard.edu/home).\
Advisors: [Saurav Aryal](https://ai4pc.howard.edu/profile-page-template/dr-saurav-aryal) and [Gloria Washington](https://sites.google.com/scs.howard.edu/gloriawashingtonphd/home)

<figure>
	<img src="{{ '/assets/img/figure_taxonomy.png' | relative_url }}" alt="Scientific figure understanding taxonomy" style="width: 100%; max-height: 360px; object-fit: contain;">
	<figcaption style="text-align: center;">Scientific figure understanding taxonomy.</figcaption>
</figure>

## Abstract

Scientific figure understanding in highly specialized domains remains a critical challenge for general-purpose vision-language models (VLMs). This paper describes a system developed for the Sci-ImageMiner competition at ICDAR 2026, which defines a benchmark for evaluating multimodal reasoning of figures in Atomic Layer and Deposition (ALD/E) research. The four major tasks that complete evaluation are classification, data table extraction, summarization, and visual question answering (VQA). The presented system applies supervised fine-tuning (SFT) with low-rank adaptation (LoRA) to the DeepSeek-OCR 2 3.4-billion parameter model. Across 2,433 sub-figures derived from 126 ALD/E research papers, multi-task training is performed. The resulting fine-tuned model achieves 53.4\% accuracy on classification tasks, an F1 BERTScore of 0.794 on summarization, and 70.8\% accuracy on Yes/No VQA. Analysis of model limitations is presented, with discussion of the challenges of precise data extraction, overfitting, and inter-class confusion among visually similar figure types.
