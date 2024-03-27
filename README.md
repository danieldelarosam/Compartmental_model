Compartmental_model

Compartmental model for C. difficile transmission in the healthcare setting. We used Rstudio and Matlab to perform analyses, packages used are included in the scripts following the next order:


1. COMPARTMENTAL MODEL STRUCTURE

1.1 MODEL STRUCTURE AND PARAMETERS DEFINITION: we describe the model structure and values for the parameter of interest used for simulation 

1.2 MODEL CALIBRATION AND TRANSMISSION RATE (DELTA) OPTIMIZATION: we optimized the transmission rate (delta parameter) to calibrate the model with the CDI incidence in our institution



2. REPRODUCTION NUMBER ANALYSES
   
2.1 MONTE CARLO SIMULATIONS: we use the function estimate by next-generation matrix (see script 4. Matlab - Reproduction number analyses) to run Montecarlo simulation with 1000 values
   obtained by random selection of parameter distributions. Mean and parameter distributions are found in Table 1. Description of input parameters and values used in estimations (main body of manuscript)
   We estimated and visualized the reproduction number distribution.
   
2.2 PARTIAL RANK CORRELATION COEFFICIENTS: we performed a partial rank correlation analysis to assess the relationship between the input values of the parameters and R0 estimates resulting from the 
   Montecarlo simulations analysis. Scatterplots were generated to compare the basic reproduction number with each parameter.

2.3 LOCAL SENSITIVITY ANALYSIS: sensitivity analysis using fixed point estimations to assess the influence of parameters on R0 estimation, using the partial derivative of the reproduction number as a
   function of each parameter. We presented normalized indices to illustrate the impact of parameter variations. These indices were determined by calculating the relative change ratio in each parameter of 
   interest to the relative change in R0 estimation. Indices were estimated in Matlab (see script 4. Matlab - Reproduction number analyses) and index results were used to generate a graphical representation 
   in this part of the script.
 
2.4 EXTENDED SENSITIVITY ANALYSIS (REPRODUCTION NUMBER): We calculated the impact (on the reproduction number) of varying each parameter within a percentage change range while keeping all other parameters      constant 

2.5 EXTENDED SENSITIVITY ANALYSIS OF TREATMENT AND ISOLATION ON ASYMPTOMATIC CARRIERS: we calculated the impact of varying parameters related to the contact precaution implementation (parameter f_2 and         gamma_2) and treatment (parameter j and sigma_2) on the reproduction number estimation. The changes in both parameters were represented in contour graphs to visualize the effect of both rates and the        effectiveness of interventions. 
   


3. CDI INCIDENCE ANALYSIS

3.1 MODEL STRUCTURE AND PARAMETER VALUES: similar to script 1. COMPARTMENTAL MODEL STRUCTURE.

3.2 EXTENDED SENSITIVITY ANALYSIS (INCIDENCE):  We calculated the impact (on the CDI incidence) of varying each parameter within a percentage change range while keeping all other parameters constant. CID   
    incidence was estimated as number of cases per 1000 admissions. 

3.3 EXTENDED SENSITIVITY ANALYSIS OF TREATMENT AND ISOLATION ON ASYMPTOMATIC CARRIERS:  we calculated the impact of varying parameters related to the contact precaution implementation (parameter f_2 and 
    gamma_2) and treatment (parameter j and sigma_2) on the CDI incidence. The changes in both parameters were represented in contour graphs to visualize the effect of both rates and the effectiveness of 
    interventions. 
