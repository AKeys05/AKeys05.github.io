---
layout: page
title: Evaluating Multimodal LLMs for Child Safety Monitoring
description: Evaluating Qwen2-VL and Video-LLaVA for detecting child-safety risks in video.
importance: 3
category: research
---

**Undergraduate Research • Washington, D.C. • September 2025–Present**

Research conducted through the [HU Institute for Human-Centered AI](https://sites.google.com/view/hcaiathoward/) — [AI for Positive Change Lab](https://ai4pc.howard.edu/home).\
Advisors: [Saurav Aryal](https://ai4pc.howard.edu/profile-page-template/dr-saurav-aryal) and [Gloria Washington](https://sites.google.com/scs.howard.edu/gloriawashingtonphd/home)

<figure>
	<img src="{{ '/assets/img/ml_danger_img.png' | relative_url }}" alt="Placeholder for the child-safety monitoring project image" style="width: 100%; max-height: 360px; object-fit: contain;">
	<figcaption style="text-align: center;">Screen capture of annotated video output from an LLM.</figcaption>
</figure>

## Abstract

Traditional baby monitoring devices serve as a cautionary tool for parents, guardians, and caregivers concerned about the safety and security of their child; however, they require constant and scrutinous supervision. With ever-so-persistent distractions and responsibilities, as well as the inevitable need for rest, humans do not have the luxury of around-the-clock surveillance. This preliminary study introduces the use of large language models (LLMs) to develop an artificial intelligence (AI)-enabled baby monitoring system that identifies when a child is engaging in unsafe behavior requiring adult attention. Forty-five use-case videos of children engaging in either dangerous or age-appropriate activity were fed into two video understanding LLMs: Qwen2-VL and Video-LLaVa. A sliding window approach was employed to simulate live video streaming. Both models were prompted to process the video input and return the first instance of danger detected. The outcomes were compared against human perception to identify maximal detection accuracy. Qwen’s accuracy matched human perception on 31/45 videos by the second and 29/45 videos by the frame, yielding a 67% average accuracy rate. LLaVa’s accuracy matched human perception on 23/45 videos by the second and frame, yielding a 51% accuracy rate. Results demonstrate that the use of AI in child danger detection is highly feasible, and Qwen2-VL presented itself as the superior model for this task. Future work aims to supply the model with context from previous windows, perform fine-tuning, and collect data from additional observers to further refine accuracy and precision in preparation for deployment to a fully operational device.
