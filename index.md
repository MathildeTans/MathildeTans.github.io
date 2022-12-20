---
title: BST 260 Final Project
feature_text: |
  ## The global effect of maternal education on childhood stunting
  Mathilde Tans
feature_image: "https://img.freepik.com/free-photo/luxury-plain-green-gradient-abstract-studio-background-empty-room-with-space-your-text-picture_1258-63593.jpg?w=2000"
excerpt: "Childhood stunting affects almost a quarter of all children under five worldwide. Aside from not reaching the (WHO) standard height for their age, stunted children are put at a disadvantage due to delayed cognitive and mental development. Recent studies tell us that maternal education can protect children from stunting. In this study, we quantify the global effect of maternal education on childhood stunting."
---

Childhood stunting affects almost a quarter of all children under five worldwide. Aside from not reaching the (WHO) standard height for their age, stunted children are put at a disadvantage due to delayed cognitive and mental development. Recent studies tell us that maternal education can protect children from stunting. In this study, we quantify the global effect of maternal education on childhood stunting.

For this study, we rely on data from the WHO Child Nutrition database and data from the World Bank. The data from the WHO is comprised of stunting prevalences from various studies around the world from the last 30 years. Some of these studies recorded the level of maternal education: no education, primary education, or secondary education. Commonly, an analysis into stunting takes the childrens' sex and age into account, as well as the area of residence (urban/rural/both). However, there is no variation in these variables in our cleaned dataset, hence we do not (have to) include age, sex, and area. 

Since household wealth and level of sanitation usage are important factors, we find proxies from the World Bank on the country level. We use GDP per capita and the percentage of the population using at least basic levels of sanitation. We take the log of the GDP and plot this against sanitation usage. The size and color of the dots is determined by the prevalence of stunting. 

![plot1](https://user-images.githubusercontent.com/73693703/208687026-ed58a959-d154-454a-990c-e5a3350a9d21.png)

In addition, we plot the prevalence of stunting against the GDP per capita. The color of the dots is determined by the level of maternal education. We see a clear shift in average prevalence of stunting between the different levels of maternal education. 

![plot2](https://user-images.githubusercontent.com/73693703/208687037-4fc65a5e-1f56-4f0c-9a23-0d5b011c0eb5.png)

## Results

We use weighted least squares to find precisely what this shift is, i.e., the effect of maternal education on childhood stunting. Based on this analysis we find that, on average, mothers who have been able to have either of the following levels of education will lead to a certain prevalence of stunting:
* No education: 37.22%
* Primary education: 30.61%
* Secondary education: 19.98%

It is worth to note, that the WHO database will include studies conducted in area's where it makes sense to study child stunting. Therefore, to be more correct, the above numbers do not reflect the overall global effect, but the average effect of maternal education across the world where childhood stunting is still a current and relevant problem. 

## Conclusion

Especially having a mother with a secondary education protects the children from being stunted. Namely, the estimated prevalence of stunting is roughly 15 percentage points lower when the mother has enjoyed secondary education compared to children whose mother has no education. This study confirms the results found in specific regions on a global level and calls for more research in how to utilize and/or improve maternal education to prevent childhood stunting. 
