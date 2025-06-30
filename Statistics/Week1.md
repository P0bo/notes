# Introduction and type of data :Basic Definitions

## What is Statistics

- $Definition:$ Statistics is the art of learning from data. It is concerned with the collection of data, their subsequent description and their analysis, which often leads to the drawing of conclusions.

### Major Branches of Statistics

- Descriptive statistics
  - $Definition:$ The part of statistics concerned with the description and summarization of data.
- Inferential Statistics
  - $Definition:$ The part of statistics concerned with the drawing of conclusions from the data.
    - To be able to draw a conclusions from the data, we must take into account the possibility of chance $\to$ introduction to probability.
### Population and Sample

- Population
  - $Definition:$ The total collection of all the elements that we are interested in.
- Sample
  - $Definition:$ A subgroup of Population that will be studied in detail.

## The purpose of statistical analysis

- If the purpose of the analysis is to examine and explore information for its own intrinsic interest only, the study is called descriptive.
  - A descriptive study may be performed either on a sample or a population.
- If the information is obtained from a sample of a population and the purpose of the study is to use that information to draw conclusions about the population, the study is inferential.
  - When an inference is made about the population, based on information obtained from the sample, does the study become inferential.

# Introduction and type of data : Understanding data

## What is Data

- $Definition:$ Data are facts and figures collected, analyzed, and summarized for the presentation and interpretation.
  - Statistics relies on data, information that is all around us.

## Data Collection

### Why Do we collect data

In order to learn something, we need to collect data.
- Interested in the characteristics of some groups of people, places, things, or events.
 - $Examples:$
   - To know about temperatures in a particular month in Chennai, India.
   - To know about the marks obtained by students in their class 12th.
   - To know how many people like a new song/ product/ video -- collected through comments.

### Data available: published data.
### Data not available: generate data.
<center> 

```
We assume data is available and our objective is to do a statistical analysis of available data.

``` 
</center>

## Structured and Unstructured data

- For the information in a database to be useful, we must know the context of the numbers and the text it holds.
- When they are scattered about with no structure, the information is of very little use.
- Hence, we need to organize data.

### Dataset

- A structured collection of data.
- It is a collection of values $\to$ could be numbers, names, roll numbers.

## Variables and cases

- $Case(observation):$ A unit from which data are collected.
- $Variable:$
  - $Intuitive:$ A variable is that "varies".
  - $Formally:$ A characteristic or attribute that varies across all units.
- $Examples$
  - In our school dataset 
    - $Case:$ Each student.
    - $Variable:$ Name, marks obtained, Board etc.
- Rows represent cases: for each case, same attribute is recorded.
- Column represent variables: For each variables, same type of value for each case is recorded.

# Introduction and type of data : Classification of data

## Categorical and Numerical variables

- $Categorical\ data$
  - Also called qualitative variables.
  - Identity group membership
- $Numerical\ data$
  - Also called quantitative variables.
  - Describe numerical properties of cases.
  - Have measurement units
- $Measurement\ Unit:$ Scale that defines the meaning of numerical data. ($example:$ weights measured in kilograms, prices in rupees, heights in centimeters,etc.)
  - The data that make up a numerical variable in a data table must share a common unit.

## Cross-sectional and time-series data

- $Time\ series:$  data recorded over time 
- $Timeplot:$  graph of a time series data showing values in chronological order.
- $Cross-sectional:$ data observed at the same time 

# Introduction and type of data : Scales of measurement

- Data collection requires one of the following scales of measurement: Nominal, ordinal, interval, or ratio.

## Nominal Scale of measurement

- When the data for a variable consist of labels or names used to identify the characteristic of an observation, the scale of measurement is considered a nominal scale. 
  - $Examples:$ Name, Board, Gender, Blood Group etc.
- Sometimes nominal variables might be numerically coded.
  - $Example:$ Phone numbers, ZIP Codes/Postal Codes, ID numbers etc.
- There's no ordering in the variable.

### $Nominal:$ Name categories without implying order.

## Ordinal Scale of measurement

- Data exhibits properties of nominal data and the order or rank of data is meaningful, then the scale if measurement is considered a ordinal scale.
- $Example$
   - Each customer who visits a restaurant provides a service rating of excellent, good or poor.
     - The data obtained are the labels --- excellent, good, or poor --- the data have the properties of nominal data.
     - In addition, the data can be ordered, with respect to the service quality.
- $Ordinal:$ Name categories that can be ordered.

## Interval scale of measurement

- If the data have all the properties of ordinal data and the interval between values is expressed in terms of a fixed unit of measure, then the scale of measurement is interval scale.
- Interval data are always numeric. Can find out difference between any two values.
- Ratios of values have no meaning here because the value of zero is arbitrary.

### $Interval:$ Numerical values that can be added/subtracted and have no absolute zero.

- $Example:$ 
  - temperature 
    - Suppose the response to a question on how hot the day is comfortable and uncomfortable, then the temperature as a variable is $Nominal.$
    - Suppose the answer to measuring the temperature of a liquid is cold, warm, hot - the variable is $Ordinal.$
    - Consider a AC room where temperature is set at $20\degree C$ and the temperature outside the room is $40\degree C.$ It is correct to say that the difference in temperature is $20\degree C$, but it incorrect to say that the difference in temperature is $20\degree C$, but it is incorrect to say that the outdoors is twice as hot as indoors.
    - Temperature in degrees Fahrenheit or degrees centigrade is an interval variable. No absolute zero.

## Ratio scale of measurement

- If the data have all the properties of interval data and the ratio of two values is meaningful, then the scale of measurement is ratio scale.
- Example: height, weight, age, marks, etc.

### $Ratio:$ Numerical values that can be added, subtracted, multiplied or divide (makes ratio comparisons possible).

<center>
<br>

|True zero exists -- ratios possible|$Ratio\ Scale$|Age, Height, Height, Marks, etc.|
-|-|-

### $\uparrow$

|No absolute zero|$Interval\ Scale$|Temperature, GPA, etc.|
-|-|-

### $\uparrow$

|Named + Ordered|$Ordinal\ Scale$|Ranking, Rating, etc.|
-|-|-

### $\uparrow$

|Named|$Nominal Scale$| Name, Blood group, ID number, etc.|
-|-|-

</center>
