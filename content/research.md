+++
draft = false
title = 'Research'
+++

### Learning to Walk Like Humans Do: A Developmental Approach to Locomotion in Deep RL
*Senior Thesis at Princeton University, Spring 2026*  
*2026 George A. Miller Prize in Cognitive Science and the Sigma Xi Book Award
[PDF](/seniorthesis.pdf) | [Code](https://github.com/natalia-espinosadice/learning-to-walk-rl)

Humans learn to stand and walk within a matter of months, exploiting a reliable sequence of postural milestones that partitions the full motor configuration space into a series of stable, tractable subproblems. In contrast, humanoid agents trained with standard reinforcement learning (RL) enjoy no such structure, confronting the full complexity of locomotion at once and facing an enormous exploration burden in high-dimensional continuous control. To address this, we propose a hierarchical reinforcement learning (HRL) framework that leverages the structure of human motor development by training each key postural transition—prone-to-crawl, crawl-to-kneel, kneel-to-lunge, lunge-to-stand and stand-to-walk—as a distinct low-level policy, thus imposing a developmental prior over the skill set. A high-level policy then learns to coordinate these motor skills via the Value Function Spaces (VFS) framework. We first validate our approach in LunarLander and BipedalWalker before applying it to Humanoid, where developmental structure directly informs the skill decomposition. Against flat RL baselines and HRL methods that discover structure from experience, our approach achieves upright posture in over 90% of evaluation episodes and completes the full developmental sequence in over 85%, while all baselines plateau at intermediate configurations. Our findings suggest that developmentally grounded structural priors substantially reduce the exploration burden of complex locomotion learning, enabling reliable postural progression where reward engineering, intrinsic motivation and emergent hierarchies fall short.

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
