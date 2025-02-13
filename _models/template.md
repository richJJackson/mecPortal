---
layout: model
title: TACE OS in HCC
image: assets/images/TACE_km1.png
area: tmpArea
description:  A template of the information to include
---

<!------>
<!------>

<!-- Setting -->
# Setting 
A quick description of the model setting is provided:  E.G. This model
predicts the survival of patients with Hepatocellular Carcinoma (HCC) BCLC stage 
B and treated with Trans Arterial Chemoembolisation (TACE).  The model has been 
generated on the data from the TACE + Placebo arm from the TACE 2 trials.

<div class="row">
	<div class="4u 12u$(medium)">
		<h3> Patients </h3>
		<p> Details on the Patients (e.g. inclusion/exclusion criteria from the 
		study) </p>
	</div>
	<div class="4u 12u$(medium)">
		<h3> Intervention </h3>
		<p> How was the intervention delivered? </p>
	</div>
	<div class="4u$ 12u$(medium)">
		<h3> Outcome </h3>
		<p> How is the Outcome defined?  E.G. Overall Survival measured as the time 
		from randomisation until death by any cause </p>
	</div>
</div>


<!------>
<!------>


<!-- Data -->
<h1 id="data">Data</h1>

<p> A description of the data used to generate the model </p>

<div class="row 200%">
	
	<div class="6u 12u$(medium)">

		<h4>Covariates</h4>
		
		<p> A list of all available data in the construction of the description of 
		all the covariates that wew included in the dataset </p>
		
		<ul>
			<li> Covariate 1</li>
			  <p> Details of how it is maesured (eg. units) </p>
			<li> Covariate 2</li>
			  <p> Details of how it is maesured (eg. units) </p>
			<li> Covariate 3</li>
			  <p> Details of how it is maesured (eg. units) </p>
			<li> Covariate 4</li>
			  <p> Details of how it is maesured (eg. units) </p>
		</ul>

  <!-- Table -->
  
  <h4>Example Table of covariate summaries</h4>
  <div class="table-wrapper">
  	<table>
  		<thead>
  			<tr>
  				<th>Name</th>
  				<th>Description</th>
  				<th>Price</th>
  			</tr>
  		</thead>
  		<tbody>
  			<tr>
  				<td>Item1</td>
  				<td>Ante turpis integer aliquet porttitor.</td>
  				<td>29.99</td>
  			</tr>
  			<tr>
  				<td>Item2</td>
  				<td>Vis ac commodo adipiscing arcu aliquet.</td>
  				<td>19.99</td>
  			</tr>
  			<tr>
  				<td>Item3</td>
  				<td> Morbi faucibus arcu accumsan lorem.</td>
  				<td>29.99</td>
  			</tr>
  			<tr>
  				<td>Item4</td>
  				<td>Vitae integer tempus condimentum.</td>
  				<td>19.99</td>
  			</tr>
  			<tr>
  				<td>Item5</td>
  				<td>Ante turpis integer aliquet porttitor.</td>
  				<td>29.99</td>
  			</tr>
  		</tbody>
  		<tfoot>
  			<tr>
  				<td colspan="2"></td>
  				<td>100.00</td>
  			</tr>
  		</tfoot>
  	</table>
  </div>
  
  <!-- End Table -->
  
  </div>
  

  
  <div class="6u 12u$(medium)">
    <!-- Image -->
    <h3>Model covariates</h3>
    Details of the covariates used to generate the model are:
    <span class="image fit"><img src="{% link assets/images/TACE_dataPlot.png %}" alt="" /></span>
    </div>
     <!-- End Image -->
  </div>



<!------>
<!------>
 
<!-- Model -->
<h1 id="data"> Model </h1>

<p> A description of the data used to generate the model: </p>

<div class="row 200%">
	
	<div class="6u 12u$(medium)">
    <h3> Model Construction </h3>
    <div class="box">
    	<p> Include details here about the process of fitting the model.  E.G. 
    	backwards stepwise procedure based on model AIC </p>
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
	
  <h4>Example Table of covariate summaries</h4>
  <div class="modelTable">
  	
  	<table>
      <thead>
      <tr>
       <th style="text-align:left;">   </th>
       <th style="text-align:right;"> est </th>
       <th style="text-align:right;"> se </th>
      </tr>
     </thead>
    <tbody>
      <tr>
       <td style="text-align:left;"> gamma0 </td>
       <td style="text-align:right;"> -3.148 </td>
       <td style="text-align:right;"> 1.269 </td>
      </tr>
      <tr>
       <td style="text-align:left;"> gamma1 </td>
       <td style="text-align:right;"> 1.778 </td>
       <td style="text-align:right;"> 0.395 </td>
      </tr>
      <tr>
       <td style="text-align:left;"> gamma2 </td>
       <td style="text-align:right;"> 0.031 </td>
       <td style="text-align:right;"> 0.050 </td>
      </tr>
      <tr>
       <td style="text-align:left;"> AFP </td>
       <td style="text-align:right;"> 0.174 </td>
       <td style="text-align:right;"> 0.043 </td>
      </tr>
      <tr>
       <td style="text-align:left;"> Cirrhosis1 </td>
       <td style="text-align:right;"> -0.389 </td>
       <td style="text-align:right;"> 0.313 </td>
      </tr>
      <tr>
       <td style="text-align:left;"> Albumin </td>
       <td style="text-align:right;"> -0.070 </td>
       <td style="text-align:right;"> 0.025 </td>
      </tr>
      <tr>
       <td style="text-align:left;"> Lesion1 </td>
       <td style="text-align:right;"> 0.025 </td>
       <td style="text-align:right;"> 0.028 </td>
      </tr>
    </tbody>
  </table>
  </div>
  <!-- End Table -->
  <div>
    <h3> Model Preduction</h3>
    See how this model can be used to predict survival!
    <ul class="actions">
      <li><a href="#" class="button special">Rshiny</a></li>
    </ul>
  </div>
 
 </div>
  
</div>
 
 <!------>
 <!------>


<!-- Validation -->
<h1 id="data"> Validataion </h1>

<p> Details on the validation of the model: </p>


<h3> Validatation Details </h3>
<div class="box">
	<p> Provide some information on how the model is validated </p>
</div>


<div class="row 200%">

	<div class="6u 12u$(medium)">

  <h4>A table to provide Validation Details</h4>
  
  <div class="table-wrapper">
  	<table>
   <thead>
    <tr>
     <th style="text-align:left;">   </th>
     <th style="text-align:right;"> est </th>
     <th style="text-align:right;"> se </th>
    </tr>
   </thead>
  <tbody>
    <tr>
     <td style="text-align:left;"> gamma0 </td>
     <td style="text-align:right;"> -3.148 </td>
     <td style="text-align:right;"> 1.269 </td>
    </tr>
    <tr>
     <td style="text-align:left;"> gamma1 </td>
     <td style="text-align:right;"> 1.778 </td>
     <td style="text-align:right;"> 0.395 </td>
    </tr>
    <tr>
     <td style="text-align:left;"> gamma2 </td>
     <td style="text-align:right;"> 0.031 </td>
     <td style="text-align:right;"> 0.050 </td>
    </tr>
    <tr>
     <td style="text-align:left;"> AFP </td>
     <td style="text-align:right;"> 0.174 </td>
     <td style="text-align:right;"> 0.043 </td>
    </tr>
    <tr>
     <td style="text-align:left;"> Cirrhosis1 </td>
     <td style="text-align:right;"> -0.389 </td>
     <td style="text-align:right;"> 0.313 </td>
    </tr>
    <tr>
     <td style="text-align:left;"> Albumin </td>
     <td style="text-align:right;"> -0.070 </td>
     <td style="text-align:right;"> 0.025 </td>
    </tr>
    <tr>
     <td style="text-align:left;"> Lesion1 </td>
     <td style="text-align:right;"> 0.025 </td>
     <td style="text-align:right;"> 0.028 </td>
    </tr>
  </tbody>
  </table>
  </div>

  </div>
  
  	<div class="6u 12u$(medium)">
  	  <!-- Image -->
  <h3>Validation</h3>

  Some text to describe the validation output

  <span class="image fit"><img src="{% link https://richjjackson.github.io/mecPortal/assets/images/TACE_km1.png %}" alt="" /></span>
  <span class="image fit"><img src="{% link assets/images/pic03.jpg %}" alt="" /></span>
   </div>

   
  </div>


<!------>
<!------>

## Use this model!


Download this model and learn how to use it by visiting 
github/richJJackson/pscLibrary/test_model


<!------>
<!------>
 
## References

Meyer T, Fox R, Ma YT, Ross PJ, James MW, Sturgess R, Stubbs C, Stocken DD, Wall 
L, Watkinson A, Hacking N. Sorafenib in combination with transarterial 
chemoembolisation in patients with unresectable hepatocellular carcinoma (TACE 
2): a randomised placebo-controlled, double-blind, phase 3 trial. The lancet 
Gastroenterology & hepatology. 2017 Aug 1;2(8):565-75.

