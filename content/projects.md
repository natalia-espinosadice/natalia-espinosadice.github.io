+++
draft = false
title = 'Projects'
+++

# 2025 
<hr style="border: 0; border-top: 1px solid #ddd; margin: 2em 0;">

### Hierarchical Developmental RL  
*Senior Thesis at Princeton University*  
[Code (in progress)](https://github.com/natalia-espinosadice/hierarchical-developmental-locomotion) | [Midyear Report coming soon]

Building on the junior thesis detailed below, this work rethinks developmental inspiration through a hierarchical reinforcement learning lens. Instead of training a sequential curriculum directly, individual motor skills (ex: lying-to-sitting, kneeling-to-standing, standing-to-walking) are trained separately with their own policies and value functions. A higher-level controller then selects among these skills by consulting their value functions, enabling online composition and recovery if the agent falls. So far, we've tested our approach in toy environments (Lunarlander, Cartpole swing-up) and are working to extend the method to BipedalWalker and eventually to full Humanoid locomotion. 

### Learning to Walk Like Humans Do
*Spring Junior Thesis at Princeton University*  
[Junior Thesis](/juniorthesis_spring25.pdf) | [Code](https://github.com/natalia-espinosadice/learning-to-walk-rl)

This project explored how principles of human motor development could improve reinforcement learning for humanoid locomotion. Two strategies were investigated in parallel: (i) a curriculum of locomotion subtasks aligned with developmental milestones (ex: crawling before standing) and (ii) progressively expanding neural networks that “grow” in depth or width as task complexity increases. Baseline results highlighted both the promise and the challenges of transferring knowledge across subtasks, and these experiments laid the foundation for the senior thesis project detailed above. 

### Sample-Efficient Synthetic Data Generation via Reinforcement Learning 
*Summer REU Project at Vanderbilt University*  
[Paper/code coming soon]  

Synthetic health data offers a powerful tool for enabling machine learning research while protecting patient privacy and addressing data access barriers. However, existing generative models often struggle in small-sample settings, limiting their utility in domains where data is scarce. This project introduces a reinforcement learning–based framework for synthetic electronic health record (EHR) generation. Using the NIH Bridge2AI AI-READI diabetes dataset as a testbed, we benchmarked our RL model against state-of-the-art EHR generative approaches, including GAN-based and diffusion-based methods. On the AI-READI dataset, the RL model achieved higher downstream utility, closer statistical fidelity and lower privacy risks than competing models. When scaled to the larger MIMIC-IV EHR dataset, the RL framework matched the performance of existing state-of-the-art models, demonstrating both robustness and scalability.


### Reimplementing MR.Q: The Role of Representations 
*Final Project for COS 435 at Princeton University*  
[Project Writeup](/COS435_Final_Paper.pdf) | [Code](https://github.com/natalia-espinosadice/COS-435-RL-MrQ)  

This project investigated the role of representations in MR.Q, a generalist reinforcement learning algorithm. We asked two key questions: (i) Does an explicit planner still matter once you have a strong MR.Q-style representation? and (ii) How small can that representation become before performance deteriorates? We found that a one-step planning update often failed to help and even hurt performance - particularly in sparse-reward, pixel-based Atari tasks - while scaling down representation size proved more forgiving in discrete or lower-dimensional domains than in complex continuous-control settings. 

### Deliberation in RL 
[Coming soon]

## 2024 
<hr style="border: 0; border-top: 1px solid #ddd; margin: 2em 0;">

### Predicting Future Drug Trafficking Hotspots in Colombia 
*Fall Junior Independent Work at Princeton University*  
[Final Report](/iw_fall24.pdf) | [Code](https://github.com/natalia-espinosadice/predicting-drug-trafficking-hotspots)  

This project applied machine learning to forecast drug trafficking activity across Colombia’s departments using United Nations seizure data. Socioeconomic indicators and engineered time-series features were used to train Random Forest, SVM and XGBoost models, with XGBoost achieving the best performance. The analysis revealed key drivers such as crime rates, government operations and urban–rural population patterns, offering an empirical analysis of existing socioeconomic theories.

### Classifying and Understanding Autism from Brain Scans
*Summer Research Project at University of Macedonia-Thessaloniki*  
[Code](https://github.com/natalia-espinosadice/brainscan-autoencoder)  

This project applied stacked autoencoders to structural MRI scans from the Autism Brain Imaging Data Exchange (ABIDE) dataset. The models were trained to compress and reconstruct brain images, and the learned representations were used to classify scans as autistic or normally developing. To probe group differences, the models were cross-tested - trained on one group and evaluated on the other - so that discrepancies in reconstruction quality could highlight structural variations between autistic and non-autistic brains.


### Voice-Based Machine Learning for Diagnosis
*Industry Research at Dasion*  

This project developed machine learning pipelines to diagnose health conditions such as autism and depression from voice recordings. Work focused on creating robust preprocessing strategies to handle noisy, real-world data, along with advanced feature extraction and classification techniques to support accurate diagnosis. 


