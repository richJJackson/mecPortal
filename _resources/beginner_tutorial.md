---
layout: post
order: 2
title: Beginner's Tutorial
description:  A beginners tutorial for PSCs
image: assets/images/beginner.jpg
---

<section id="one">
<div class="box-round">

<h2>What is a Personalised Synthetic Control?</h2>

<p>
A <b>Personalised Synthetic Control (PSC)</b> is a statistical model
that can estimate what might have happened to a treated patient
if they had instead received the current standard care. Rather than
comparing that patient to one average control group,
PSCs build an individualised prediction using information from 
similar patients and a counterfactual model.
</p>


</div>
</section>

<section id="two">
<div class="box-round">

<h2>Why use PSCs?</h2>

<p>PSCs answer the question: <i>how do patient outcomes under an observed experimental treatment compare with the expected outcome under the current standard of care?</i></p>

<ul>
  <li><b>They support individualised comparison:</b> each treated patient is compared against their own counterfactual prediction.</li>
  <li><b>They can be used in single-arm settings:</b> especially when no control arm is available.</li>
  <li><b>They use clinically relevant patient features:</b> such as prognostic baseline covariates.</li>
  <li><b>They provide interpretable treatment-effect summaries:</b> at patient level and cohort level.</li>
</ul>


</div>
</section>

<section id="three">
<div class="box-round">

<h2>How does a PSC work?</h2>



<ol>
  <li><b>Start with patient data.</b> Use data from patients treated the current standard of care.</li>
  <li><b>Fit a model on the patient data.</b> The model links baseline patient covariates to expected outcomes that standard of care.</li>
  <li><b>Apply the PSC model to a data cohort of patients treated with an experimental treatment</b> For each treated patient, predict their expected outcome under the standard care.</li>
  <li><b>Compare the actual observed versus predicted outcomes.</b> The difference between the observed treated outcome and the PSC prediction gives the estimated treatment effect.</li>
</ol>

</div>
</section>

<section id="four">
<div class="box-round">

<h2>A simple example</h2>

<p>
A patient with advanced cancer receives a new treatment 
in a single-arm study. We observe their survival time, 
but we do not observe what would have happened if that 
same patient had instead received standard care.
</p>

<p>
A PSC (built from standard-care patients with similar 
clinical characteristics, e.g., age, performance status,) predicts the
patient's expected outcome had they been treated with the current standard
treatment. If the treated patient's outcome is better than the predicted 
outcome, this may suggest that the experimental treatment has greater 
efficacy. 
</p>

<p>
It is important to remember that the comparison is
<b>personalised</b>: it is based on the treated patient's
own baseline characteristics.
</p>

</div>
</section>

<section id="five">
<div class="box-round">

<h2>What questions can PSCs help to answer?</h2>

<ul>
  <li>How does a treated patient's observed outcome compare with their expected outcome under the standard care?</li>
  <li>What is the estimated treatment effect across a treated cohort?</li>
  <li>What is the estimated treatment effect across different subgroups?</li>
</ul>


</div>
</section>



<section id="six">
<div class="box-round">

<h2>Key assumptions you should know</h2>

<p>PSCs have requirements. For a beginner, it is important to know that:</p>

<ul>
  <li>The method used to predict expected outcomes should fit the data structure well.</li>
  <li>The treated patients are comparable to the reference setting, so the treated data cohort
  should not be too different to the patient population used to build the PSC model.</li>
  <li>Outcomes, covariates should exist and mean the same thing in both datasets used.</li>
</ul>

<p>
The <a href="advanced_manual.html">Advanced Technical Manual</a> gives a more formal treatment of these assumptions.
</p>

</div>
</section>



<section id="nine">
<div class="box-round">

<h2>Beginner guide/tutorials</h2>


<ul class="actions">
  <li><a href="video_walkthrough.html" class="button ">Watch video tutorials for beginners</a></li>
</ul>

</div>
</section>

<section id="ten">
<div class="box-round">

<h2>Where next?</h2>

<p>Explore other resource that best matches your next step.</p>

<ul>
  <li><a href="getting_started_guide.html">Getting Started Guide</a></li>
  <li><a href="video_walkthrough.html">Video Walkthroughs</a> for guided demonstrations.</li>
  <li><a href="advanced_manual.html">Advanced Technical Manual</a></li>
  <li><a href="../learn/howto_formatData.html">Data preparation and formatting </a>tutorial.</li>
  <li><a href="../models.html">Available models</a> currently.</li>
</ul>

</div>
</section>
