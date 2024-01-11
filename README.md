# Theoretical Neuroscience

Computational neuroscience I did in my course on Theoretical Neuroscience (WS 22/23). 

## Rate networks model and chaotic dynamics

Model of rate networks depicting interaction of neuron populations via spike rates. Neuron population states are described by activation levels ($x_i(t)$ for population $i$).
Spike rate for this activation level is $r_i(t) = f(x_i(t))$. $f(x) = tanh(x)$ is the nonlinear transfer function. Weight function $W_{ij}$ determines impact of spike rate on population $j$ by $i$ and is modelled by a Gaussian. 
Overall dynamics described by: 
$\frac{dx_i(t)}{dt} = -x_i(t) + {\sum_{j=1}}^N W_{ij} f(x_j(t))$

## Poisson Spike Train

Simulation of a homogeneous Poisson spike train with rate 1 spike per time unit and distributions of number of spikes and interspike intervals. 
