---
title       : BMI Calculator
subtitle    : Using the Shiny BMI Calculator APP  
author      : Ryan Wissman
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Body Mass Index

1. Body mass index is a measure of body fat based on weight and height
2. This measure is a simple way to determine your body's current status (normal, underweight, overweight)
3. Knowing only your height and weight the BMI calculator can quickly determine your BMI category and will place your current status on a chart of BMI ranges
4. This calculator was designed to be easy to use and can be used by any user
5. The APP was designed to use either imperial or metric measurements so it can be used by just about anybody

--- .class #id 

## The BMI Weight Ranges
1. While an imperfect measure, BMI does have weight ranges 
2. The following table displays the CDC published ranges for BMI

| BMI            | Weight Status            |
|----------------|--------------------------|
| Below 18.5     | Underweight              |
| 18.5 - 24.9    | Normal or Healthy Weight |
| 25.0 - 29.9    | Overweight               |
| 30.0 and Above | Obese                    |


3. You can find more information on the CDC's website:
4. http://www.cdc.gov/healthyweight/assessing/bmi/adult_bmi/index.html

--- .class #id 

## The Formula (Imperial)

1. There are two distinct formulas used to calculate BMI. 
2. The formula to calculate BMI for imperial measurements is as follows
3. Weight (in pounds) / (Height (in inches) * Height (in inches)) * 703
4. 703 is a constant. 
5. For example, let's say you have a height of 69 inches and weight 165 pounds:


```r
165 / 69^2 * 702
```

```
## [1] 24.32892
```

6. The number displayed above would be your BMI and it would indicate that you have a normal weight.

--- .class #id 

## The Formula (Metric)

1. For metric measures the formula is the same, without the constant 703 as follows
2. Weight (in kilograms) / (Height (in centimeters) * Height (in centimeters) / 100)
3. Therefore, if we have a weight of 70kg and a height of 2.0 meters (200 centimeters):


```r
70 / (200/100)^2
```

```
## [1] 17.5
```

4. The number above would indicate that we have a normal body weight.

--- .class #id 

## Shiny BMI Calculator App

1. The shiny BMI calculator is a great way to quickly determine your BMI
2. The app will give you an instant answer as to wether you have a healthy or unhealthy weight
3. Another useful feature of the app is that it will display a chart indicating health and unhealthy weight ranges and plot your input criteria directly on the chart
4. You can access the BMI calculator here: https://speedy3d.shinyapps.io/Coursera-DataProducts-Project-BMI
