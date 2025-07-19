# $L4.1:$ Association between two variables - Review of course

## Review 

- What is statistics?
  - Descriptive statistics, inferential statistics.
- Understad how data are collected.
  - Identify variables and cases (observations) in a data set
- Types of data
  - Classify data as categorical or numerical data.
  - Measurement scales -- nominal, ordinal, interval, and ratio.
- Describing categorical data
  - Creating frequency tables, understanding relative frequency
  - Creating pie charts and bar charts
  - Descriptive measures of Mode and Median
- Describing numerical data
  - Creating frequency tables: single valued and grouped data.
  - Measures of central tendency: Mean, Median and Mode
  - Measures of dispertion: Range, Varience, Standard deviation
  - Persentiles, Quartiles, Interquartile range.

# $L4.2:$ Association between two categorical variables - Introduction

## Learning objective

- Use of two-way contigency tables to understand association between two categorical variables.
- Understand association between numrical variables through scatter plots; compute and interpret correlation.
- Understand relationship between a categorical and numerical variable.


## Introduction

- To understand the association between two categorical variables.
- Learn how to two-way contingency table.
- Learn concept of relative row/column frequencies and how to use them to determine whether there is an association between the categorical variables.

### $Example\ 1:$ Gender versus use of smartphone

- A market research firm is interested in finding out whether ownership of a smartphone is associated with gender of a student. In other words, they want to find out whether more females own a smartphone while compared to males, or whether owning a smartphone is independent of gender.
- To answer this question, a group of 100 college going children were surveyed about whether they owned a smart phone or not.
- The categorical variables in this example are
  - Gender: Male, Female (2 Categories)- Nominal variable
  - Own a smartphone: Yes, No (2 Categories)- Nominal varible.

#### $Example\ 1:$ Gender versus use of smartphone - Summarize data

- We have the following summery statistics 
  - There are 44 female and 56 male students
  - 76 students owned a smartphone, 24 did not.
  - 34 female students owned a smartphone 42 male students owned a smartphone.
- The data given in the example can be organized using a two-way table, reffered to as a contingency table.

<center><table><tr><td></td><td></td><td colspan=2>Own a smartphone</td><td></td></tr>
<tr><td></td><td></td><td>No</td><td>Yes</td><td>Row total</td></tr>
<tr><td rowspan=3>Gender</td></tr>
<tr><td>Female</td><td>10</td><td>34</td><td>44</td></tr>
<tr><td>Male</td><td>14</td><td>42</td><td>56</td></tr>
<tr><td></td><td>Coumn total</td><td>24</td><td>76</td><td>100</td></tr></table></center>

## Contingency table using google sheets

- $Step\ 1 :$ Choose the columns of the variables for which you seek an association.
- $Step\ 2 :$ Go to Data-click on Pivot table option
- $Step\ 3 :$ Click on create option in the pivot table- it will open the pivot table editor:
  - $3.1:$ Under the Rows tab, click on the first categorical variable.
  - $3.2:$ Under the columns tab, click on the second categorical variable.
  - $3.3:$ Under the values tab, click on either of the variables and then click on the COUNTA tab under "summarize by" tab.

### $Example\ 2:$ Income versus the use of smartphone

- A market research firm is interested in finding out whether ownership of a smartphone is associated with income of an individual. In other words, they want to find out whether income is associated with ownership of a smartphone.
- To answer this question, a group of 100 randomly picked individuals were surveyed about whether they owned a smart phone or not.
  - The categorical variables in this example are
  - Income: Low, Medium, High (3 categories) - Ordinal variable
  - Own a smartphone: Yes, No (2) categories) - Nominal variable

#### $Example\ 2:$ Income versus the use of smartphone - Summarize data

- We have the following summary statistics
  - There are 20 High income, 66 medium income, and 14 low income participants.
  - 62 participants owned a smartphone, 38 did not own.
  - 18 High income participants owned a smartphone, 39 Medium income participants owned a smartphone, and 5 Low income participants owned a smartphone.
- The contingency table corresponding to the data is given below.

<center><table><tr><td></td><td></td><td colspan=2>Own a smartphone</td><td></td></tr>
<tr><td></td><td></td><td>No</td><td>Yes</td><td>Row total</td></tr>
<tr><td rowspan=4>Income level</td></tr>
<tr><td>High</td><td>2</td><td>18</td><td>20</td></tr>
<tr><td>Medium</td><td>27</td><td>39</td><td>66</td></tr>
<tr><td>Low</td><td>9</td><td>5</td><td>14</td></tr>
<tr><td></td><td>Coumn total</td><td>38</td><td>62</td><td>100</td></tr></table></center>

## Section summary

- Organize bivariate categorical data into a two-way table - contingency table.
- If data is ordinal, maintain order of the varible in the table.

# $L4.3:$ Association between two categorical variable - Relative frequences

## Row relative frequencies

- $Defination:$ Divide each cell frequency in a row by its row total
- $Example:$ 
  - What proportion of total participents own a smartphone?
  - What proportion of female particepents own a smartphone?

<center><table><tr><td></td><td></td><td colspan=2>Own a smartphone</td><td></td></tr>
<tr><td></td><td></td><td>No</td><td>Yes</td><td>Row total</td></tr>
<tr><td rowspan=3>Gender</td></tr>
<tr><td>Female</td><td>10/44</td><td>34/44</td><td>44</td></tr>
<tr><td>Male</td><td>14/56</td><td>42/56</td><td>56</td></tr>
<tr><td></td><td>Coumn total</td><td>24/100</td><td>76/100</td><td>100</td></tr></table></center>

- Which is

<center><table><tr><td></td><td></td><td colspan=2>Own a smartphone</td><td></td></tr>
<tr><td></td><td></td><td>No</td><td>Yes</td><td>Row total</td></tr>
<tr><td rowspan=3>Gender</td></tr>
<tr><td>Female</td><td>23.73%</td><td>77.27%</td><td>44</td></tr>
<tr><td>Male</td><td>25.00%</td><td>75.00%</td><td>56</td></tr>
<tr><td></td><td>Coumn total</td><td>24.00%</td><td>76.00%</td><td>100</td></tr></table></center>

## Column relative frequencies

- $Defination:$ Divide each cell frequency in a row by its column total
- $Example:$ 
  - What proportion of total participents are female?
  - What proportion of smartphone owners particepents female?

<center><table><tr><td></td><td></td><td colspan=2>Own a smartphone</td><td></td></tr>
<tr><td></td><td></td><td>No</td><td>Yes</td><td>Row total</td></tr>
<tr><td rowspan=3>Gender</td></tr>
<tr><td>Female</td><td>10/24</td><td>34/76</td><td>44/100</td></tr>
<tr><td>Male</td><td>14/24</td><td>42/76</td><td>56/100</td></tr>
<tr><td></td><td>Coumn total</td><td>24</td><td>76</td><td>100</td></tr></table></center>

- Which is

<center><table><tr><td></td><td></td><td colspan=2>Own a smartphone</td><td></td></tr>
<tr><td></td><td></td><td>No</td><td>Yes</td><td>Row total</td></tr>
<tr><td rowspan=3>Gender</td></tr>
<tr><td>Female</td><td>41.67%</td><td>44.74%</td><td>44%</td></tr>
<tr><td>Male</td><td>58.33%</td><td>55.26%%</td><td>56%</td></tr>
<tr><td></td><td>Coumn total</td><td>24</td><td>76</td><td>100</td></tr></table></center>

## Section summery 

- Concept of relative frequency: row relative frequency and column relative frequency

## Association between two variables

- What do we mean by stating two variables are associated?
  - Knowing information about one variable provides information about the other variable.
- To determine if two categorical variables are associated, we use the notion of relative row frequencies and relative colunb frequencies described earlier.

- If the row relative frequencies( the column relative frequencies) are the same for all rows( columns) then we say that the two variables are not associated with each other.
- If the row relative frequencies( the column relative frequencies) are the different for some rows( columns) then we say that the two variables are associated with each other.

<center><table><tr><td></td><td></td><td colspan=2>Own a smartphone</td><td></td></tr>
<tr><td></td><td></td><td>No</td><td>Yes</td><td>Row total</td></tr>
<tr><td rowspan=3>Gender</td></tr>
<tr><td>Female</td><td>23.73%</td><td>77.27%</td><td>44</td></tr>
<tr><td>Male</td><td>25.00%</td><td>75.00%</td><td>56</td></tr>
<tr><td></td><td>Coumn total</td><td>24.00%</td><td>76.00%</td><td>100</td></tr></table></center>

<center><table><tr><td></td><td></td><td colspan=2>Own a smartphone</td><td></td></tr>
<tr><td></td><td></td><td>No</td><td>Yes</td><td>Row total</td></tr>
<tr><td rowspan=3>Gender</td></tr>
<tr><td>Female</td><td>41.67%</td><td>44.74%</td><td>44%</td></tr>
<tr><td>Male</td><td>58.33%</td><td>55.26%%</td><td>56%</td></tr>
<tr><td></td><td>Coumn total</td><td>24</td><td>76</td><td>100</td></tr></table></center>

### Gender and smart phone are not associated with each other
