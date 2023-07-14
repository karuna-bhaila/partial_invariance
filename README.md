# Chi square difference testing for Partial Invariance

All code required to run the tests is in the `chi_square_difference_testing.ipynb` file.

## Requirements
- The code is in python notebook format. Use jupyter notebook to run.
- Install the following packages via pip/conda.

        numpy==1.21.5
        pandas==1.4.2

## Test Data
- Place your file containing chi-square values of all factor loadings in the `data` folder.
- Column names should be in the format `chi${factor loading}`; for example: `chi12345`.
- A row should contain chi-square values for all factor loadings for a simulation.

## Run
- The code requires the following input from the user:

| Variable         | Description |
| ---------------- | ----------- |
| input_file       | Name of the input file containing chi-square values       |
| num_factors      | Number of factors        |
| fixed_loading    | String indicating the factor that is always constrained           |
| thr              | Threshold value for difference testing (3.8415) |
  
- Run all cells in the `chi_square_difference_testing.ipynb` file as is to implement tests for the `L2355merged.csv` file.
- Change the variables above to run tests on your data.

## Results
- The results will be stored in two files for each constant factor loading: `${input filename}_${fixed loading}_results` and `${input filename}_${fixed loading}_summary` in the `results` folder.
- The `${input filename}_${fixed loading}_results` file contains individual search results for each simulation.
- The `${input filename}_${fixed loading}_summary` file contains the sum of the results from all simulations.
