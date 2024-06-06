#### [[Polynomial Kernel]] of Degree $d$
$$
k(\vec {x},\vec {z}) = (\vec{x} \cdot \vec{z})^d
$$

Where: $d = 1$
- $d$ = represents the mapping to dimension $d$
And the transformations are given by:

$$
\phi(\vec {x})  \phi(\vec z) = \begin{bmatrix} x_1 \\ x_2 \end{bmatrix} \cdot \begin{bmatrix} z_1 \\ z_2 \end{bmatrix} = x_1z_1 + x_2z_2 = (\vec{x} \cdot \vec{z})
$$
### Second degree polynomial mapping
$$
\Phi({\vec x}) = \Phi\begin{bmatrix}
           x_1 \\
           x_2 
         \end{bmatrix} =
         \begin{bmatrix}
           x_1^2 \\
           \sqrt{2}x_1x_2 \\
           x_2^2 
         \end{bmatrix}
$$
Where: $d = 2$
$$
\Phi(\vec x)\Phi(\vec z)=\begin{bmatrix}
x_1^2 \\
\sqrt{2} x_1 x_2 \\
x_2^2
\end{bmatrix}
\cdot
\begin{bmatrix}
z_1^2 \\
\sqrt{2} z_1 z_2 \\
z_2^2
\end{bmatrix}
$$
$$
= x_1^2 z_1^2 + 2 x_1 x_2 z_1 z_2 + x_2^2 z_2^2 = (x_1 z_1 + x_2 z_2)^2 = ({\vec x} \cdot {\vec z})^2
$$
