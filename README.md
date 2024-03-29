# SpecLim Calculator 
Created to validate the [Shiny Application and Reproducible Pitch Coursera Project](https://www.coursera.org/learn/data-products?specialization=data-science-statistics-machine-learning) 

This **SpecLimits Calculator** RShiny app is built to facilitate the setting of those specification limits for process parameters having **at least** an historical of **20 batch results**.

In that case, the specifications limits assessment is based on the following statistical methodology:

- If the distribution of the parameter is supposed to normal and justified by a Shapiro-Wilk test at 1% level, then the specification limits will be based on a parametric approach using the confidence-coverage tolerance interval (2-sided, or upper limit or lower limit) estimation

- If the Shapiro-Wilk test reject the normal distribution, the log-normality is tested and

    - if the log-normality is not rejected then, the specification limits will be based on a confidence-coverage tolerance interval (2-sided, or upper limit or lower limit) using the log-transformed data. The limits will then be back-transformed.
    - else (if the log-normality is rejected), the distribution is unknown and a non-parametric approach will be used (Parametric capability-based limits) 
  

See the **RShiny app** [here](https://hajeramara.shinyapps.io/SpecLim/)

To test it, just download the Data.xlsx file from the git repository.

For **more details**, please see the **pitch**: https://rpubs.com/HSA75/987043



