---
layout: model
title: Sorafenib OS
image: assets/images/hcc.jpg
area: HCC
description:  A model to describe overall survival in patients with aHCC
---




<!------------------------>
<!------------------------>
<!-- Setting -->
<!------------------------>
<!------------------------>

<div class="box">

<h1 id="sett">Setting and Data</h1>

<h2>Setting </h2>
<p>
Data were taken from the BRISK-FL study - a randomised, double-blinded
phase III trial which compared Brivanib with Sorafenib as a first-line therapy
in patients with unresectable, advanced hepatocellular carcinoma (aHCC). 
Patients were randomised from
May 2009 until August 2011. Patients were recruited from Asia, Europe, the
Americas, Australia and Africa.
</p>

<h2> Estimand </h2>
<div class="box">
  <div class="row">
  
	  <div class="6u 12u$(medium)">
	    <div class="box">
  		  <h3> Patients </h3>
  		<p> 
  		Patients were eligible if they had advanced HCC 
  		and had no prior systemic therapy for HCC.
  		Patients were included if they had an Eastern Cooperative Oncology,
  		Group performance status (ECOG-PS) score of 0 or 1, a Child-Pugh A 
  		liver function score, and at least one untreated measurable 
  		lesion.
  		</p>
  	  </div>	
	  </div>
	  
	  <div class="3u 12u$(medium)">
		  <div class="box">
		  <h3> Intervention </h3>
		  <p> 
		  Patients received 400 mg of sorafenib twice per day plus 
		  brivanib-matched placebo.
		  </p>
		  </div>	
	   </div>
	  
	  <div class="3u$ 12u$(medium)">
		  <div class="box">
		  <h3> Outcome </h3>
		  <p> 
		  The primary outcome is overall survival which was measured from the
		  date of randomisation until the date of death by any cause.
		  </p>
		  </div>	
  </div>
</div>
</div>






<!------------------------>
<!------------------------>
<!-- Data -->
<!------------------------>
<!------------------------>
<h2 id="data">Data</h2>

<p> 
The dataset consisted of 570 patients of whom 412 (73%) observed an 
event and 158 (27%) did not. The median overall survival (95.8% CI) was 
9.9 (8.5, 11.5) months. 
</p>

<div class="row 200%">
	
	<div class="6u 12u$(medium)">

  <!-- Table -->
		<h3>Model Covariates</h3>
		
		<p> 
		The covariates selected for inclusion in the model were:<br>
		Vascular invasion (VI),Eastern Cooperative Oncology 
		Group (ECOG) Score, metastasis, log(alpha-fetoprotein (AFP)),
		albumin (ALB), (log) serum creatinine and Aetiology. An interaction
		term between VI and age was also included.
		</p>
		
      <div class="table-wrapper">
      <table>
 <thead>
  <tr>
   <th style="text-align:left;"> </th>
   <th style="text-align:left;"> N = 570 </th>
  </tr>
 </thead>
<tbody>
      <tr>
       <td style="text-align:left;"> <b>Vascular Invasion</b> </td>
       <td style="text-align:left;"> 161 (28%) </td>
      </tr>
      <tr>
       <td style="text-align:left;"> <b>Eastern Cooperative Oncology Group Score</b></td>
       <td style="text-align:left;"> </td>
      </tr>
      <tr>
        <td style="text-align:left;"> &nbsp;&nbsp;&nbsp;&nbsp;0 </td>
        <td style="text-align:left;"> 345 (61%) </td>
      </tr>
      <tr>
       <td style="text-align:left;"> &nbsp;&nbsp;&nbsp;&nbsp;1 </td>
       <td style="text-align:left;">  225 (39%) </td>
      </tr>
      <tr>
       <td style="text-align:left;"> <b>Metastasis</b> </td>
       <td style="text-align:left;"> 410 (72%) </td>
      </tr>
      <tr>
       <td style="text-align:left;"> <b>AFP</b> </td>
       <td style="text-align:left;"> 5.2 (2.1, 8.0) </td>
      </tr>
      <tr>
       <td style="text-align:left;"> <b>Albumin</b> </td>
       <td style="text-align:left;"> 39 (35, 42) </td>
      </tr>
      <tr>
       <td style="text-align:left;"> <b>Creatinine</b> </td>
       <td style="text-align:left;"> 4.31 (4.15, 4.46) </td>
      </tr>
      <tr>
       <td style="text-align:left;"> <b>AST</b> </td>
       <td style="text-align:left;"> 4.04 (3.56, 4.52) </td>
      </tr>
      <tr>
       <td style="text-align:left;"> <b>Aetiology</b> </td>
       <td style="text-align:left;">  </td>
      </tr>
      <tr>
        <td style="text-align:left;"> &nbsp;&nbsp;&nbsp;&nbsp;HCV </td>
        <td style="text-align:left;"> 111 (19%) </td>
      </tr>
      <tr>
       <td style="text-align:left;"> &nbsp;&nbsp;&nbsp;&nbsp;HBV </td>
       <td style="text-align:left;"> 248 (44%) </td>
      </tr>
       <tr>
       <td style="text-align:left;"> &nbsp;&nbsp;&nbsp;&nbsp;Other </td>
       <td style="text-align:left;"> 211 (37%) </td>
      </tr>
</tbody>
</table>
      </div>
  
  </div>
  <!-- End Table -->
  

  <div class="6u 12u$(medium)">
    <!-- Image -->
    <span class="image fit"><img src="{% link assets/images/at_bev_ka.png %}" alt="" /></span>
  </div>
     <!-- End Image -->
  </div>








<!------------------------>
<!------------------------>
<!-- Model -->
<!------------------------>
<!------------------------>



<div class="box">
<h1 id="data"> Model </h1>

<p> The model constructed was a flexible parametric survival model using
a spline function to model the underlying cumulative hazard function. Four internal
knots were chosen and were placed at the timepoints 3, 6 12, and 24 months. 
</p>

</div>