# Exercise-8: 

This exercise is due by the start of class on **7.11.2016**.
Late submissions will lose 25% of the total points per day late.

## Ideas
- Reporting measured values as mean ± std dev (or std error) - best estimate ± uncertainty
  - Round to 1 significant figure, report mean to same range
- Converting formulas to Python
  - Mean
  - Std deviation
  - Std error
- Visualizing uncertainty
  - Errorbar plots
  - Normal distribution (yes)

## Problem 1: Converting math to Python
One of the goals of this part of the course is to develop your quantitative geoscience skills, including learning how to convert mathematical equations to Python code.
Doing this allows you to explore how various equations work and produce useful data plots or predictions, something increasingly done by geoscience professionals.

- For this problem, you should create Python functions for the following common statistical equations:
  - The **mean** or **average**
  
    ![Mean value equation](Images/mean.png)<br/>
*Equation 1. The mean value, where x<sub>i</sub> is a value to be included in the mean calculation and N is the total number of values to average*.
  - The **standard deviation**

    ![Standard deviation equation](Images/standard-deviation.png)<br/>
*Equation 2. The standard deviation*.
  - The **standard deviation of the mean** or **standard error**

    ![Standard error](Images/standard-error.png)<br/>
*Equation 3. The standard error*.
- Each of the functions should be part of a Python script called `geo-stats.py`.
- Within the `geo-stats.py` file, include tests that demonstrate your code is working properly using the ages measured for minerals in the two geochronological samples below.

    | Sample   | Subsample ID | Age [Ma] | 
    | -------- | ------------ | -------- |
    | **F09**  | F09-1        | 2.01     |
    |          | F09-2        | 1.95     |
    |          | F09-3        | 2.38     |
    |          | F09-4        | 2.3      |
    |          | F09-5        | 2.0      |
    | **BH63** | BH63-1       | 4.77     |
    |          | BH63-2       | 5.11     |
    |          | BH63-3       | 3.30     |
    |          | BH63-4       | 3.34     |
    |          | BH63-5       | 4.45     |<br/>
*Table 1. Apatite (U-Th)/He thermochronometer ages from Coutand et al. (2014)*[1].
  - To input the data you can simply create lists of the ages, rather than reading a file.
  - Your tests should use your three functions to calculate the mean, standard deviation, and standard error for each set of ages.
  - In addition, you should use the NumPy functions `np.mean()`, `np.std()`, and `np.sqrt()` to calculate the mean, standard deviation, and standard error values for each age list.
  - The calculated values can be output to the screen using the `print()` function.

### Questions for Problem 1
1. 
2. 
3. 

## Problem 2: Visualizing uncertainty


## Hints
If you get stuck, have a look at the [hints for this week's exercise]().

### Footnote(s)
[1]: [Coutand, I., Whipp, D.M., Grujic, D., Bernet, M., Fellin, M.G., Bookhagen, B., Landry, K.R., Ghalley, S.K. and Duncan, C., 2014. Geometry and kinematics of the Main Himalayan Thrust and Neogene crustal exhumation in the Bhutanese Himalaya derived from inversion of multithermochronologic data. *Journal of Geophysical Research: Solid Earth*, *119*(2), pp.1446-1481](https://dx.doi.org/10.1002/2013JB010891)

# Answers
This is some text.
You can make it **bold** or use *italics*.
You can also display images, as shown below.

![A sine curve](Images/sine-curve.png)<br/>
*Figure 1. A sine curve*.
