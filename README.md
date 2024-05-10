COMPARTMENTAL MODEL (SCRIPTS)

This repository outlines the compartmental model designed to simulate the transmission of C. difficile in healthcare environments. It elaborates on both the structure of the model and the analyses performed, utilizing RStudio and MATLAB for our simulations and analyses. 

Model results are included in the manuscript entitled: Assessing the impact of asymptomatic carriers and infection control interventions on healthcare-associated C. difficile transmission: a compartmental model approach.

1. COMPARTMENTAL MODEL STRUCTURE

1.1 MODEL STRUCTURE AND PARAMETERS DEFINITION: The model's structure is described, and the parameters of interest used in the simulations are defined.

1.2 TRANSMISSION RATE (DELTA) OPTIMIZATION: The transmission rate (delta parameter) was optimized to calibrate the model with the Clostridioides difficile infection (CDI) cases observed in our institution.

1.3 SIMULATIONS: Simulations using random parameter values with optimized delta parameter

#1.4 ESTIMATION OF REPRODUCTION NUMBER OF SIMULATION: Estimation of the reproduction number for simulation in section 1.3. R0 formula is derived from Matlab 1: Reproduction number function

2. GLOBAL SENSITIVITY ANALYSIS

2.1 GLOBAL SENSITIVITY ANALYSIS: REPRODUCTION NUMBER: We estimate R0 function using 1000 randoms  values for each parameter to subsequently perform partial rank correlation coefficients

2.2 PARTIAL RANK CORRELATION COEFFICIENTS (PRCC): REPRODUCTION NUMBER:  relationship between the input values of the parameters and R0 estimates from prior simulations was assessed. Scatterplots were created to compare the basic reproduction number with each parameter.

3. GLOBAL SENSITIVITY ANALYSIS
 
3.1 LOCAL SENSITIVITY ANALYSIS: a sensitivity analysis was conducted using fixed-point estimations to evaluate the influence of parameters on the R0 estimate, using the partial derivative of the reproduction number as a function of each parameter. Normalized indices were presented to depict the impact of parameter variations. These indices were calculated by determining the relative change ratio in each parameter to the relative change in the R0 estimate. Indices were estimated in MATLAB (see script Matlab 2: Sensitive index), and results were visually represented in this section of the script.

4. EXTENDED SENSITIVITY ANALYSES
 
4.1 EXTENDED SENSITIVITY ANALYSIS (REPRODUCTION NUMBER): the impact on the reproduction number of varying each parameter within a percentage change range, while keeping all other parameters constant, was calculated.

4.2 EXTENDED SENSITIVITY ANALYSIS OF TREATMENT AND ISOLATION ON ASYMPTOMATIC CARRIERS: the impact of varying parameters related to the implementation of contact precautions (parameters f_2 and gamma_2) and treatment (parameters j and sigma_2) on the reproduction number estimate was calculated. Changes in both parameters were depicted in contour graphs to visualize the impact of both rates and the effectiveness of interventions.
   
4.3 EXTENDED SENSITIVITY ANALYSIS (INCIDENCE): The impact on CDI incidence of varying each parameter within a percentage change range, while keeping all other parameters constant, was calculated. CDI incidence was estimated as the number of cases per 1000 admissions.

4.4 EXTENDED SENSITIVITY ANALYSIS OF TREATMENT AND ISOLATION ON ASYMPTOMATIC CARRIERS: the impact of varying parameters related to the implementation of contact precautions (parameters f_2 and gamma_2) and treatment (parameters j and sigma_2) on the CDI incidence was calculated. Changes in both parameters were depicted in contour graphs to illustrate the impact of both rates and the effectiveness of interventions.


