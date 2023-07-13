# Chi square difference testing for Partial Invariance

All code required to run the tests is in the `chi_square_difference_testing.ipynb` file.

## Requirements
Install the following packages via pip/conda.
    numpy==1.21.5
    pandas==1.4.2

## Test Data
Place your file containing chi-square values of all factor loadings in the `data` folder. Column names should be in the format `chi<factor loading>`; for example: `chi12345`. Each row should contain chi-square values for all factor loadings for one simulation.

## Run
The code requires the following input from the user:
    input_file: name of the input file containing chi-square values
    num_factors = number of factors
    fixed_loading = string indicating the factor that is always constrained
    thr = threshold value for difference testing (3.8415)
Refer to the `ipynb` file for an example run.
Run all cells in the `chi_square_difference_testing.ipynb` file.

## Results
The results will be stored in two files for each constant factor loading: `results_<*fixed loading*>_<*input filename*>` and `summary_<*fixed loading*>_<*input filename*>` in the `results` folder.
The `results_<*fixed loading*>_<*input filename*>` file contains individual search results for each scenario, and the `summary_<*fixed loading*>_<*input filename*>` file contains the sum of the results from all scenarios.
