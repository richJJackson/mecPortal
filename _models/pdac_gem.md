---
layout: model
title: Gemcitabine OS
image: assets/images/hcc.jpg
area: PDAC
description:  A model to describe overall survival in patietns with aHCC
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
Data were taken from the European Study group for PAncreatic Cancer (ESPAC) 3 
Study - A randomised phase III study to investigate the role of chemotherapy in 
patients following surgery for Pancreatic Ductal Adenocarcinoma.  Patient were
randomised post surgery.  Patients were recruited from 159 pancreatic cancer 
centers in Europe, Australasia, Japan, and Canada
</p>

<h2> Estimand </h2>
<div class="box">
  <div class="row">
  	
  	<div class="6u 12u$(medium)">
  	  <div class="box">
    		<h3> Patients </h3>
    		<p> Patients were eligible if they had undergone complete macroscopic (R0 
    		or R1) resection for ductal adenocarcinoma of the pancreas with 
    		histological confirmation and with no evidence of malignant ascites, 
    		peritoneal metastasis, or spread to the liver or other distant abdominal 
    		or extra-abdominal organs. Patients had to be fully recovered from the 
    		operation, with a World Health Organization performance score of 2 or 
    		lower and a life expectancy of more than 3 months. Patients with previous 
    		use of neoadjuvant chemotherapy or other concomitant chemotherapy and with 
    		pancreatic lymphoma, macroscopically remaining tumor (R2 resection), or 
    		TNM stage IVb disease were excluded. </p>
    	</div>	
  	</div>
  	
  	<div class="3u 12u$(medium)">
  		<div class="box">
  		<h3> Intervention </h3>
  		<p> Patients received gemcitabine as 1000 mg/m2 intravenous infusion once a 
  		week for 3 of every 4 weeks for up to 6 months </p>
  		</div>	
  	</div>
  	
  	<div class="3u$ 12u$(medium)">
  		<div class="box">
  		<h3> Outcome </h3>
  		<p> The Outcome is Overall Survival measured as the point from randomisation 
  		until death by any cause </p>
  		</div>	
  	</div>

  		<h3> Inter-current Events </h3>
  		<p> The chosen estimand for analysis follows the Treatment Policy approach, ignoring 
      any intercurrent events or termination of therapies as is suitable for evaluating 
      patients at the point of treatment choice.   Lastly, as a key prognositc 
      indicator, only patients with a basleine measure of CA19.9 were retained in the 
      model.</p>

  </div>
</div>



<!------------------------>
<!------------------------>
<!-- Data -->
<!------------------------>
<!------------------------>


<h2 id="data">Data</h2>

<p> Data considered for inclusion in the model were observed from the baseline
case report forms of the ESPAC-3 study and included T stage, N stage, Resection
Margin Status, Local Invasion, WHO status, Tumor Grade (Differentiation), Tumour
Size, pre-operative CA19.9 and post-operative CA19.9</p>

<div class="row 200%">
	
	<div class="6u 12u$(medium)">

  <!-- Table -->
		<h4>Covariates</h4>
      <div class="table-wrapper">
      <table>
       <thead>
        <tr>
         <th style="text-align:left;"> Covariate </th>
         <th style="text-align:left;"> Level </th>
         <th style="text-align:left;"> All Pts. </th>
        </tr>
       </thead>
      <tbody>
        <tr>
         <td style="text-align:left;"> Total </td>
         <td style="text-align:left;">  </td>
         <td style="text-align:left;"> 359 </td>
        </tr>
        <tr>
         <td style="text-align:left;"> T Stage </td>
         <td style="text-align:left;"> 2 </td>
         <td style="text-align:left;"> 27 (100%) </td>
        </tr>
        <tr>
         <td style="text-align:left;"> T Stage </td>
         <td style="text-align:left;"> 3 </td>
         <td style="text-align:left;"> 78 (100%) </td>
        </tr>
        <tr>
         <td style="text-align:left;"> T Stage </td>
         <td style="text-align:left;"> 4 </td>
         <td style="text-align:left;"> 254 (100%) </td>
        </tr>
        <tr>
         <td style="text-align:left;"> Tumor Grade </td>
         <td style="text-align:left;"> 1 </td>
         <td style="text-align:left;"> 53 (100%) </td>
        </tr>
        <tr>
         <td style="text-align:left;"> Tumor Grade </td>
         <td style="text-align:left;"> 2 </td>
         <td style="text-align:left;"> 223 (100%) </td>
        </tr>
        <tr>
         <td style="text-align:left;"> Tumor Grade </td>
         <td style="text-align:left;"> 3 </td>
         <td style="text-align:left;"> 83 (100%) </td>
        </tr>
        <tr>
         <td style="text-align:left;"> Lymph Node </td>
         <td style="text-align:left;"> 1 </td>
         <td style="text-align:left;"> 105 (100%) </td>
        </tr>
        <tr>
         <td style="text-align:left;"> Lymph Node </td>
         <td style="text-align:left;"> 2 </td>
         <td style="text-align:left;"> 254 (100%) </td>
        </tr>
        <tr>
         <td style="text-align:left;"> (log) CA19.9 </td>
         <td style="text-align:left;"> median (IQR) </td>
         <td style="text-align:left;"> 3.332 (2.398, 4.256) </td>
        </tr>
      </tbody>
      </table>
            
      
      </div>
  
  <!-- End Table -->
  
  </div>
  
  <div class="6u 12u$(medium)">
    <!-- Image -->
    <h3>Model covariates</h3>
    Details of the covariates used to generate the model are:
    <span class="image fit"><img src="{% link assets/images/e3_data.png %}" alt="" /></span>
    </div>
     <!-- End Image -->
  </div>

</div>





<!------------------------>
<!------------------------>
<!-- Model -->
<!------------------------>
<!------------------------>


<div class="box">
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
      <span class="image fit"><img src="{% link assets/images/e3_gem_fpm.png %}" alt="" /></span>
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
   <th style="text-align:left;">   </th>
   <th style="text-align:left;"> Est (se) </th>
   <th style="text-align:left;"> HR (95% CI) </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> gamma0 </td>
   <td style="text-align:left;"> -10.18 (1.08) </td>
   <td style="text-align:left;"> 0 (0 - 0) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> gamma1 </td>
   <td style="text-align:left;"> 2.89 (0.52) </td>
   <td style="text-align:left;"> 17.94 (6.51 - 49.43) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> gamma2 </td>
   <td style="text-align:left;"> 0.33 (0.49) </td>
   <td style="text-align:left;"> 1.39 (0.54 - 3.6) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> gamma3 </td>
   <td style="text-align:left;"> -0.58 (0.8) </td>
   <td style="text-align:left;"> 0.56 (0.12 - 2.66) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> gamma4 </td>
   <td style="text-align:left;"> 0.55 (0.43) </td>
   <td style="text-align:left;"> 1.74 (0.74 - 4.07) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> t3 </td>
   <td style="text-align:left;"> 0.56 (0.27) </td>
   <td style="text-align:left;"> 1.75 (1.04 - 2.95) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> t4 </td>
   <td style="text-align:left;"> 0.42 (0.25) </td>
   <td style="text-align:left;"> 1.52 (0.94 - 2.46) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> grade2 </td>
   <td style="text-align:left;"> 0.41 (0.18) </td>
   <td style="text-align:left;"> 1.51 (1.07 - 2.13) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> grade3 </td>
   <td style="text-align:left;"> 0.73 (0.2) </td>
   <td style="text-align:left;"> 2.08 (1.41 - 3.07) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> nodes2 </td>
   <td style="text-align:left;"> 0.49 (0.14) </td>
   <td style="text-align:left;"> 1.63 (1.24 - 2.13) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> lca199 </td>
   <td style="text-align:left;"> 0.21 (0.04) </td>
   <td style="text-align:left;"> 1.23 (1.14 - 1.33) </td>
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
  
</div>


</div>

<!------------------------>
<!------------------------>
<!-- Validation -->
<!------------------------>
<!------------------------>

<div class="box">

<h1 id="valid"> Validation </h1>

<p> Details on the validation of the model: </p>


<h3> Validation Details </h3>
<div class="box">
	<p> Provide some information on how the model is validated </p>
</div>


<div class="row 200%">

	<div class="6u 12u$(medium)">

  <h4>Calibration </h4>
  
    <div class="table-wrapper">
  
  <table>
 <thead>
  <tr>
   <th style="text-align:left;">   </th>
   <th style="text-align:left;"> est (se) </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> C-Statistic </td>
   <td style="text-align:left;"> 0.63 (0.017) </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Slope </td>
   <td style="text-align:left;"> 0.996 (0.125) </td>
  </tr>
</tbody>
</table>
  </div>

<h4>Discrimination</h4>
 
  <div class="table-wrapper">
    <table>
     <thead>
      <tr>
       <th style="text-align:left;">   </th>
       <th style="text-align:left;"> est (se) </th>
       <th style="text-align:left;"> HR (95% CI) </th>
      </tr>
     </thead>
    <tbody>
      <tr>
       <td style="text-align:left;"> Risk Group 1 </td>
       <td style="text-align:left;">  </td>
       <td style="text-align:left;">  </td>
      </tr>
      <tr>
       <td style="text-align:left;"> Risk Group 2 </td>
       <td style="text-align:left;"> 0.532 (0.194) </td>
       <td style="text-align:left;"> 1.702 (1.163, 2.492) </td>
      </tr>
      <tr>
       <td style="text-align:left;"> Risk Group 3 </td>
       <td style="text-align:left;"> 1.002 (0.194) </td>
       <td style="text-align:left;"> 2.724 (1.864, 3.982) </td>
      </tr>
      <tr>
       <td style="text-align:left;"> Risk Group 4 </td>
       <td style="text-align:left;"> 1.628 (0.223) </td>
       <td style="text-align:left;"> 5.094 (3.292, 7.887) </td>
      </tr>
    </tbody>
    </table>
   

  </div>

  </div>
  
  	<div class="6u 12u$(medium)">
  	  <!-- Image -->

  Some text to describe the validation output

  <span class="image fit"><img src="{% link assets/images/e3_gem_discr.png %}" alt="" /></span>


   </div>

  </div>

</div>



<!------------------------>
<!------------------------>

<div class="box">

<h1 id="valid"> Use this model </h1>


Download this model and learn how to use it by visiting 
github/richJJackson/pscLibrary/test_model

</div>

<!------------------------>
<!------------------------>

 <div class="box">
<h1 id="valid"> References </h1>

Details on the trial which provided the data for this model can be found at:

Neoptolemos JP, Stocken DD, Bassi C, et al. Adjuvant Chemotherapy With 
Fluorouracil Plus Folinic Acid vs Gemcitabine Following Pancreatic Cancer 
Resection: A Randomized Controlled Trial. JAMA. 2010;304(10):1073–1081. 
doi:10.1001/jama.2010.1275
</div>
