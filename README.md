# Merge Ddistribution Data

The Jupyter notebook in this  repo reads all the Supplemental Data ([https://www.cbo.gov/system/files/115th-congress-2017-2018/reports/53597-supplementaldata-zipped.zip](https://www.cbo.gov/system/files/115th-congress-2017-2018/reports/53597-supplementaldata-zipped.zip)) from CBO's [Distribution of Household Income, 2014](https://www.cbo.gov/publication/53597) report, and combines them into a single rectangular file.

## Input Data
The code downloads and unzips the data into the `input_data` directory.

The csv files in the zipped file that get processed are:

	* table_01_demographics_1979_2014.csv  
	* table_02_income_group_minimums_1979_2014.csv  
	* table_03_average_household_income_1979_2014.csv  
	* table_04_median_household_income_1979_2014.csv  
	* table_05_components_inc_before_transfers_taxes_1979_2014.csv  
	* table_06_components_means_tested_transfers_1979_2014.csv  
	* table_07_components_federal_taxes_1979_2014.csv  
	* table_08_means_tested_transfer_rates_1979_2014.csv  
	* table_09_federal_tax_rates_1979_2014.csv  
	* table_10_household_income_shares_1979_2014.csv  
	* table_11_means_tested_transfer_shares_1979_2014.csv  
	* table_12_federal_tax_shares_1979_2014.csv  

### Easy Files
First, all the "easy" files are processed and merged together.

(An "easy" file has the same file format with records ranked by 'household_type', 'income_group', and 'year')

### Hard Files
There are two 'hard' files that needed some cleaning up before merging:
	* table_02_income_group_minimums_1979_2014.csv  
	* table_04_median_household_income_1979_2014.csv  

## Medians
The medians file is easier, and gets delt with first.

Medians are merged on only for records where ['household_type' == 'all_households'] and ['income_group' == 'all_quintiles'].

All other records have empty (missing) values.

## Minimums
The minimums data file needed some more wrangling before it could be merged.

The minimums data contain 'income_group' minimums for four household sizes (1 through 4).
The minimums data are merged on to the 

## Output Data
In the `output_data` directory is a single file: `distribution_data_2014.csv`.

It contains 1440 rows and 70 columns
