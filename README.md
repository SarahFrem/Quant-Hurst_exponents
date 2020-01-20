# Quantitative finance 

## Hurst Exponents estimation in a multifractional Brownian motion

### Simulation Study and Application to FX market on a high frequency basis (15 minutes)

Based on Mr Matthieu Garcin research paper: Estimation of time-dependent Hurst exponents with variational smoothing and application to forecasting foreign exchange rates (2017 Elsevier B.V)

_What's a standard brownian motion W_t in a few properties:_
- 𝑊_0 = 0 
- 𝑊_𝑡 continuous
- Increments are independant
- 𝑊_𝑡 – 𝑊_𝑠 ~ N(0, t-s), 0 ≤ s ≤ t
		
_What's a fractional brownian motion W_t in a few additonal properties:_
- Ε[(W_𝑡 – 𝑊_𝑠)^2 ]= 𝜎^2 |𝑡 −𝑠|^2𝐻
- Ε[ W_t . W_s ]= 𝜎^2 (|𝑡|^2𝐻+ |𝑠|^2𝐻  − |𝑡 −𝑠|^2𝐻)
- Increments are correlated with a H ≠ 1/2

_What's then a multifractional brownian motion:_
- Hurst Exponents are time-dependent
- Ε[𝑊_𝑡 .𝑊_𝑠 ]=  𝜎^2/2  𝑔 (𝐻(𝑡)+𝐻(𝑠))  (|𝑡 |^(𝐻(𝑡)+𝐻(𝑠))+ |𝑠|^(𝐻(𝑡)+𝐻(𝑠))  − |𝑡 −𝑠|^(𝐻(𝑡)+𝐻(𝑠)))

The paper gives a method called variational smooting for estimating time-dependent Hurst exponents:
  - Study case on simulated MbM
  - Study case on 15 min basis FX market time series where the observation of a long memory leads to the key hypothesis: those time series are driven by an underneath MbM.  


