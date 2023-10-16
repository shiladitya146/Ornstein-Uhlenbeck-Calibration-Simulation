# Ornstein-Uhlenbeck-Calibration-Simulation

Ornstein-Uhlenbeck (OU) is a mean-reverting continuous time stochastic process often used in simulation of price dynamics in the energy markets.  
The OU process is represented as:  
<p align="center">$dx_t= θ(μ- x_t )dt+ σdW_t$</p><br>

* $x_t$  is a variable being modelled<br>
* $θ$ is the mean reversion spread<br>    
* $μ$ is the long term mean level<br>    
* $σ$ is the volatility<br>    
* $dt$ is an infinitesimal time step<br>    
* $dW_t$  is brownian motion (random part)<br>  

The three parameters (θ,μ,σ) are calibrated to a historical time series using either of the 3 approaches:<br>
* Maximum likelihood estimation (MLE)<br>
* Least squares regression<br>
* Analytical formula<br>

Referencing the paper ‘**_Calibration of the exponential Ornstein–Uhlenbeck process when spot prices are visible through the maximum log-likelihood method. Example with gold prices_**’<a href="https://www.researchgate.net/publication/326883877_Calibration_of_the_exponential_Ornstein-Uhlenbeck_process_when_spot_prices_are_visible_through_the_maximum_log-likelihood_method_Example_with_gold_prices" >(Link)</a> here is a python implementation of Ornstein–Uhlenbeck in discrete time.<br>

Within the juypter notebook you will find the following:<br>
* Calibration of the three parameters (θ,μ,σ) from a JKM time series using both MLE and analytical formula.<br>
* Use the calibrated parameters in simulating JKM prices n days forward. 


