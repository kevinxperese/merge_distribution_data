# The Distribution of Household Income, 2014 -- Supplmental Data

The data contained here supplement information provided in CBO's March 2018 
report The Distribution of Household Income, 2014.
www.cbo.gov/publication/53597

## Contents
* README.txt
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

To open the files without read-only access, save the zipped archive to a 
local file directory and extract the files to a new directory.

## General Notes
All data files are in comma-separated values format.
Column headings are in row 1, data start in row 2.

Numbers in the data may not add up to totals because of rounding. Data files 
with dollar values are rounded to the nearest hundred and cells with dollar 
values between -$50 and $50 are empty (missing). Data files with percentages 
are rounded to the nearest tenth and cells with percentage values between -0.05 
percent and 0.05 percent are also empty (missing). Finally, population counts 
less than 0.05 million are also empty (missing). 

All years in the data are calendar years.

Income is adjusted for inflation using the price index for personal consumption
expenditures, which is calculated by the Bureau of Economic Analysis (BEA). 
Those data are updated regularly by BEA. The data used to make the adjustments 
are from the January 26, 2018 revision of the series.

Most files are sorted by three variables: household_type, income_group, and 
year. Only two files are **not** sorted by those variables:
* table_02_income_group_minimums_1979_2014.csv
* table_04_median_household_income_1979_2014.csv

There are four household type values:
* all_households
* hh_with_children (a household with one or more people under age 18)
* elderly_headed_hh (a household with either a head or spouse age 65 or older)
* nonelderly_childless_hh (may have secondary elderly persons living in the 
  household, but no children)

## Income Measures
**Income groups** are created by ranking households by their size-adjusted 
income before taxes and transfers. A household consists of people sharing a 
housing unit, regardless of their relationships. Each income quintile (fifth) 
contains approximately equal numbers of people but slightly different numbers 
of households. Similarly, each percentile (hundredth) contains approximately 
equal numbers of people but different numbers of households. If a household has 
negative income (that is, if its business or investment losses are larger than 
its other income), it is excluded from the lowest income group but included in 
totals.

**Income before transfers and taxes** consists of market income plus social 
insurance benefits.

**Market income** consists of labor income; business income; capital income 
(including capital gains); income received in retirement for past services; and 
other nongovernmental sources of income. (See the appendix for more details.)

**Social insurance benefits** consist of benefits from Social Security (Old Age,
Survivors, and Disability Insurance); Medicare (measured as the average cost to 
the government of providing those benefits); unemployment insurance; and 
workers’ compensation.

**Means-tested transfers** are cash payments and in-kind services provided 
through federal, state, and local government assistance programs. Eligibility 
to receive such transfers is determined primarily on the basis of income, which 
must be below certain thresholds. The largest transfer programs are Medicaid 
and the Children's Health Insurance Program (measured as the average cost to 
the government of providing those benefits); the Supplemental Nutrition 
Assistance Program (formerly known as the Food Stamp program); and 
Supplemental Security Income. (See the appendix for more details.)

**Federal taxes** consist of individual income taxes, payroll taxes, corporate 
income taxes, and excise taxes. In this analysis, taxes for a given year are 
the amount a household owes on the basis of income received that year, 
regardless of when the taxes are paid. Taxes from those four sources accounted 
for 94 percent of federal revenues in fiscal year 2014. The remaining federal 
revenue sources not allocated to U.S. households include states’ deposits for 
unemployment insurance, estate and gift taxes, net income earned by the Federal 
Reserve, customs duties, and miscellaneous fees and fines.

**Average means-tested transfer rates** are calculated as means-tested 
transfers divided by income before transfers and taxes.

**Average federal tax rates** are calculated as federal taxes divided by income 
before transfers and taxes.
