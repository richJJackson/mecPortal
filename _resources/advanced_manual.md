---
layout: post
order: 3
title: Advanced Technical Manual
description: Technical guidance for implementing Personalised Synthetic Controls
image: assets/images/technical-manual.jpg
---



<section id="one">
<div class="box-round">

<h2>Core Technical Manuals</h2>

<p>Use the links below for complete function-level documentation and a full worked example.</p>
<ul class="actions">
      <li><a href="https://cran.r-project.org/web/packages/psc/psc.pdf" target="_blank" rel="noopener noreferrer" class="button special glass big">CRAN Reference Manual</a></li>
</ul>

<p>
The vignette includes methodology details, package workflows, and a motivating survival example.
  <ul class="actions">
      <li><a href="https://richjjackson.github.io/psc/articles/psc.html" target="_blank" rel="noopener noreferrer" class="button special glass big">PSC Vignette</a></li>
  </ul>
</p>

</div>
</section>

<section id="two">
<div class="box-round">

<h2>Methodology</h2>

<p><b>Personalised Synthetic Controls (PSCs)</b> estimate counterfactual outcomes for treated individuals by combining:</p>
<ul>
  <li>a model for outcomes under the current standard care, and</li>
  <li>patient-level covariates for the treated data cohort.</li>
</ul>

<p>This enables treatment-effect estimation when a direct randomised control arm is unavailable.</p>

<h3>Key assumptions to report</h3>
<ul>
  <li><b>Conditional exchangeability:</b> key prognostic factors affecting treatment and outcome are measured.</li>
  <li><b>Stable Unit Treatment Variability Assumption</b> each patient's potential outcome is not altered by other patients or treatment-label representation.</li>
  <li><b>Correct model specification:</b> the parametric counterfactual model is appropriate for endpoint type and covariate structure.</li>
  <li><b>Posterior approximation:</b> the estimation procedure assumes the model posterior is well-approximated by a multivariable normal distribution.</li>
  <li><b>Transportability:</b> application of the CFM from its development setting to the target cohort.</li>
  <li><b>Positivity/overlap:</b> treated patients have non-zero control probability and inference remains within supported covariate ranges.</li>
  <li><b>Data consistency:</b> endpoint definitions, covariate coding, and follow-up windows are aligned across datasets.</li>
  <li> <a href="../framework.html">Read more about PSC assumptions</a></li>
</ul>

<h3>Recommended technical outputs</h3>
<ul>
  <li>covariate balance and overlap diagnostics,</li>
  <li>model fit checks and calibration summaries,</li>
</ul>

</div>
</section>


<section id="three">
<div class="box-round">

<h2>Package Workflow</h2>

<ol>
  <li><b>Prepare data</b> with required variables and consistent coding.</li>
  <li><b>Fit base model</b> for the standard-care outcome process.</li>
  <li><b>Create a PSC counterfactual model</b> (using the pscCFM() function in the psc package).</li>
  <li><b>Compare treated cohort vs counterfactual predictions</b> using PSCfit() function.</li>
  <li><b>Summarize and visualize</b> treatment effects.</li>
</ol>

<p>See the vignette for current function names, argument signatures, and endpoint-specific examples.</p>

<h3>Implementation</h3>
<ul>
  <li>.</li>
</ul>

<h3>Recommended reporting structure</h3>
<ul>
  <li><b>Data:</b> Background, eligibility criteria, missingness handling.</li>
  <li><b>Model:</b> formula/structure, fitting strategy.</li>
  <li><b>Diagnostics:</b> overlap, calibration, validation.</li>
  <li><b>Results:</b> estimates, interval estimates, subgroup summaries.</li>
</ul>

</div>
</section>
