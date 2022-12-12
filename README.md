# Principal-Component-Analysis

# Overview

This program is designed to perform a Principal Components Analysis on an unnamed brewery. Once I have completed the PCA, I will investigate the loadings of the first 6 components.

**Local data and authentication keys removed for anonymity.

# Process

To begin the program I will connect and authenticate my service account with my Google Big Query project (containing the data needed for the PCA). Once I have connected to my project, I'll build a SQL query that returns my needed columns and feeds the results into a pandas dataframe. Finally I will pivot my dataframe to allow me to begin my PCA.

Next I will begin my PCA using SKLearn. I'll limit my PCA to 20 components and set svd_solver to full. Then I'll build a plot of the first 20 components based on their explained variance. Plot code adapted from https://medium.com/analytics-vidhya/pca-and-how-to-interpret-it-with-python-8aa664f7a69a

Now I am ready to investigate the loadings of the top 6 components within my PCA. I used a function from https://medium.com/analytics-vidhya/pca-and-how-to-interpret-it-with-python-8aa664f7a69a to allow me to plot the loadings within each component. Finally I will interpret the results.
