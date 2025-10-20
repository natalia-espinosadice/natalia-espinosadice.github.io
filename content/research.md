+++
draft = false
title = 'Research'
+++


### Hierarchical Developmental RL
*Senior Thesis at Princeton University, Present*  

This work introduces a hierarchical reinforcement learning framework inspired by human developmental trajectories. Individual motor skills are trained separately with their own policies and value functions. A higher-level controller then selects among these skills by consulting their value functions, enabling online composition and recovery if the agent falls. So far, we've tested our approach in toy environments (LunarLander, Cartpole swing-up) and are working to extend the method to full Humanoid locomotion.

### Learning to Walk Like Humans Do
*Junior Thesis at Princeton University, Spring 2025*  
[PDF](/juniorthesis_spring25.pdf) | [Code](https://github.com/natalia-espinosadice/learning-to-walk-rl)

This project explored how principles of human motor development could improve reinforcement learning for humanoid locomotion. 
Two strategies were investigated in parallel: (i) a curriculum of locomotion subtasks aligned with developmental milestones 
(ex: crawling before standing) and (ii) progressively expanding neural networks that “grow” in depth or width as task complexity increases. Baseline results highlighted both the promise and the challenges of transferring knowledge across subtasks. These experiments laid the groundwork for the senior thesis work detailed above.

### Reimplementing MR.Q: The Role of Representations 
*Final Project for COS 435 at Princeton University, Spring 2025*  
[PDF](/COS435_Final_Report.pdf) | [Code](https://github.com/natalia-espinosadice/COS-435-RL-MrQ)  

This project investigated the role of representations in MR.Q, a generalist reinforcement learning algorithm. We asked two key questions: (i) Does an explicit planner still matter once you have a strong MR.Q-style representation? and (ii) How small can that representation become before performance deteriorates? We found that a one-step planning update often failed to help and even hurt performance - particularly in sparse-reward, pixel-based Atari tasks - while scaling down representation size proved more forgiving in discrete or lower-dimensional domains than in complex continuous-control settings. 


### Predicting Future Drug Trafficking Hotspots in Colombia 
*Junior Independent Work at Princeton University, Fall 2024*  
[PDF](/iw_fall24.pdf) | [Code](https://github.com/natalia-espinosadice/predicting-drug-trafficking-hotspots)  

This project applied machine learning to forecast drug trafficking activity across Colombia’s departments using United Nations seizure data. Socioeconomic indicators and engineered time-series features were used to train Random Forest, SVM and XGBoost models, with XGBoost achieving the best performance. The analysis revealed key drivers such as crime rates, government operations and urban–rural population patterns, offering an empirical analysis of existing socioeconomic theories.

### Classifying and Understanding Autism from Brain Scans
*Research at University of Macedonia-Thessaloniki, Summer 2024*  
[Code](https://github.com/natalia-espinosadice/brainscan-autoencoder)  

This project applied stacked autoencoders to structural MRI scans from the Autism Brain Imaging Data Exchange (ABIDE) dataset. The models were trained to compress and reconstruct brain images, and the learned representations were used to classify scans as autistic or normally developing. To probe group differences, the models were cross-tested - trained on one group and evaluated on the other - so that discrepancies in reconstruction quality could highlight structural variations between autistic and non-autistic brains.


### Voice-Based Machine Learning for Diagnosis
*Industry Research at Dasion, 2023-2024*  

This project developed machine learning pipelines to diagnose health conditions from voice recordings. Work focused on creating robust preprocessing strategies to handle noisy, real-world data, along with advanced feature extraction and classification techniques to support accurate diagnosis. 

<style>
/* GLOBAL override, no theme selectors needed */
h3 { margin-bottom: 0.15em !important; }
h3 + p { margin-top: 0.25em !important; }
</style>
