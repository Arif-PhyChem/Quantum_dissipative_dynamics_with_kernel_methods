## Speeding up quantum dissipative dynamics of open systems with kernel methods
## New J. Phys. 23 (2021) 113019, https://doi.org/10.1088/1367-2630/ac3261

Prerequisite steps for ML-dynamics with the KRR model

1) The training data has already been provided, however you can run HEOM.py to generate trajectories with HEOM method. 
   For that, you need Qutip package https://qutip.org/
 
2) Download MLatom from http://mlatom.com/ and install it following the instructions on this website

3) Download the training and test data given in the repository

4) Each file from training and test data consists of 4 columns. They respectively are time, state-1 population,  
     state-2 population and population difference. We are training KRR model for population difference only.  

4) Prepare your input data files (the ready-made input data files (prepared_input_files.zip) are already provided)

5) Prepare your input file for MLatom following mlatom.inp

6) We have already provided the ready-made trained models; trained_sym_model (for symmetric case）and 
     trained_asym_model (for asymmetric case)however you can still train ML by running "mlatom mlatom.inp > output"

7) using run_ML_dynamaics.bash, you can run ML dynamics
