COMPARTMENTAL MODEL (SCRIPTS)

This repository outlines the compartmental model designed to simulate the transmission of C. difficile in healthcare environments. It elaborates on both the structure of the model and the analyses performed, utilizing RStudio and MATLAB for our simulations and analyses. 

Results of the model are included in the manuscript entitled: Assessing the impact of asymptomatic carriers and infection control interventions on healthcare-associated C. difficile transmission: a compartmental model approach.

1. COMPARTMENTAL MODEL STRUCTURE

1.1 MODEL STRUCTURE AND PARAMETERS DEFINITION: The model's structure is described, and the parameters of interest used in the simulations are defined.

1.2 MODEL CALIBRATION AND TRANSMISSION RATE (DELTA) OPTIMIZATION: The transmission rate (delta parameter) was optimized to calibrate the model with the Clostridioides difficile infection (CDI) incidence in our institution.


2. REPRODUCTION NUMBER ANALYSES
   
2.1 MONTE CARLO SIMULATIONS: we used the function estimated by the next-generation matrix (refer to script 4. MATLAB - REPRODUCTION NUMBER ANALYSES) to conduct Monte Carlo simulations with 1000 values derived through random selection from parameter distributions. Mean and parameter distributions are detailed in Table 1, "Description of Input Parameters and Values Used in Estimations" (main body of manuscript). The distribution of the reproduction number was estimated and visualized.
   
2.2 PARTIAL RANK CORRELATION COEFFICIENTS (PRCC): the relationship between the input values of the parameters and R0 estimates from the Monte Carlo simulations was assessed. Scatterplots were created to compare the basic reproduction number with each parameter.
 
2.3 LOCAL SENSITIVITY ANALYSIS: a sensitivity analysis was conducted using fixed-point estimations to evaluate the influence of parameters on the R0 estimate, using the partial derivative of the reproduction number as a function of each parameter. Normalized indices were presented to depict the impact of parameter variations. These indices were calculated by determining the relative change ratio in each parameter to the relative change in the R0 estimate. Indices were estimated in MATLAB (see script 4. MATLAB - REPRODUCTION NUMBER ANALYSES), and the results were visually represented in this section of the script.
 
2.4 EXTENDED SENSITIVITY ANALYSIS (REPRODUCTION NUMBER): the impact on the reproduction number of varying each parameter within a percentage change range, while keeping all other parameters constant, was calculated.

2.5 EXTENDED SENSITIVITY ANALYSIS OF TREATMENT AND ISOLATION ON ASYMPTOMATIC CARRIERS: the impact of varying parameters related to the implementation of contact precautions (parameters f_2 and gamma_2) and treatment (parameters j and sigma_2) on the reproduction number estimate was calculated. Changes in both parameters were depicted in contour graphs to visualize the impact of both rates and the effectiveness of interventions.
   


3. CDI INCIDENCE ANALYSIS

3.1 MODEL STRUCTURE AND PARAMETER VALUES: similar to script 1. COMPARTMENTAL MODEL STRUCTURE.

3.2 EXTENDED SENSITIVITY ANALYSIS (INCIDENCE): The impact on CDI incidence of varying each parameter within a percentage change range, while keeping all other parameters constant, was calculated. CDI incidence was estimated as the number of cases per 1000 admissions.


3.3 EXTENDED SENSITIVITY ANALYSIS OF TREATMENT AND ISOLATION ON ASYMPTOMATIC CARRIERS: the impact of varying parameters related to the implementation of contact precautions (parameters f_2 and gamma_2) and treatment (parameters j and sigma_2) on the CDI incidence was calculated. Changes in both parameters were depicted in contour graphs to illustrate the impact of both rates and the effectiveness of interventions.


