# Rate-Networks

Model of rate networks depicting interaction of neuron populations via spike rates. Neuron population states are described by activation levels ($x_i(t)$ for population $i$).
Spike rate for this activation level is $r_i(t) = f(x_i(t))$. $f(x) = tanh(x)$ is the nonlinear transfer function. Weight function $W_{ij}$ determines impact of spike rate on population $j$ by $i$ and is modelled by a Gaussian. 
Overall dynamics described by: 
\begin{equation}
\frac{dx_i(t)}{dt} = -x_i(t) + \sum_{j=1}^N W_{ij} f(x_j(t))
\end{equation}
