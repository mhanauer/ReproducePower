---
title: "Readable English"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```
Test if you can reproduce with just means
```{r}
set.seed(123)
dataReal = as.data.frame(cbind(y = rnorm(100000), x = rnorm(100000)))
head(dataReal)
t.test(dataReal$y, dataReal$x)

mean(dataReal$y)
mean(yTest)
yTest = rnorm(mean(dataReal$y), sd(dataReal$y), n = length(dataReal$y))
xTest = rnorm(mean(dataReal$x), sd(dataReal$y), n = length(dataReal$x))
t.test(yTest, xTest)

cor(yTest, xTest)
cor(dataReal$y, dataReal$x)
```

