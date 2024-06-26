---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
background: '/img/dalle.jpg'
---

<style>
.responsive {
  width: 35%;
  height: auto;
  float: left;
  border: 5px solid #555;
  padding: 5px 5px 5px 5px;
  margin-right: 15px;
  margin-bottom: 15px;
</style>

<style>
* {
  box-sizing: border-box;
}

/* The actual timeline (the vertical ruler) */
.timeline1 {
  position: relative;
  max-width: 1200px;
  margin: 0 auto;
}

/* The actual timeline (the vertical ruler) */
.timeline1::after {
  content: '';
  position: absolute;
  width: 6px;
  background-color: black;
  top: 20px;
  bottom: 0;
  left: 50%;
  margin-left: -3px;
}

/* Container around content */
.container1 {
  padding: 10px 40px;
  position: relative;
  background-color: inherit;
  width: 50%;
}

/* The circles on the timeline */
.container1::after {
  content: '';
  position: absolute;
  width: 25px;
  height: 25px;
  right: -12px;
  background-color: black;
  border: 4px solid #FF9F55;
  top: 15px;
  border-radius: 50%;
  z-index: 1;
}

/* Place the container to the left */
.left1 {
  left: 0;
}

/* Place the container to the right */
.right1 {
  left: 50%;
}

/* Add arrows to the left container (pointing right) */
.left1::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  right: 30px;
  border: medium solid lightgrey;
  border-width: 10px 0 10px 10px;
  border-color: transparent transparent transparent lightgrey;
}

/* Add arrows to the right container (pointing left) */
.right1::before {
  content: " ";
  height: 0;
  position: absolute;
  top: 22px;
  width: 0;
  z-index: 1;
  left: 30px;
  border: medium solid lightgrey;
  border-width: 10px 10px 10px 0;
  border-color: transparent lightgrey transparent transparent;
}

/* Fix the circle for containers on the right side */
.right1::after {
  left: -12px;
}

/* The actual content */
.content1 {
  padding: 15px 20px;
  background-color: lightgrey;
  position: relative;
  border-radius: 6px;
  border-color: black;
}

/* Media queries - Responsive timeline on screens less than 600px wide */
@media screen and (max-width: 600px) {
  /* Place the timelime to the left */
  .timeline1::after {
  left: 31px;
  }
  
  /* Full-width containers */
  .container1 {
  width: 100%;
  padding-left: 70px;
  padding-right: 25px;
  }
  
  /* Make sure that all arrows are pointing leftwards */
  .container1::before {
  left: 60px;
  border: medium solid black;
  border-width: 10px 10px 10px 0;
  border-color: transparent lightgrey transparent transparent;
  }

  /* Make sure all circles are at the same spot */
  .left1::after, .right1::after {
  left: 15px;
  }
  
  /* Make all right containers behave like the left ones */
  .right1 {
  left: 0%;
  }
}
</style>

<figure>
    <img src="/img/me.jpg" alt="Alex Chan" class="responsive"/>
<figure>

<p markdown="1">
Hi! I'm **Alex**, a Machine Learning PhD student at Cambridge, currently interning at Spotify. I am interested in developing safe and robust machine learning systems that behave in the way we expect, and
thus able to work with humans effectively. My work has often explored inverse reinforcement learning and
imitation learning in order to learn from humans, and I’m interested in using this knowledge and generative
AI to create insight and develop personalised, human-centric, decision making systems.
</p>

<p markdown="1">
If for some reason you're interested in [who I am](/about) or [what I do](/research) then you've come to the right place. However, if you can't find something feel free to get in contact through one of the many ways available in the modern world - including my [email](mailto:me@alexjchan.com) and this [form](/contact).
</p>

<p markdown="1">
[CV](/docs/Academic_CV.pdf){:target="_blank"} | [Email](mailto:me@alexjchan.com) | [Google Scholar](https://scholar.google.com/citations?user=yfy_BGIAAAAJ&hl=en&oi=sra){:target="_blank"} | [Github](https://github.com/XanderJC){:target="_blank"} | [LinkedIn](https://www.linkedin.com/in/alexjchan/){:target="_blank"} | [Twitter](https://twitter.com/AlexJChan){:target="_blank"}
</p>

<h1>Recent News</h1>

<div class="timeline1">
<div class="container1 left1">
    <div class="content1">
      <h3>Jan 2024</h3>
      <p markdown="1">  [**How to Catch an AI Liar: Lie Detection in Black-Box LLMs by Asking Unrelated Questions**](https://openreview.net/forum?id=567BjxgaTp){:target="_blank"}  accepted to ICLR 2024!</p>
    </div>
  </div>
  <div class="container1 right1">
    <div class="content1">
      <h3>Sep 2023</h3>
      <p markdown="1"> Two papers accepted to NeurIPS 2023: [**AllSim: Systematic Simulation and Benchmarking of Repeated Resource Allocation Policies in Multi-User Systems with Varying Resources**](https://openreview.net/forum?id=wiw5mnja8W){:target="_blank"} and [**GAUCHE: A Library for Gaussian Processes in Chemistry**](https://openreview.net/forum?id=vzrA6uqOis){:target="_blank"}! Also a fun workshop paper: [**Optimising Human-AI Collaboration by Finding Convincing Explanations**](https://arxiv.org/abs/2311.07426){:target="_blank"}! </p>
    </div>
  </div>
<div class="container1 left1">
    <div class="content1">
      <h3>Jun 2023</h3>
      <p markdown="1">  Starting as a **Research Scientist Intern at Spotify** as part of the Satisfaction, Interaction and Algorithms (SIA) team, working on intergratings large language models into the content moderation pipeline using culturally finetuned models.</p>
    </div>
  </div>
  <div class="container1 right1">
    <div class="content1">
      <h3>Jan 2023</h3>
      <p markdown="1"> Taking part as a [**SERI-MATS Scholar**](https://www.serimats.org/){:target="_blank"} working with Owain Evans, investigating deception in large language models along with methods to detect a notion of lying using only black-box access.</p>
    </div>
  </div>
<div class="container1 left1">
    <div class="content1">
      <h3>Sep 2022</h3>
      <p markdown="1">  Accepted to NeurIPS 2022: [**Synthetic Model Combination: An Instance-wise Approach to Unsupervised Ensemble Learning**](https://openreview.net/forum?id=RgWjps_LdkJ){:target="_blank"}! </p>
    </div>
  </div>
  <div class="container1 right1">
    <div class="content1">
      <h3>Mar 2022</h3>
      <p markdown="1"> Awarded second place in the [**G-Research PhD prize in maths and data science**](https://www.gresearch.co.uk/article/g-research-phd-prize-in-maths-and-data-science-2022/){:target="_blank"} for best PhD draft dissertation!</p>
    </div>
  </div>
  <div class="container1 left1">
    <div class="content1">
      <h3>Jan 2022</h3>
      <p markdown="1"> Again, two papers accepted to ICLR! [**Inverse Online Learning: Understanding Non-Stationary and Reactionary Policies**](https://openreview.net/forum?id=DYypjaRdph2){:target="_blank"} and [**POETREE: Interpretable Policy Learning with Adaptive Decision Trees**](https://openreview.net/forum?id=AJsI-ymaKn_){:target="_blank"}. </p>
    </div>
  </div>
  <div class="container1 right1">
    <div class="content1">
      <h3>Oct 2021</h3>
      <p markdown="1"> [**The Medkit-learn(ing) Environment: Medical Decision Modelling through Simulation**](https://openreview.net/forum?id=Ayf90B1yESX){:target="_blank"} is accepted to the Neural Information Processing Systems (NeurIPS) main conference track on Datasets and Benchmarks.</p>
    </div>
  </div>
  <div class="container1 left1">
    <div class="content1">
      <h3>Jan 2021</h3>
      <p markdown="1"> First place in the [Hex Cambridge](https://hackcambridge.com){:target="_blank"} hackathon Optiver Challenge out of about 40 teams. Developed an algorithmic trading strategy for market making a dual listed product. </p>
    </div>
  </div>
  <div class="container1 right1">
    <div class="content1">
      <h3>Jan 2021</h3>
      <p markdown="1"> Two papers accepted to ICLR! [**Scalable Bayesian Inverse Reinforcement Learning**](https://openreview.net/forum?id=4qR3coiNaIv){:target="_blank"} and [**Generative Time-series Modeling with Fourier Flows**](https://openreview.net/forum?id=PpshD0AXfA){:target="_blank"}.</p>
    </div>
  </div>
  <div class="container1 left1">
    <div class="content1">
      <h3>Sep 2020</h3>
      <p markdown="1"> Graduated the MPhil in Machine Leaning and Machine Intelligence and started a PhD in Machine Learning for Healthcare at the University of Cambridge. </p>
    </div>
  </div>
  <div class="container1 right1">
    <div class="content1">
      <h3>May 2020</h3>
      <p markdown="1"> My first ever paper accepted to ICML: [**Unlabelled Data Improves Bayesian Uncertainty Calibration under Covariate Shift**](https://arxiv.org/abs/2006.14988){:target="_blank"}.</p>
    </div>
  </div>
</div>