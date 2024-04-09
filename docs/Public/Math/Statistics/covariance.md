*See: [[correlation]]*

*Covariance* is a normalized ([[normalmeasure of how two variables ([[variable]]) $X$ and $Y$ change together linearly. 

Given a population of size $n$, it is calculated as follows:

$$
COV[X, Y] = E[(X - E[X])(Y - E[Y])] = \frac{\Sigma^n_{i=1} (X_i-\overline{X})(Y_i-\overline{Y})}{n}
$$
The sign of the *covariance* indicates the direction of the relationship between variables:
- when $COV[X, Y] > 0$, $X$ and $Y$ increase and decrease together.
- when $COV[X, Y] < 0$, $X$ tends to decrease while $Y$ tends to increase and vice versa.
- when $COV[X, Y] = 0$, $X$ and $Y$ do not display any of the above two tendencies. No linear relationship between $X$ and $Y$. 

Note: *Covariance can only measure the directional relationship, not the magnitude. *