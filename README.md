# Chi square difference testing for Partial Invariance

All code required to run the tests is in the `chi_square_difference_testing.ipynb` file.

## Requirements
Install the following packages via pip/conda.

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
  
- Refer to the `.ipynb` file for an example run.
- Run all cells in the `chi_square_difference_testing.ipynb` file.

## Results
- The results will be stored in two files for each constant factor loading: `results_${input filename}_${fixed loading}` and `summary_${input filename}_${fixed loading}` in the `results` folder.
- The `results_${input filename}_${fixed loading}` file contains individual search results for each scenario.
- The `summary_${input filename}_${fixed loading}` file contains the sum of the results from all scenarios.
