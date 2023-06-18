# Approximating-prices-and-greeks-in-continuous-time-models
Implementation of paper of Kristensen and Mele: Adding and subtracting Black-Scholes: A new approach to approximating derivative prices in continuous-time models. 
This repository contains almost all the numerical experiments in Section 5 of the paper.

`derivative prices` contains the numerical results of option prices under both Heston and non-affine model respectively corresponding to Table 1 and 2 and `greeks` contains the numerical results of some greeks under the same two models corresponding to Table 3 and 4.
All the numerical experiments above are from Section 5.1.2.2.
Both two series of experiments fix the instantaneous return variance or initial underlying stock price at a time and respectively take different values of the other.
Although the difference between Heston and non-affine model is just the parameter $\xi$ (0.5 in the former while 0.6 in the latter), 
we can always get exactly the same results with the JFE paper for Heston model and somehow slightly biased results for non-affine model, with some of them systemicly larger while some others differs irregularly.
However, we can conclude that the approximation works quite well.

`bond prices` contains the numerical results of bond prices with a maturity of six months under a non-affine two-factor model corresponding to the first panel of Table 5 from Section 5.2.2. 
We still obtain results that are slightly larger than both benchmark values and results in JFE paper.
