Antiderivatives are the inverses of derivatives. Let's have $f(x)$ and $F(x)$  the function of the area bounded by $f$ from $a$ to $b$. I will show that $F'(x)=f(x)$ . Let $c \in (a,b)$ . We know that $F(c)=k$ for some $k$ , and $F(c+dx) = F(c)+f(c)*dx$ (intuicion de los rectangulitos cuya base tiende a 0). Despejando, $F(c+dx)-F(c) = f(c)*dx$ , $\frac {dF} {dx} = f(c) \Box$. 

### Fundamental theorem of calculus 

$$\int_a^b{f(x)dx}=F(b)-F(a)$$ Por definicion $F$ es la antiderivada de $f$,  y ya vimos que $F$ es el area de la curva de su derivada. Veamos el TFC de una forma intuitiva. Por la linealidad de la integral, $\int_a^b{f(x)dx}=\int_0^b{f(x)dx}-\int_0^a{f(x)dx}$ . Por la definicion de $F$, que es $F(x)=\int_0^x f(x)dx$ esto equivale a decir $F(b)-F(a)$ . La logica menos circular. Pero tiene mucho sentido, si sabes calcular el area entre 0 y un numero arbitrario, el area de $a$ a $b$ es lo acumulado hasta $b$ menos lo acumulado hasta $a$.

### Uniqueness of antiderivative up to the constant

$\textbf{Theorem}: \text{If } F' = f$ and $G' = f$  (F and G both antiderivatives of f then $F=G+C$ (they only differ by a constant.

$\textbf{Proof}: (F-G)' = F'-G' = f-f =0$  Since the derivative of $F - G$ is 0, that new function must be a constant.

### Basic application

Finding $F$ based on $f$ and a single value of $F$. Simple case: we know $F(0) = k$ . Then $F(t)$, for $t>0$ is $$F(t) = \int_0^t{f(t)dt} + F(0)$$
Why? Because what we want to find is $F$, which is the area under a curve of $f$, which we know. To calculate the change of the area we can use $\int_0^t{f(t)dt}$ as previously established. By TFC $\int_0^t{f(t)dt} = F(t)-F(0)$ . To get $F(t)$ back we simply add back $F(0)$.

Generalizing, if we know $F(k)$ for some $k>0$ , by the earlier formula we know that $$F(k) = \int_0^k{f(t)dt} + F(0)$$
Here we know everything except $F(0)$, which we can find. From there, we get a general formula for $F(t)$. 

#### Does this make sense for k<0?

There is an intuive and easy way to apply the former to different real world scenarios with time/velocity. Negative time doesn't make any sense, but is there any reasonable meaning behind using $t<0$? $$\int_b^a{f(x)dx}=F(a)-F(b)$$
 $$\int_a^b{f(x)dx}=F(b)-F(a)$$
 $$\int_b^a{f(x)dx} = -\int_a^b{f(x)dx} $$
 Por simplicidad sea $t>0$, quiero $F(-t)$ 
$$F(-t) = \int_0^{-t}{f(t)dt} + F(0)= -\int_{-t}^{0}{f(t)dt} + F(0)$$ Y ahora esto si tiene la forma de una integral normal. Tiene una interpretacion coherente? Sea $t=1, -t=-1$ y $F(0)=3$ La integral normal $\int_0^{-1}{f(t)dt = 1}$. Entonces en el momento "-1" $F$ valia un cierto valor $x$ y en $F(0)$ valia 3. En ese intervalo ascendio por 1. El resultado logico es que $F(-1)=-1+3=2$. Asi, podemos generalizar $F(k) = \int_0^k{f(t)dt} + F(0)$ para todos los reales, y en caso de negativos es como "contar para atras".

## Metodos de integracion

[[Integration by Parts]]

