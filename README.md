## Kyomuhangi-and-Giorgi_unified-mechanistic-model
## Title:  A unified and flexible modelling framework for the analysis of malariaserology data

authors:  Irene Kyomuhangi (i.kyomuhangi@lancaster.ac.uk, kyomuhai@gmail.com)  and Emanuele Giorgi, Lancaster University (e.giorgi@lancaster.ac.uk), CHICAS,  Lancaster University 


# Background
This script contains syntax used for the analysis of malaria serology data as described in the paper: "A unified and flexible modelling framework for the analysis of malaria serology data" . Epidemiology & Infection, pages 1-18, 2021" DOI: https://doi.org/10.1017/S0950268821000753
The antibody measurements used in this analysis are PfAMA OD values obtained from ELISA, however the methods are applicable to any malaria antigen type. 

Throughout the script we indicate where the code may need to change depending on the dataset/antibody type under analysis. 
Explanations of the functions and operations used are provided within the syntax itself, and further details of statistical/mathematical principles of this analysis can be found in the paper. 

To request access to the dataset used, please contact Gillian Stresman (Gillian.Stresman@lshtm.ac.uk) or Chris Drakeley (Chris.Drakeley@lshtm.ac.uk) at LSHTM.  


# Packages
This code is run in R. Packages to install: numDeriv, tidyverse, latex2exp, data.table, lme4, stringr, dplyr, mixtools, truncnorm, haven

# Data

Data for this analysis should contain:
1) continuous antibody measurements (eg, OD and MFI). Note that this analysis does not use seropositive/seronegative values
2) age in years

Ensure that your dataset does not contain missing values for either of these variables. 

This code can be extended to include analysis using other variables/covariates and we have indicated where this is possible in the syntax. 

# Flow of the code

The syntax is split into 8 steps which cover: 
1) implementation of the equations in the paper, and 
2) the generation of figures and table in the paper. 

Explanations of the functions and operations used in the sytax are provided, and further details of statistical/mathematical principles of this analysis can be found in the paper. 

The steps are as follows:

STEP 1: DESCRIPTIVE AND EXPLORATIVE ANALYSIS OF THE DATA (FIGURES 1, 4, 5)

STEP 2: FITTING THE UNIFIED MECHANISTIC MODEL (UFM)

STEP 3: GENERATING 95% CIs FOR THE UFM PARAMETER ESTIMATES

STEP 4: FITTING THE EMPIRICAL MODEL (EM)

STEP 5: GENERATING 95% CIs FOR THE EM PARAMETER ESTIMATES

STEP 6: COMPARING THE UFM AND EM (FIGURE 6)

STEP 7: SHOWING HOW LAMBDA OVER TIME IN THE UFM (FIGURE 7)

STEP 8: COMPARING THE UFM AND EM (TABLE 1)
