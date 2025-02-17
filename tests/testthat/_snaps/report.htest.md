# report.htest

    Code
      report(cor.test(mtcars$wt, mtcars$mpg))
    Output
      Effect sizes were labelled following Funder's (2019) recommendations.
      
      The Pearson's product-moment correlation between mtcars$wt and mtcars$mpg is negative, statistically significant, and very large (r = -0.87, 95% CI [-0.93, -0.74], t(30) = -9.56, p < .001)

---

    Code
      report(cor.test(mtcars$wt, mtcars$mpg, method = "spearman"))
    Warning <simpleWarning>
      Cannot compute exact p-value with ties
    Output
      Effect sizes were labelled following Funder's (2019) recommendations.
      
      The Spearman's rank correlation rho between mtcars$wt and mtcars$mpg is negative, statistically significant, and very large (rho = -0.89, S = 10292.32, p < .001)

---

    Code
      report(cor.test(mtcars$wt, mtcars$mpg, method = "kendall"))
    Warning <simpleWarning>
      Cannot compute exact p-value with ties
    Output
      Effect sizes were labelled following Funder's (2019) recommendations.
      
      The Kendall's rank correlation tau between mtcars$wt and mtcars$mpg is negative, statistically significant, and very large (tau = -0.73, z = -5.80, p < .001)

---

    Code
      report(t.test(iris$Sepal.Width, mu = 1))
    Output
      Effect sizes were labelled following Cohen's (1988) recommendations.
      
      The One Sample t-test testing the difference between iris$Sepal.Width (mean = 3.06) and mu = 1 suggests that the effect is positive, statistically significant, and large (difference = 2.06, 95% CI [2.99, 3.13], t(149) = 57.81, p < .001; Cohen's d = 4.72, 95% CI [4.17, 5.29])

---

    Code
      report(t.test(iris$Sepal.Width, mu = -1, alternative = "l"))
    Output
      Effect sizes were labelled following Cohen's (1988) recommendations.
      
      The One Sample t-test testing the difference between iris$Sepal.Width (mean = 3.06) and mu = -1 suggests that the effect is positive, statistically not significant, and large (difference = 4.06, 95% CI [-Inf, 3.12], t(149) = 114.01, p > .999; Cohen's d = 9.31, 95% CI [8.25, 10.40])

---

    Code
      report(t.test(iris$Sepal.Width, mu = 5, alternative = "g"))
    Output
      Effect sizes were labelled following Cohen's (1988) recommendations.
      
      The One Sample t-test testing the difference between iris$Sepal.Width (mean = 3.06) and mu = 5 suggests that the effect is negative, statistically not significant, and large (difference = -1.94, 95% CI [3.00, Inf], t(149) = -54.59, p > .999; Cohen's d = -4.46, 95% CI [-5.80, -3.93])

---

    Code
      report(t.test(formula = wt ~ am, data = mtcars))
    Output
      Effect sizes were labelled following Cohen's (1988) recommendations.
      
      The Welch Two Sample t-test testing the difference of wt by am (mean in group 0 = 3.77, mean in group 1 = 2.41) suggests that the effect is negative, statistically significant, and large (difference = -1.36, 95% CI [0.85, 1.86], t(29.23) = 5.49, p < .001; Cohen's d = 2.03, 95% CI [1.13, 2.91])

---

    Code
      report(t.test(formula = wt ~ am, data = mtcars, alternative = "l"))
    Output
      Effect sizes were labelled following Cohen's (1988) recommendations.
      
      The Welch Two Sample t-test testing the difference of wt by am (mean in group 0 = 3.77, mean in group 1 = 2.41) suggests that the effect is negative, statistically not significant, and large (difference = -1.36, 95% CI [-Inf, 1.78], t(29.23) = 5.49, p > .999; Cohen's d = 2.03, 95% CI [1.13, 2.91])

---

    Code
      report(t.test(formula = wt ~ am, data = mtcars, alternative = "g"))
    Output
      Effect sizes were labelled following Cohen's (1988) recommendations.
      
      The Welch Two Sample t-test testing the difference of wt by am (mean in group 0 = 3.77, mean in group 1 = 2.41) suggests that the effect is negative, statistically significant, and large (difference = -1.36, 95% CI [0.94, Inf], t(29.23) = 5.49, p < .001; Cohen's d = 2.03, 95% CI [1.13, 2.91])

---

    Code
      report(t.test(Pair(extra.1, extra.2) ~ 1, data = sleep2))
    Output
      Effect sizes were labelled following Cohen's (1988) recommendations.
      
      The Paired t-test testing the difference between Pair(extra.1, extra.2) (mean of the differences = -1.58) suggests that the effect is negative, statistically significant, and large (difference = -1.58, 95% CI [-2.46, -0.70], t(9) = -4.06, p < .01; Cohen's d = -1.35, 95% CI [-2.23, -0.44])

