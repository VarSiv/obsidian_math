### Formula:
$$\int u(x)\cdot v'(x)dx=u(x)\cdot v(x) - \int u'(x) \cdot v(x)dx$$ In its definite form: 
$$\int_a^b u(x)\cdot v'(x)dx=u(x)\cdot v(x)\Bigg\vert_a^b - \int_a^b u'(x) \cdot v(x)dx$$
Derivation:
$$\Big(u(x)\cdot v(x)\Big)'=u'(x)\cdot v(x)+u(x)\cdot v'(x)$$
$$\int\Big(u(x)\cdot v(x)\Big)'dx=\int u'(x)\cdot v(x)dx+\int u(x)\cdot v'(x)dx$$
Sidetrack: cuando podemos derivar/integrar etc de ambos lados? como se que es una operacion bien definida? Explicacion: Se que la primera linea es una igualdad de funciones (por props basicas de la derivada) que vale para todo x. Entonces cuando integramos ambos lados las antiderivadas son iguales hasta una constante, y por como es la familia de funciones esto es igualdad (tiene q ver q estan en la misma clase de equivalencia!!).  

Formulacion alternativa: Pensamos $u'(x)=\frac{du}{dx}$ como $du=u'(x)dx$ y $v'(x)=\frac{dv}{dx}$ como $dv=v'(x)dx$. Usando $$\int u(x)\cdot v'(x)dx=u(x)\cdot v(x) - \int u'(x) \cdot v(x)dx$$

Reemplazamos y nos queda
$$\int u(x)dv=u(x)\cdot v(x) - \int v(x)du$$
### Logica

You have your original function $f$,  and you want to break it down into $f=u(x)\cdot v'(x)$ in such a way that $u'(x)\cdot v(x)$ is easy to integrate. The "rules" for choosing $u$ (which I don't like): LIATE

Logarithmic
Inverse trigonometric ($\arctan , \arcsin$), etc
Algebraic (polynomials ig?)
Trigonometric
Exponential
### Ejemplos

1
$$\int x\cdot e^xdx$$
$$u(x)=x \text{ } v'(x)=e^x$$
$$\int x\cdot e^xdx=x\cdot e^x-\int 1\cdot e^xdx=x\cdot e^x-e^x+C $$

2
$$\int x\cdot ln(x)dx$$
$$u(x)=ln(x) \text{ } v'(x)=x$$
$$\int x\cdot ln(x)dx=ln(x)\cdot \frac{x^2}{2}-\int \frac{x^2}{2}\cdot \frac{1}{x}dx=ln(x)\cdot \frac{x^2}{2}-\frac{x^2}{4}+C$$

3
$$\int x\cdot sin(x)dx$$
$$u(x)=x \text{ } v'(x)=sin(x)$$
$$\int x\cdot sin(x)dx=-x\cdot cos(x)-\int -cos(x)dx=-x\cdot cos(x)+sin(x)+C$$
4 A more interesting example.
$$\int e^xcos(x)dx$$
$$u(x)=cos(x) \text{ } v'(x)=e^x$$
$$\int e^xcos(x)dx=e^xcos(x)-\int -e^xsin(x)dx=e^xcos(x)+\int e^xsin(x)dx$$
Find the new integral with $sin$ by using parts
$$\int e^xsin(x)dx=e^xsin(x)-\int e^xcos(x)dx$$
Substitute back in 
$$\int e^xcos(x)dx=e^xcos(x)+e^xsin(x)-\int e^xcos(x)dx$$
Now its easy to see that
$$\int e^xcos(x)dx=\frac{e^x\Big(cos(x)+sin(x)\Big)}{2}+C$$
5 One that also uses substitution
$$\int arctan(x)dx$$
$$u=arctan(x) \text{ }v'=1$$
$$u'=\frac {1}{x^2+1} \text{ }v=x$$
$$\int arctan(x)dx=arctan(x)\cdot x-\int \frac {x}{x^2+1}dx$$
Now we use substitution $u=x^2+1$ $du=2xdx$ $\frac {1}{2}du=xdx$ 
$$\int arctan(x)dx=arctan(x)\cdot x-\int \frac{1}{2u}du=arctan(x)\cdot x-\fra{}{}$$