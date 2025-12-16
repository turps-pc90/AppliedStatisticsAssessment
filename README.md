# Applied Statistics Assessment

![Atlantic Technological University - ATU](https://www.atu.ie/app/themes/atu-theme/assets/main/img/layout/logo-full-accent.svg)

## Table of Contents

- [Assessment Instructions](#assessmentInstructions)
- [Technologies Used](#techUsed)
- [Running The Notebook](#usage)
- [References](#references)

## Assessment Instructions <a id="assessmentInstructions"></a>

### Problem 1: Extending the Lady Tasting Tea

Let's extend the Lady Tasting Tea experiment as follows.
The original experiment has 8 cups: 4 tea-first and 4 milk-first.
Suppose we prepare 12 cups: 8 tea-first and 4 milk-first.
A participant claims they can tell which was poured first.  

Simulate this experiment using `numpy` by randomly shuffling the cups many times and calculating the probability of the participant correctly identifying all cups by chance.
Compare your result with the original 8-cup experiment.  

In your notebook, explain your simulation process clearly, report and interpret the estimated probability, and discuss whether, based on this probability, you would consider extending or relaxing the p-value threshold compared to the original design.  

### Problem 2: Normal Distribution

Generate 100,000 samples of size 10 from the standard normal distribution.
For each sample, compute the standard deviation with `ddof=1` (sample SD) and with `ddof=0` (population SD).
Plot histograms of both sets of values on the same axes with transparency.
Describe the differences you see.
Explain how you expect these differences to change if the sample size is increased.

### Problem 3: t-Tests

A type II error occurs when a test fails to reject the null hypothesis even though it is false.
For each mean difference $d = 0, 0.1, 0.2, \dots, 1.0$, repeat the following simulation 1,000 times:

1. Draw two samples of size 100, one from the standard normal distribution and one from the normal distribution with mean $d$ and standard deviation 1.
2. Run an independent samples t-test on the two samples, rejecting the null hypothesis if the p-value is less than 0.05.
3. Record the proportion of times the null hypothesis is not rejected.

Plot this proportion against $d$, and explain how the type II error rate changes as the difference in means increases.

### Problem 4: ANOVA

Generate three independent samples, each of size 30, from normal distributions with means 0, 0.5, and 1, each with standard deviation 1.

1. Perform a one-way ANOVA to test whether all three means are equal.
2. Perform three independent two-sample t-tests: samples 1 vs 2, 1 vs 3, and 2 vs 3.
3. Compare the conclusions.

Write a short note on why ANOVA is preferred over running several t-tests.

-----

## Technologies Used <a id="techUsed"></a>

| Python | Jupyter Notebook |  NumPy | SciPy | Matplotlib | Seaborn |
|-------|-------|-------|-------|------------|---------|
| ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) | ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white) | ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) | ![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=white) | ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) | ![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge) |

-----

## Running The Notebook <a id="usage"></a>

The project is available here - https://github.com/turps-pc90/AppliedStatisticsAssessment - and all files associated with the project are stored in this repository. It can be cloned by using the following command:

<p>git clone https://github.com/turps-pc90/AppliedStatisticsAssessment.git</p>

Install the required dependencies by using the requirements.txt file provided in the GitHub repository.

The use of seeds throughout the problems ensures that the output of each task and the functions within them are reproducible. 

-----

## References <a id="references"></a>

**Pandas Documentation** (2025). *pandas.pivot_table — pandas 2.3.3 documentation* [online].  
   Available at: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.pivot_table.html  
   (Accessed: 24 October 2025).

**Plotly Technologies Inc.** (2025). *Getting started with Plotly in Python – Jupyter Notebook Support* [online].  
   Available at: https://plotly.com/python/getting-started/#jupyter-notebook-support  
   (Accessed: 24 October 2025).

**NumPy Documentation** (2025). *NumPy Reference — NumPy v1.x Documentation* [online].  
    Available at: https://numpy.org/doc/stable/reference/index.html#reference  
    (Accessed: 15 December 2025).

**Waskom, M.** (2024). *seaborn: statistical data visualization — seaborn 0.13.2 documentation* [online].  
   Available at: https://seaborn.pydata.org/  
   (Accessed: 1 November 2025).

**Matplotlib Development Team** (2025). *Quick start guide — Matplotlib 3.10.5 documentation* [online].  
   Available at: https://matplotlib.org/stable/users/explain/quick_start.html  
   (Accessed: 1 November 2025).

**Bhattacharyya, D.** (2024). *Z-Scores and the Standard Normal Distribution in Python: From Theory to Practice* [online]. Medium.  
   Available at: https://medium.com/@bdebika_73918/z-scores-and-the-standard-normal-distribution-in-python-from-theory-to-practice-99f4d3fd7fe9  
   (Accessed: 1 November 2025).

**Chugani, V.** (2024). *How to Use NumPy for Probability Distributions* [online]. Statology.  
   Available at: https://www.statology.org/how-to-use-numpy-for-probability-distributions/  
   (Accessed: 25 November 2025).

**Guttag, J.** (2016). *Lecture 6: Monte Carlo Simulation*. In: *Introduction to Computational Thinking and Data Science — Fall 2016*.  
   Massachusetts Institute of Technology: MIT OpenCourseWare [online].  
   Available at: https://ocw.mit.edu/courses/6-0002-introduction-to-computational-thinking-and-data-science-fall-2016/resources/lecture-6-monte-carlo-simulation/  
   (Accessed: 29 November 2025).

**Chosnek, D.** (2022). *How To Use the Underscore (_) Properly in Python*. Better Programming [Medium], 6 September.  
   Available at: https://medium.com/better-programming/how-to-use-underscore-properly-in-python-37df5e05ba4c  
   (Accessed: 29 November 2025).

**GeeksforGeeks** (2025). *P-Value: Comprehensive Guide to Understand, Apply, and Interpret* [online].  
   Available at: https://www.geeksforgeeks.org/machine-learning/p-value/  
   (Accessed: 1 December 2025).

**Gilbert, J.** (2017). *What are degrees of freedom* [online video]. YouTube.  
    Available at: https://www.youtube.com/watch?v=rATNoxKg1yA  
    (Accessed: 10 December 2025).

**Penn State Eberly College of Science** (n.d.). *STAT 200: Elementary Statistics – Lesson 6.1: Type I and Type II Errors*.  
    Available at: https://online.stat.psu.edu/stat200/lesson/6/6.1  
    (Accessed: 13 December 2025).

**Starmer, J.** (2015). *Hypothesis testing and p-values*. StatQuest with Josh Starmer.  
    Available at: https://www.youtube.com/watch?v=0oc49DyA3hU  
    (Accessed: 13 December 2025).

**Laerd Statistics** (2023). *One-way ANOVA using SPSS Statistics* [online].  
    Available at: https://statistics.laerd.com/spss-tutorials/one-way-anova-using-spss-statistics.php  
    (Accessed: 15 December 2025).

**SciPy** (2023). *scipy.stats.f_oneway* [online].  
    Available at: https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.f_oneway.html  
    (Accessed: 15 December 2025).

**Wikipedia** (2023). *Analysis of variance* [online].  
    Available at: https://en.wikipedia.org/wiki/Analysis_of_variance  
    (Accessed: 15 December 2025).

**GeeksforGeeks** (2025). *Difference Between T-Test and ANOVA* [online].  
    Available at: https://www.geeksforgeeks.org/data-science/difference-between-t-test-and-anova/  
    (Accessed: 15 December 2025).
