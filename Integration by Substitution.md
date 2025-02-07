We use $u=g(x)$, $du=g'(x)dx$ to compute $$\int f(g(x))\cdot g'(x)=\int f(u)du$$
This is very abstract and hard to understand. It's difficult to identify when an expression we're trying to integrate follows the pattern on the left. Let's break it down with a simple example.
$$\int cos(x^2)\cdot 2xdx$$
Here, $u=g(x)=x^2$   $du=g'(x)=2xdx$. Now we can easily compute $$\int cos(u)du=sin(u)=sin(x^2)+C$$
### Why does this work? A basic explanation
Let's say we have a function $f(z)$, with $F(z)$ its antiderivative. 
