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
        <a href="/cv.pdf" title="CV"><i class="ai ai-cv"></i></a>
        <a href="https://scholar.google.com/citations?user=XXXXX" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>
        <a href="https://github.com/natalia-espinosadice" title="GitHub"><i class="fab fa-github"></i></a>
        <a href="https://www.linkedin.com/in/natalia-espinosa-dice" title="LinkedIn"><i class="fab fa-linkedin"></i></a>
        <a href="mailto:nespinosadice22@gmail.com" title="Email"><i class="fas fa-envelope"></i></a>
      </div>
    </aside>
    <div class ="rightcol">
        <main class="content">
        <p>
            I am a senior undergraduate in Computer Science at Princeton University, where I am advised by Tom Griffiths. I am pursuing minors in Cognitive Science and Latin American Studies. I also serve as a Writing Center Head Fellow and Editor-In-Chief of the <a href="https://tortoise.princeton.edu/"><i>Tortoise</i></a> Journal.
        </p>
        <p>
            I am broadly interested in <strong>reinforcement learning</strong> as a methodology for building more efficient,
            generalizable and structured AI systems. At Vanderbilt University Medical Center, I developed a
            <a href="projects/#sample-efficient-synthetic-data-generation-via-reinforcement-learning">
            sample-efficient RL-based generative model for privacy-preserving synthetic health data
            </a>
            that outperformed existing state-of-the-art GAN and diffusion models, particularly when confronted with limited
            training samples. For my
            <a href="projects/#learning-to-walk-like-humans-do">junior thesis</a> at Princeton, I explored how an agent
            could ‘learn to walk like humans do’ via a developmentally inspired RL curriculum and expanding neural networks.
            My <a href="projects/#hierarchical-developmental-rl">senior thesis</a> extends this work by introducing a
            hierarchical reinforcement learning framework that sequences motor skills through value functions, enabling online
            composition. 
        </p>
        <p>
            My research is more broadly motivated by human-centered AI: both how AI can help humans, and how insights from human learning and cognition can inspire more efficient algorithms. Previously, I’ve worked on various applications of machine learning in healthcare settings. At Dasion, I built a
            <a href="projects/#voice-based-machine-learning-for-diagnosis">voice analysis model</a> to detect various medical conditions—including autism, diabetes and depression—from audio data. I also spent a summer at the University of Macedonia–Thessaloniki, where I built a
            <a href="projects/#classifying-and-understanding-autism-from-brain-scans">stacked autoencoder model</a> to classify MRI brain scans as autistic or normally developing.
        </p>
        <p>
        <strong>I am applying to PhD and Master’s programs this application cycle.</strong>
        </p>
        <h2>Publications</h2>
            <div class="pub-card">
            <strong>Sample-Efficient Synthetic Data Generation via Reinforcement Learning</strong><br>
            Preprint coming soon!
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

/* push the block to the right without touching the centered H1 above it */
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

/* Sidebar card */
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

/* Icons */
.icon-row{ display:flex; justify-content:center; gap:16px; margin-top:10px; font-size:1.5rem; }
.icon-row a{ color:#2b4dbd; }
.icon-row a:hover{ transform: translateY(-2px); transition: .15s ease; }

/* Right column stack */
.rightcol{
  display:flex;
  flex-direction:column;
  gap:12px;               /* << only small space between intro and pubs */
  margin:0;
}



/* Publications */
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

/* Mobile */
@media (max-width: 900px){
  .two-col{ grid-template-columns: 1fr; }
  .profile-card{ position: static; }
}
</style>
