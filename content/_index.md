+++
draft = false
title = 'Home'
+++
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
        <a href = "/CV.pdf" title="CV"><i class="ai ai-cv"></i></a>
        %<a title="Google Scholar"><i class="ai ai-google-scholar"></i></a>%
        <a href="https://github.com/natalia-espinosadice" title="GitHub"><i class="fab fa-github"></i></a>
        <a href="https://www.linkedin.com/in/natalia-espinosa-dice" title="LinkedIn"><i class="fab fa-linkedin"></i></a>
        <a href="mailto:nespinosadice22@gmail.com" title="Email"><i class="fas fa-envelope"></i></a>
      </div>
    </aside>
    <div class ="rightcol">
        <main class="content">
        <p>
            I am a senior undergraduate in Computer Science at Princeton University, where I am advised by <a href = "https://cocosci.princeton.edu/tom/index.php"> Tom Griffiths </a>. I am pursuing minors in Cognitive Science and Latin American Studies. I also serve as a <a href = "https://writing.princeton.edu/undergraduates/writing-center"> Writing Center </a> Head Fellow and Editor-In-Chief of the <a href="https://tortoise.princeton.edu/"><i>Tortoise</i></a> Journal.
        </p>
        <p>
            I am broadly interested in <strong>reinforcement learning</strong> as a methodology for building more efficient,
            generalizable and structured AI systems. Under the mentorship of Brad Malin at Vanderbilt University Medical Center, I developed a
            <a href = "#publications">
            sample-efficient RL-based generative model for privacy-preserving synthetic health data
            </a>
            that outperformed existing state-of-the-art GAN and diffusion models, particularly when confronted with limited
            training samples. For my
            <a href = "#jrthesis">junior thesis</a> at Princeton, I explored how an agent
            could ‘learn to walk like humans do’ via a developmentally inspired RL curriculum and expanding neural networks.
            My <a href="#srthesis">senior thesis</a> extends this work by introducing a
            hierarchical RL framework that sequences motor skills through value functions, enabling online
            composition. 
        </p>
        <p>
            My research is more broadly motivated by human-centered AI: both how AI can help humans, and how insights from human learning and cognition can inspire more efficient algorithms. Previously, I’ve worked on various applications of machine learning in healthcare settings. Under the mentorship of Weiqing Gu at <a href = https://data-to-decision.com/ >Dasion </a>, I built a
            <a href="#dasion">voice analysis model</a> to detect various medical conditions—including autism, diabetes and depression—from audio data. I also spent a summer at the University of Macedonia–Thessaloniki, where I built a
            <a href="#umacedonia">stacked autoencoder model</a> to classify MRI brain scans as autistic or normally developing.
        </p>
        <p>
        <strong>I am applying to PhD programs this application cycle.</strong>
        </p>
        <hr style="border: 0; border-top: 1px solid #ddd; margin: 2em 0;">
        <h2 id="publications">Publications</h2>
        <div class="pub-card">
          <strong>Sample-Efficient Synthetic Data Generation via Reinforcement Learning</strong><br>
          <em>Preprint coming soon!</em><br>  
          <p>
          Synthetic health data offers a powerful tool for enabling machine learning research while protecting patient privacy and addressing data access barriers. However, existing generative models often struggle in small-sample settings, limiting their utility in domains where data is scarce. This project introduces a reinforcement learning–based framework for synthetic electronic health record (EHR) generation. Using the NIH Bridge2AI AI-READI diabetes dataset as a testbed, we benchmarked our RL model against state-of-the-art EHR generative approaches, including GAN-based and diffusion-based methods. On the AI-READI dataset, the RL model achieved higher downstream utility, closer statistical fidelity and lower privacy risks than competing models. When scaled to the larger MIMIC-IV EHR dataset, the RL framework matched the performance of existing state-of-the-art models, demonstrating both robustness and scalability.
          </p>
        </div>
        <hr style="border: 0; border-top: 1px solid #ddd; margin: 2em 0;">
        <h2>Research</h2>
        <div class="research">
          <div class="pub-card" id="srthesis">
            <strong>Hierarchical Developmental RL</strong><br>
            <em>Senior Thesis at Princeton University, Present</em><br>
            <p>
              This work introduces a hierarchical reinforcement learning framework inspired by human developmental trajectories. Individual motor skills are trained separately with their own policies and value functions. A higher-level controller then selects among these skills by consulting their value functions, enabling online composition and recovery if the agent falls. So far, we've tested our approach in toy environments (LunarLander, Cartpole swing-up) and are working to extend the method to full Humanoid locomotion.
            </p>
          </div>
          <div class="pub-card" id="jrthesis">
            <strong>Learning to Walk Like Humans Do</strong><br>
            <em> Junior Thesis at Princeton University, Spring 2025</em><br>
            <a href="/juniorthesis_spring25.pdf">PDF</a> | 
            <a href="https://github.com/natalia-espinosadice/learning-to-walk-rl">Code</a>
            <p>
              This project explored how principles of human motor development could improve reinforcement learning for humanoid locomotion. 
              Two strategies were investigated in parallel: (i) a curriculum of locomotion subtasks aligned with developmental milestones 
              (ex: crawling before standing) and (ii) progressively expanding neural networks that “grow” in depth or width as task complexity increases. Baseline results highlighted both the promise and the challenges of transferring knowledge across subtasks. These experiments laid the groundwork for the senior thesis work detailed above.
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
        Last updated October 2025
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
