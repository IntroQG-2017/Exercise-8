# Exercise 8: Coding and visualizing geostatistics
In this week's exercise we will take our first steps toward learning how to convert equations into Python code, and visualizing some geochronological data.
We will be using Python tools that are already familiar to us, but applying them in a slightly different way than in the earlier exercises.

This exercise is due by the start of class on **7.11.2016**.
Late submissions will lose 25% of the total points per day late.

## Problem 1: Converting math to Python
One of the goals of this part of the course is to develop your quantitative geoscience skills, including learning how to convert mathematical equations to Python code.
Doing this allows you to explore how various equations work and produce useful data plots or predictions, something increasingly done by geoscience professionals.

- For this problem, you should create Python functions for the following common statistical equations:
  - The **mean** or **average**, calculated using a function you should call `mean()`.
  
    ![Mean value equation](Images/mean.png)<br/>
*Equation 1. The mean value, where x<sub>i</sub> is a value to be included in the mean calculation and N is the total number of values to average*.
  - The **standard deviation**, calculated using a function you should call `stddev()`.

    ![Standard deviation equation](Images/standard-deviation.png)<br/>
*Equation 2. The standard deviation*.
  - The **standard deviation of the mean** or **standard error**, calculated using a function you should call `stderr()`.

    ![Standard error](Images/standard-error.png)<br/>
*Equation 3. The standard error*.
- Each of the functions should be part of a Python script called `geo-stats.py`.
- Within the `geo-stats.py` file, include tests that demonstrate your code is working properly using the ages measured for minerals in the five geochronological samples below.

    | Sample    | Subsample ID | Age [Ma] | 
    | --------- | ------------ | -------- |
    | **F09**   | F09-1        | 2.01     |
    |           | F09-2        | 1.95     |
    |           | F09-3        | 2.38     |
    |           | F09-4        | 2.3      |
    |           | F09-5        | 2.0      |
    | **BH63**  | BH63-1       | 4.77     |
    |           | BH63-2       | 5.11     |
    |           | BH63-3       | 3.30     |
    |           | BH63-4       | 3.34     |
    |           | BH63-5       | 4.45     |
    | **BH161** | BH161-1      | 8.8      |
    |           | BH161-3      | 2.15     |
    | **BH412** | BH412-1      | 4.74     |
    |           | BH412-2      | 5.14     |
    |           | BH412-3      | 5.14     |
    |           | BH412-4      | 5.5      |
    |           | BH412-5      | 5.1      |
    | **BHF04** | BHF04-1      | 2.21     |
    |           | BHF04-3      | 5.1      |
    |           | BHF04-4      | 2.93     |
    |           | BHF04-5      | 4.69     |<br/>
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
In this problem we will continue to develop our Python mathematical and plotting skills by visualizing the calculated sample geochronological ages from Problem 1 using the *normal distribution*.
The normal distribution is a mathematical function with a bell shape, also known as the *Gauss function* or *Gaussian*.
This function is centered on the mean value of a given set of values, where its value is greatest, and its value decreases away from the mean in what is hopefully a familiar form.
Your tasks in the exercise are to:

1. Use the mean and standard deviation values calculated in Problem 1 to calculate the normal distribution for each of the five samples in Table 1.
  - Since you will use the values and functions from Problem 1 in this problem, I suggest you make a copy of your code from Problem 1 and save it in your exercise repository as `geo-stats-problem2.py`.
  - The mathematical definition of the normal function is

    ![The normal distribution](Images/normal-distribution.png)<br/>
    *Equation 4. The normal distribution, where e is the exponential function and x is the value for which the normal distribution is calculated, some age within a range of ages in our case*.
  - You should convert this equation to a Python function called `gaussian()`, and save it in your `geo-stats-problem2.py` file.
  - The ages for which the normal distribution should be calculated are from 0-10 Ma in increments of 0.1 Ma.
  In other words, at each of those ages you will calculate the value of the normal distribution for each sample.
  - The resulting five normal distribution values should be plotted using Matplotlib.
    - Formatting stuff goes here...

## Hints
If you get stuck, have a look at the [hints for this week's exercise](https://github.com/Intro-Quantitative-Geology/Lesson-8-Basic-geostatistics/blob/master/Lesson/hints.md).

### Footnote(s)
[1]: [Coutand, I., Whipp, D.M., Grujic, D., Bernet, M., Fellin, M.G., Bookhagen, B., Landry, K.R., Ghalley, S.K. and Duncan, C., 2014. Geometry and kinematics of the Main Himalayan Thrust and Neogene crustal exhumation in the Bhutanese Himalaya derived from inversion of multithermochronologic data. *Journal of Geophysical Research: Solid Earth*, *119*(2), pp.1446-1481](https://dx.doi.org/10.1002/2013JB010891)

# Answers
This is some text.
You can make it **bold** or use *italics*.
You can also display images, as shown below.

![A sine curve](Images/sine-curve.png)<br/>
*Figure 1. A sine curve*.
