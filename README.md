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
  
    ![Mean value equation](mean.png)<br/>
*Equation 1. The mean value*.
  - The **standard deviation**

    ![Standard deviation equation](standard-deviation.png)<br/>
*Equation 2. The standard deviation*.
  - The **standard deviation of the mean** or **standard error**

    ![Standard error](standard-error.png)<br/>
*Equation 3. The standard error*.
- Each of the functions should be part of a Python script called `geo-stats.py`.
- Within the `geo-stats.py` file, include tests that demonstrate your code is working properly using the two tables of geochronological ages below.
  - To input the data you can simply create lists of the ages, rather than reading a file.
  - Your tests should use your three functions to calculate the mean, standard deviation, and standard error for each set of ages.
  - In addition, you should use the NumPy functions `np.mean()`, `np.std()`, and `np.sqrt()` to calculate the mean, standard deviation, and standard error values for each age list.
  - The calculated values can be output to the screen using the `print()` function.

### Questions for Problem 1

## Hints
If you get stuck, have a look at the [hints for this week's exercise]().

# Answers
This is some text.
You can make it **bold** or use *italics*.
You can also display images, as shown below.

![A sine curve](img/sine-curve.png)<br/>
*Figure 1. A sine curve*.
