We use $u=g(x)$, $du=g'(x)dx$ to compute $$\int f(g(x))\cdot g'(x)=\int f(u)du$$
This is very abstract and hard to understand. It's difficult to identify when an expression we're trying to integrate follows the pattern on the left. Let's break it down with a simple example.
$$\int cos(x^2)\cdot 2xdx$$
Here, $u=g(x)=x^2$   $du=g'(x)=2xdx$. Now we can easily compute $$\int cos(u)du=sin(u)=sin(x^2)+C$$
### Why does this work? A basic explanation

Let's say we have a function $f(z)$, with $F(z)$ its antiderivative. By the chain rule we know that $F(g(x))=F'(g(x))\cdot g'(x)$ or by definition of $F$ $f(g(x))\cdot g'(x)$. So now we know that $$\int f(g(x))g'(x)dx=F(g(x))$$
Another way to see this:

$$ u=g(x), \text{ }\frac {du}{dx}=g'(x), \text{ } du=g'(x)dx $$

Why can we treat $u$ as a variable and a function at the same time? Smth to understand later, from Chat's explanation we "hide" x by using u, and we can treat it as a new variable that's dependent on the old variable x. not completely sure I buy it but whatev.

### Ejemplos

1 $$\int (8x-12)(4x^2-12x)^4dx$$
$$u=4x^2-12x \hspace{1cm} \frac{du}{dx}=8x-12\hspace{1cm}du=(8x-12)dx$$
$$\int (8x-12)(4x^2-12x)^4dx=\int u^4du=\frac{u^5}{5}+C=\frac{(4x^2-12x)^5}{5}+C$$
2
$$\int 90x^2sin(2+6x^3)dx$$
$$u=2+6x^3 \hspace{1cm} \frac{du}{dx}=18x^2\hspace{1cm}5du=90x^2dx$$
$$\int 90x^2sin(2+6x^3)dx=\int 5sin(u)du=-5cos(u)+C=$$