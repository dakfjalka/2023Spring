## 简单方程求解

### e.g.1 设 $u=u(x,y)$ 为 $x, y$ 的二元函数，求解 $u_x=f(x)$

> $$ u(x, y)=\int f(x)dx $$
> 
> let $F^\prime(x) = f(x)$
>
> $$ u(x, y) = F(x) + C(y) $$
>

### e.g.2 $u=u(t,x)$ , $u_t = au_x$ , $a\in\R$（一维一阶线性波动方程）

> 特解： $\phi(t,x) = x + at$
>
> 令$G(\xi)$ 为 $\xi$ 连续可微函数，$u(x,t) = G(x+at)$
>
> $$ u_t = aG^\prime(x+at) = au_x$$
>
> 故 $u(x,t)=G(x+at)$ 是原方程的一般解.
>

### e.g.3 $u=u(x,y)$, $u_{x,y} = 0$

> $u_{xy}=0\Rightarrow u_x=f(x)\Rightarrow u(x,y)=F(x) + G(y)$
>
> 这里 $F(x), G(x)$ 都为可微函数

### e.g.4 $u=u(t,x)$ , $u_{tt}=a^2u_{xx}, a>0$

> 做变换
> 
> $$ \begin{cases}\xi=x+at\\ \eta=x-at\end{cases} $$
>
> $$ \begin{aligned}u_t&=u_\xi\frac{\partial\xi}{\partial t}+u_\eta\frac{\partial\eta}{\partial t}\\ &=a u_\xi-au_\eta\end{aligned}$$
>
> $$ u_{tt}=a^2(u_{\xi\xi}-2u_{\xi\eta}+u_{\eta\eta}) $$
>
> $$ u_{xx}= u_{\xi\xi}+2u_{\xi\eta}+u_{\eta\eta}$$
>
> 代入方程得到
>
> $$ u_{\xi\eta}=0$$
>
> 由 e.g.3 得
> 
> $$u(x,t)=u(\xi,\eta)=F(\xi)+G(\eta)=F(x+at)+G(x-at)$$

---

$$
\int_\R u(t,x)dx=1 \forall t>0
$$

$$
\lim\limits_{t\to 0}u(t, x)\ \ \text{when}\ x=\xi
$$