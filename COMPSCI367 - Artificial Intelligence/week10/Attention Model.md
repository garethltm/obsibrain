- this [[model(s)]] allows an [[Recurrent Neural Network (RNN)]] to pay attention to specific parts of the input that is considered as being important, which improves the performance of the resulting [[model(s)]] in practice. By noting $\alpha ^{<t,t'>}$ the amount of attention that output $y^{<t>}$ should pay to the activation $a^{<t'>}$ & $c^{<t>}$ the context at time t, we have:
$$c^{<t>}=\displaystyle\sum_{t'}\alpha ^{<t,t'>}a^{<t'>}$$
with
$$\displaystyle\sum_{t'}\alpha ^{<t,t'>}=1$$