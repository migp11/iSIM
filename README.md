# I. R code for model building and analysis
The model is included in the files labeled iSIM_desc.tsv, iSIM_met.tsv, and iSIM_react.tsv files. The main_script.R script runs the analyses and produces the figures presented in the manuscript. 

Version: R 3.4.1

# II.	MATLAB code for model building and analysis
Information for installing and running basic functions with the COBRA toolbox18 is available at: https://opencobra.github.io/cobratoolbox/stable/. 

The main_build_model.m MATLAB script builds the base model by adding in the reactions, metabolites, and genes as describes in the manuscript to a variable called model which is then saved. The main_run_analysis.m MATLAB script contains the code to run the analyses and to reproduce the figures in the manuscript. The script first loads the model which was produced in the first script, performs analyses, and generates figures. The script calls the functions coloring.m and ef_tbl_fva.m for the associate analysis and generating figures. 

Versions: MATLAB 2016b, gurobi 7.0.2, COBRA toolbox 3.0

# III.	Python code for model building and analysis
Information for installing and running basic functions with the COBRApy package19 is available at: https://github.com/opencobra/cobrapy. 

The SMBL_iSIM_createModel.py script generates a metabolic model and saves it as an .xml file later use. You must run this script first to generate the model, which is then loaded and analyzed using the following script. The FigureCreationScript.py contains the code to run the analyses and reproduce the figures produced in the manuscript. 

Versions: Python 3.6.7, gurobi 8.1.0, Cobrapy 0.11.3
