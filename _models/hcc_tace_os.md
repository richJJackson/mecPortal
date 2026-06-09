---
layout: model
title: TACE OS
image: assets/images/hcc.jpg
area: HCC
description:  A model to describe overall survival in patients with HCC
---

<a id="top"></a>





<!------------------------>
<!------------------------>
<!-- Contents -->
<!------------------------>
<!------------------------>
<div class="section-nav">
  <a href="#setting">Setting</a> |
  <a href="#data">Data</a> |
  <a href="#mod">Model</a> |
  <a href="#valid">Validation</a> |
  <a href="#use">Use Model</a> |
  <a href="#ref">References</a>
</div>


<!------------------------>
<!------------------------>
<!-- Setting -->
<!------------------------>
<!------------------------>

<div class="box collapsible-section">


<div class="section-header">
  <h2 id="setting">Setting </h2>
</div>

<div class="section-content">
<p>
The data were derived from the TACE 2 trial, a randomized, double-blind, placebo-controlled phase III trial in patients with unresectable HCC. The study investigated whether the addition of sorafenib to TACE improved progression-free survival compared with TACE plus placebo.
</p>

<h2> Estimand </h2>

  <div class="row">
  
      <div class="6u 12u$(medium)">
        <div class="box">
          <h3> Patients </h3>
        <p> Patients had to have unresectable, liver-confined HCC, a patent main portal vein, an Eastern Cooperative Oncology Group (ECOG) performance score of ≤1, and Child–Pugh class A liver function.
        </p>
      </div>	
      </div>
      
      <div class="3u 12u$(medium)">
          <div class="box">
          <h3> Intervention </h3>
          <p> Patients received Tace+Placebo. Patients were received placebo combined with TACE using drug-eluting beads (DEB-TACE) performed 2-5 weeks 
        post-randomisation. Further DEB-TACE was performed according to radiological  response and patient tolerance. </p>
          </div>	
       </div>
      
      <div class="3u$ 12u$(medium)">
          <div class="box">
          <h3> Outcome </h3>
          <p>  The primary outcome was PFS and secondary outcomes included overall survival (OS), toxicity and QOL.
          </p>
          </div>	
  </div>
</div>

<div class="row">
<p>
<a href="#top">Back to Top</a>
</p>
</div>
</div>
</div>

<!------------------------>
<!------------------------>
<!-- Data -->
<!------------------------>
<!------------------------>

<div class="box collapsible-section">

<div class="section-header">
<h2 id="data">Data</h2>
</div>

<div class="section-content">
<p> The dataset consisted of 156 patients of whom 88 (56%) observed an 
event and 68 (44%) did not. The median overall survival (95% CI) was 
19.9(16.7,23.9) months. </p>

<div class="row 200%">
    
    <div class="6u 12u$(medium)">

  <!-- Table -->
        <h3>Model Covariates</h3>
        
        <p> The covariates selected for inclusion in the model were<br>
        Albumin-Bilirubin score (ALBI),  alpha-fetoprotein (AFP) and Maximum Tumour Size (MAXSZ) </p>
      <div class="table-wrapper">
      <table>
 <thead>
  <tr>
   <th style="text-align:left;"> </th>
   <th style="text-align:left;"> N = 156 </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> ALBI </td>
   <td style="text-align:left;"> -2.57 (-2.93, -2.25) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> AFP </td>
   <td style="text-align:left;"> 3.09 (1.61, 5.59) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> MAXSZ </td>
   <td style="text-align:left;"> 5.4 (3.6, 7.45) </td>
  </tr>
</tbody>
</table>
      </div>
  
  </div>
  <!-- End Table -->
  

  <div class="6u 12u$(medium)">
    <!-- Image -->
    <span class="image fit"><img src="{% link assets/images/fc4728cc-f72d-479f-9fcd-eafe43b2970f.png %}" alt="" /></span>
  </div>
     <!-- End Image -->
  </div>
<p>
  <a href="#top">Back to Top</a>
</p>
</div>
</div>




<!------------------------>
<!------------------------>
<!-- Model -->
<!------------------------>
<!------------------------>


<div class="box collapsible-section">

<div class="section-header">
  <h2 id="mod"> Model </h2>
</div>

<div class="section-content">
<p> The model constructed was a flexible parametric survival model using
a spline function to model the underlying cumulative hazard function. Four internal
knots were chosen and were placed at the timepoints 3, 6 12, and 24 months. 
</p>

<div class="row 200%">
    
    <div class="6u 12u$(medium)">
    <h3> Model Construction </h3>
    <div class="box">
        <p> Include details here about the process of fitting the model.  E.G. 
        backwards stepwise procedure based on model AIC. 
        </p>
    </div>
    
    <!-- Image -->
    <div>
      <h3>Model Fit</h3>
      Some text to describe what is provided
      <span class="image fit"><img src="{% link assets/images/TACE_km1.png %}" alt="" /></span>
    </div>
  
  </div>
    <!-- End Image -->
    
    
    
  <div class="6u 12u$(medium)">

<!-- Table -->
    
   <h4>Model Estimates</h4> 

  <div class="modelTable">
    
    <table>

 <thead>
  <tr>
  <th style="text-align:left;"> Parameter </th>
   <th style="text-align:left;"> Estimate (SE) </th>
   <th style="text-align:left;"> HR (95% CI) </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> gamma0 </td>
   <td style="text-align:left;"> -4.251 (0.976) </td>
   <td style="text-align:left;"> 0.01(0 - 0.1) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> gamma1 </td>
   <td style="text-align:left;"> 1.818 (0.398) </td>
   <td style="text-align:left;"> 6.16(2.82 - 13.45) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> gamma2 </td>
   <td style="text-align:left;"> 0.036 (0.049) </td>
   <td style="text-align:left;"> 1.04(0.94 - 1.14) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> ALBI </td>
   <td style="text-align:left;"> 0.839 (0.261) </td>
   <td style="text-align:left;"> 2.32(1.39 - 3.86) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> AFP </td>
   <td style="text-align:left;"> 0.174 (0.042) </td>
   <td style="text-align:left;"> 1.19(1.1 - 1.29) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> MAXSZ </td>
   <td style="text-align:left;"> 0.048 (0.026) </td>
   <td style="text-align:left;"> 1.05(1 - 1.1) </td>
  </tr>
</tbody>
</table>

  </div>
  <!-- End Table -->
  <div>
    <h3> Model Prediction</h3>
    See how this model can be used to predict survival!
    <ul class="actions">
      <li><a href="#" class="button special">Rshiny</a></li>
    </ul>
  </div>
 
 </div>
<a href="#top">Back to Top</a>
</div>
</div>
</div>

<!------------------------>
<!------------------------>
<!-- Validation -->
<!------------------------>
<!------------------------>

<div class="box collapsible-section">

<div class="section-header">
  <h2 id="valid"> Validation </h2>
</div>

<div class="section-content">
<h3> Validation Details </h3>

    <p> Validation are reported in term of Calibration, Discrimination and Somers' D.  
    Calibration is reported in terms of the Mallows C-Statistic and by regressing 
    the fitted linear predictor against the outcome (Slope). The linear predictor is 
    derived using the model's coefficients. <br>
    
    Discrimination is evaluated by categorising patients into 4 risk groups.  
    Risk groups are generated by using the 5th, 50th and 85th centiles of the 
    linear predictor. The risk groups are	compared graphically 
    and the relative risk is evaluated by fitting a 
    univariable Cox Proportional Hazards Model.
    </p>



<div class="row 200%">

    <div class="6u 12u$(medium)">

  <h4>Calibration</h4>
  
    <div class="table-wrapper">
  <table>
 <thead>
  <tr>
   <th style="text-align:left;">  </th>
   <th style="text-align:left;"> est (se) </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> C-Statistic </td>
   <td style="text-align:left;"> 0.70 (0.017) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Slope </td>
   <td style="text-align:left;"> 1.00 (0.101) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Somers' D </td>
   <td style="text-align:left;"> 0.41 </td>
  </tr>
</tbody>
</table>
  </div>

<h4>Discrimination</h4>
  
  <div class="table-wrapper">
    <table>
     <thead>
      <tr>
       <th style="text-align:left;"> </th>
       <th style="text-align:right;"> est (se) </th>
       <th style="text-align:right;"> HR (95% CI) </th>
      </tr>
     </thead>
    <tbody>
      <tr>
       <td style="text-align:left;"> Risk Group 1 </td>
       <td style="text-align:left;"> </td>
       <td style="text-align:left;"> </td>
      </tr>
      <tr>
       <td style="text-align:left;">  Risk Group 2 </td>
       <td style="text-align:left;">  0.06 (0.26) </td>
       <td style="text-align:left;"> 1.06 (0.63, 1.77) </td>
      </tr>
      <tr>
       <td style="text-align:left;"> Risk Group 3 </td>
       <td style="text-align:left;">  1.06 (0.24) </td>
       <td style="text-align:left;">  2.89 (1.81, 4.61) </td>
      </tr>
      <tr>
       <td style="text-align:left;"> Risk Group 4 </td>
       <td style="text-align:left;"> 1.82 (0.26) </td>
       <td style="text-align:left;"> 6.20 (3.70, 10.37) </td>
      </tr>
    </tbody>
    </table>
  
  </div>

  </div>
    <h3>Risk Separation</h3>
    <div class="6u 12u$(medium)">
      <!-- Image -->

  Kaplan Meier plot to show survival estimates within each of the 4 risk groups

  <span class="image fit"><img src="{% link assets/images/atBev_discrim.png %}" alt="" /></span>


   </div>

  </div>
<p>
<a href="#top">Back to Top</a>
</p>

</div>

</div>

<!------------------------>
<!------------------------>

<div class="box collapsible-section">

<div class="section-header">
  <h2 id="use"> Use this model </h2>
</div>

<div class="section-content">
<div class="row">
  <div class="5u 12u$(medium)">
    <div class="box">
    <p>
      Download this model and learn how to use it by visiting
        <ul class="actions">
          <li><a href= "github/richJJackson/pscLibrary/test_model" class="button special">Download</a> </li>
        </ul>
    </p>
    </div>
  </div>
</div>
<div class="row">
<p>
<a href="#top">Back to Top</a>
</p>
</div>
</div>
</div>

<!------------------------>
<!------------------------>

<div class="box collapsible-section">

  <div class="section-header">
    <h2 id="ref"> References </h2>
  </div>

  <div class="section-content">
    Details on the trial which provided the data for this model can be found at:
    
    Johnson, P.J. et al. (2013) ‘Brivanib Versus Sorafenib As First-Line 
    Therapy in Patients With Unresectable, Advanced Hepatocellular Carcinoma:
    Results From the Randomized Phase III BRISK-FL Study’, Journal of clinical 
    oncology, 31(28), pp. 3517–3524. 
    Available at: https://doi.org/10.1200/JCO.2012.48.4410.
  </div>
</div>

<p>
<a href="#top">Back to Top</a>
</p>