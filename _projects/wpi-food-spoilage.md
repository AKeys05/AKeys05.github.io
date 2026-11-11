---
layout: page
title: Machine Learning for Food Spoilage and Shelf-Life Prediction
description: A mechanistic-neural approach to predicting food spoilage and shelf life, with an interpretable chatbot interface.
importance: 4
category: research
---

**Summer Research • Worcester, MA • May–July 2026.**

10-week research project conducted through the [NSF Applied AI for Advanced Applications REU Program](https://www.wpi.edu/academics/departments/data-science/students/reu-program) @ WPI\
Advisors: [Fabricio Murai](https://www.wpi.edu/people/faculty/fmurai)

<figure>
	<img src="{{ '/assets/img/spoilage_img.png' | relative_url }}" alt="Methodology Overview" style="width: 100%; max-height: 360px; object-fit: contain;">
	<figcaption style="text-align: center;">System design overview of the mechanistic-neural model and chatbot interface.</figcaption>
</figure>

## Abstract

Food safety decisions rely on static shelf-life estimates that ignore real-world variation in storage conditions, a gap that matters most in settings such as disaster relief, where both consuming unsafe food and discarding safe food carry increased costs. Existing mechanistic models require per-condition calibration, while deep learning approaches lack biological grounding. We aimed to predict bacterial spoilage from environmental conditions - such as pH, water content, and temperature - and make those predictions usable by non-experts. Using ComBase, a public database of multi-laboratory growth experiments, we built a preprocessing pipeline that standardized curves into a consistent format, yielding a benchmark of spoilage-growth curves spanning a wide range of foods and organisms. We paired a Baranyi growth model driven by cardinal-parameter kinetics with learned networks that correct its initial population, its growth parameters, and its output residual, evaluated under a shared, replicate-grouped, food-stratified five-fold cross-validation. The corrected model substantially improved curve-fit accuracy and reduced the false-alarm rate relative to the mechanistic baseline, with more modest gains in shelf-life timing prediction. To facilitate use by non-experts, we built a conversational interface returning plain-English explanations of these predictions. Correcting a biologically grounded model with learned components therefore improves spoilage prediction without sacrificing interpretability; future work will expand the dataset to additional foods and organisms.
