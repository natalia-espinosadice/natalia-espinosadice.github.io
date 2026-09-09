+++
draft = false
title = 'Home'
+++
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/academicons@1.9.4/css/academicons.min.css">

<div class="fullbleed push-right">
  <div class="two-col">
    <aside class="profile-card">
      <img src="/images/IMG_4823.png" alt="Portrait">
      <h3 class="profile-name">Natalia Espinosa Dice</h3>
      <p class="affil">
        Department of Computer Science<br>
        Princeton University
      </p>
      <div class="icon-row">
        <a href="/cvv.pdf" title="CV"><i class="fa-regular fa-file-lines"></i></a>
        <a href="https://github.com/natalia-espinosadice" title="GitHub"><i class="fab fa-github"></i></a>
        <a href="https://www.linkedin.com/in/natalia-espinosa-dice" title="LinkedIn"><i class="fab fa-linkedin"></i></a>
        <a href="mailto:nespinosadice22@gmail.com" title="Email"><i class="fa-solid fa-envelope"></i></a>
        <a href="https://scholar.google.com/citations?user=zDVmnM4AAAAJ&hl=en&oi=sra" title="Google Scholar"><i class="fa-solid fa-graduation-cap"></i></a>
      </div>
    </aside>
    <div class ="rightcol">
        <main class="content">
        <p>
            I am a first-year Master's student in Computer Science at McGill University and MILA, where I am advised by <a href = "https://mila.quebec/en/directory/siamak-ravanbakhsh"> Siamak Ravanbakhsh </a>. I completed my undergraduate degree in Computer Science at Princeton University, where I was advised by <a href = "https://cocosci.princeton.edu/tom/index.php"> Tom Griffiths </a>. There, I pursued minors in Cognitive Science and Latin American Studies, and I served as a <a href = "https://writing.princeton.edu/undergraduates/writing-center"> Writing Center </a> Head Fellow and Editor-In-Chief of the <a href="https://tortoise.princeton.edu/"><i>Tortoise</i></a> Journal. 
        </p>
        <p>
            I am broadly interested in <strong>reinforcement learning</strong> as a methodology for building more efficient,
            generalizable and structured AI systems. My <a href = "#srthesis"> undergraduate senior thesis </a> investigated the challenge of learning long-horizon humanoid locomotion in high-dimensional continuous control, where naïve RL faces an enormous exploration burden. I developed a hierarchical reinforcement learning framework that leveraged insights from human motor development to decompose locomotion into a sequence of tractable postural skills. My thesis was awarded the <a href = "https://cogsci.princeton.edu/news/announcing-2026-winners-senior-thesis-prizes-cognitive-science"> George A. Miller Prize in Cognitive Science </a> and the Sigma Xi Book Award. 
        </p> 
        <p>  
            Under the mentorship of Brad Malin at Vanderbilt University Medical Center, I developed a
            <a href = "#rlsyn"> sample-efficient RL-based generative model for privacy-preserving synthetic health data </a>
            that outperformed existing state-of-the-art GAN and diffusion models, particularly when confronted with limited training samples. In subsequent work, this <a href = "#regression"> framework was extended with regression-based rewards </a> to improve the preservation of statistical relationships in synthetic data. I also contributed to the <a href = "https://aws.amazon.com/marketplace/pp/prodview-mxp3i7s3ugkxq"> Synthetic AI-READI dataset <a>, a multimodal synthetic cohort for Type 2 Diabetes research now publically available. 
        </p>
        <p>
            My research is more broadly motivated by human-centered AI: both how AI can help humans, and how insights from human learning and cognition can inspire more efficient algorithms. Previously, I’ve worked on various applications of machine learning in healthcare settings. Under the mentorship of Weiqing Gu at <a href = https://data-to-decision.com/ >Dasion </a>, I built a
            <a href="#dasion">voice analysis model</a> to detect various medical conditions—including autism, diabetes and depression—from audio data. I also spent a summer at the University of Macedonia–Thessaloniki, where I built a
            <a href="#umacedonia">stacked autoencoder model</a> to classify MRI brain scans from autistic and neurotypical individuals. 
        </p>
        <hr style="border: 0; border-top: 1px solid #ddd; margin: 2em 0;">
        <h2 id="publications">Publications</h2>
        <div class="pub-card" id = "rlsyn">
          <strong>A Reinforcement Learning Approach to Synthetic Data Generation</strong><br>
          <a href="https://arxiv.org/abs/2512.21395">Preprint; </a> <em> Accepted at the Journal of Biomedical Informatics </em> | <a href=https://github.com/natalia-espinosadice/RLSyn>Code</a>
          <p>
          Synthetic data generation is a promising approach for enabling data sharing in biomedical studies while preserving patient privacy. Yet, state-of-the-art generative models often require large datasets and complex training procedures, limiting their applicability in small-sample settings common in biomedical research. This study aims to develop a more principled and efficient approach to SDG and evaluate its efficacy for biomedical applications. In this work, we reframe SDG as a reinforcement learning (RL) problem and introduce RLSyn, a novel framework that models the data generator as a stochastic policy over patient records and optimizes it using Proximal Policy Optimization with discriminator-derived rewards. We evaluate RLSyn on two biomedical datasets--AI-READI and MIMIC-IV--and benchmark it against state-of-the-art generative adversarial networks (GANs) and diffusion-based methods across extensive privacy, utility, and fidelity evaluations. On MIMIC-IV, RLSyn achieves predictive utility comparable to diffusion models (S2R AUC 0.902 vs 0.906 respectively) while slightly outperforming them in fidelity (NMI 0.001 vs. 0.003; DWD 2.073 vs. 2.797) and achieving comparable, low privacy risk (~0.50 membership inference risk AUC). On the smaller AI-READI dataset, RLSyn again matches diffusion-based utility (S2R AUC 0.873 vs. 0.871), while achieving higher fidelity (NMI 0.001 vs. 0.002; DWD 13.352 vs. 16.441) and significantly lower vulnerability to membership inference attacks (AUC 0.544 vs. 0.601). Both RLSyn and diffusion-based models substantially outperform GANs across utility and fidelity on both datasets. Our results suggest that reinforcement learning provides a principled and effective approach for synthetic biomedical data generation, particularly in data-scarce regimes. 
          </p>
        </div>
        <div class="pub-card" id = "regression">
          <strong>Reward-Guided Generation Improves the Scientific Utility of Synthetic Biomedical Data</strong><br>
          <a href="https://www.medrxiv.org/content/10.64898/2026.03.11.26348077v1.full.pdf">Preprint</a>
          <p>
           Synthetic data generation is a promising approach for biomedical data sharing and dataset augmentation, yet existing methods lack mechanisms to preserve statistical properties necessary for scientific analysis. To address this, we introduce RLSYN+REG, a reinforcement learning-driven generative model, which encourages that regression models trained on synthetic data reproduce the coefficients and predictions of their real-data counterparts. We evaluate RLSYN+REG on MIMIC-III and the American Community Survey (ACS) across regression model reproduction, fidelity to real data, and privacy. Synthetic data from RLSYN+REG substantially improves upon that of RLSYN, raising correlations between real and synthetic regression coefficients from 0.054 to 0.600 on MIMIC-III and from 0.160 to 0.376 on ACS. Predictive performance also improves, reducing the gap between real-data baselines by 81.4% and 97.6% on MIMIC-III and ACS, respectively. These improvements come with negligible cost to fidelity or privacy and are robust to reductions in training data.
          </p>
        </div>
        <hr style="border: 0; border-top: 1px solid #ddd; margin: 2em 0;">
        <h2>Research</h2>
        <div class="research">
          <div class="pub-card" id="srthesis">
            <strong>Learning to Walk Like Humans Do: A Developmental Approach to Locomotion in Deep RL </strong><br>
            <em> Senior Thesis at Princeton University, Spring 2026</em><br>
            <em> Awarded the 2026 George A. Miller Prize in Cognitive Science and the Sigma Xi Book Award. </em><br>
            <a href="/seniorthesis.pdf">PDF</a> | 
            <p>
              Humans learn to stand and walk within a matter of months, exploiting a reliable sequence of postural milestones that partitions the full motor configuration space into a series of stable, tractable subproblems. In contrast, humanoid agents trained with standard reinforcement learning (RL) enjoy no such structure, confronting the full complexity of locomotion at once and facing an enormous exploration burden in
              high-dimensional continuous control. To address this, we propose a hierarchical reinforcement learning (HRL) framework that leverages the structure of human motor development by training each key postural transition—prone-to-crawl, crawl-to-kneel, kneel-to-lunge, lunge-to-stand and stand-to-walk—as a distinct low-level policy, thus imposing a developmental prior over the skill set. A high-level policy then learns to coordinate these motor skills via the Value Function Spaces (VFS) framework. We first validate our approach in LunarLander and BipedalWalker before applying it to Humanoid, where developmental structure directly informs the skill decomposition. Against flat RL baselines and HRL methods that discover structure from experience, our approach achieves upright posture in over 90% of evaluation episodes and completes the full developmental sequence in over 85%, while all baselines plateau at intermediate configurations. Our findings suggest that developmentally grounded structural priors substantially reduce the exploration burden of complex locomotion
              learning, enabling reliable postural progression where reward engineering, intrinsic motivation and emergent hierarchies fall short.
            </p>
          </div>
          <div class="pub-card">
            <strong>Reimplementing MR.Q: The Role of Representations</strong><br>
            <em>Final Project for COS 435 at Princeton University, Spring 2025</em><br>
            <a href="/COS435_Final_Report.pdf">PDF</a> | 
            <a href="https://github.com/natalia-espinosadice/COS-435-RL-MrQ">Code</a>
            <p>
              This project investigated the role of representations in MR.Q, a generalist reinforcement learning algorithm. We asked two key questions: (i) Does an explicit planner still matter once you have a strong MR.Q-style representation? and (ii) How small can that representation become before performance deteriorates? We found that a one-step planning update often failed to help and even hurt performance - particularly in sparse-reward, pixel-based Atari tasks - while scaling down representation size proved more forgiving in discrete or lower-dimensional domains than in complex continuous-control settings.
            </p>
          </div>
          <div class="pub-card">
          <strong>Predicting Future Drug Trafficking Hotspots in Colombia</strong><br>
          <em>Junior Independent Work at Princeton University, Fall 2024</em><br>
          <a href="/iw_fall24.pdf">PDF</a> | 
          <a href="https://github.com/natalia-espinosadice/predicting-drug-trafficking-hotspots">Code</a>
          <p>
            This project applied machine learning to forecast drug trafficking activity across Colombia’s departments using United Nations seizure data. Socioeconomic indicators and engineered time-series features were used to train Random Forest, SVM and XGBoost models, with XGBoost achieving the best performance. The analysis revealed key drivers such as crime rates, government operations and urban–rural population patterns, offering an empirical analysis of existing socioeconomic theories.
          </p>
          </div>
          <div class="pub-card" id="umacedonia">
            <strong>Classifying and Understanding Autism from Brain Scans</strong><br>
            <em>Research at University of Macedonia-Thessaloniki, Summer 2024</em><br>
            <a href="https://github.com/natalia-espinosadice/brainscan-autoencoder">Code</a>
            <p>
              This project applied stacked autoencoders to structural MRI scans from the Autism Brain Imaging Data Exchange (ABIDE) dataset. The models were trained to compress and reconstruct brain images, and the learned representations were used to classify scans as autistic or normally developing. To probe group differences, the models were cross-tested - trained on one group and evaluated on the other - so that discrepancies in reconstruction quality could highlight structural variations between autistic and non-autistic brains.
            </p>
          </div>
          <div class="pub-card" id="dasion">
          <strong>Voice-Based ML for Diagnosis</strong><br>
          <em>Industry Research at Dasion, 2023-2024</em>
          <p>
            This project developed machine learning pipelines to diagnose various health conditions from voice recordings. Work focused on creating robust preprocessing strategies to handle noisy, real-world data, along with advanced feature extraction and classification techniques to support accurate diagnosis.
          </p>
          </div>
        </div>
        <hr style="border: 0; border-top: 1px solid #ddd; margin: 2em 0;">
        Last updated September 2026
        </main>  
    </div>
  </div>
</div>
<style>
.fullbleed{
  width: min(1100px, 95vw);
  margin-left: calc(50% - min(1100px, 95vw)/2);
  margin-right: calc(50% - min(1100px, 95vw)/2);
}
.push-right{
  --offset: 120px; /* tweak 80–180px until it looks perfect */
  margin-left: calc(32% - min(1500px, 95vw)/2 + var(--offset));
  margin-right: calc(33% - min(1500px, 95vw)/2 - var(--offset));
}
.two-col{
  display: grid;
  grid-template-columns: 360px 1fr;  /* sidebar + main */
  gap: 36px;
  align-items: start;
}
.profile-card{
  position: sticky; top: 24px;
  border-radius: 14px; padding: 18px; border: 1px solid #eee;
  box-shadow: 0 6px 22px rgba(0,0,0,.06); background:#fff;
  text-align: center;
}
.profile-card img{
  width: 100%; border-radius: 18px; display: block; margin-bottom: 14px;
  box-shadow: 0 5px 18px rgba(0,0,0,.08);
}
.profile-name{ font-size: 1.25rem; margin: 8px 0 4px; }
.affil{ color:#555; margin: 0 0 8px; }
.icon-row{ display:flex; justify-content:center; gap:16px; margin-top:10px; font-size:1.5rem; }
.icon-row a{ color:#2b4dbd; }
.icon-row a:hover{ transform: translateY(-2px); transition: .15s ease; }
.rightcol{
  display:flex;
  flex-direction:column;
  gap:12px;              
  margin:0;
}
.pubs{ margin:0; padding:0; }
.pubs::before{
  content:"";
  display:block;
  height:1px;
  background:#ddd;
  margin: 6px 0 10px;
}
.pubs h2{
  margin:0 0 8px !important;
  line-height:1.2;
}
.pub-card{
  border:1px solid #eee; background:#fff;
  border-radius:10px; padding:12px 14px;
}
@media (max-width: 900px){
  .two-col{ grid-template-columns: 1fr; }
  .profile-card{ position: static; }
}
</style>
