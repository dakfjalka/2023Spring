## Signal

is Carriers of information.

Information: to remove uncertainty.

## Mathematical model of signal.

## System

is what changes signal.

porcessing // interference

## types

- analog signal
- discrete-time signal
- digital signal : discrete time and amplitude

pulse signal?

## periodic signal

$$
x(t) = x(t + T)
$$

$$
x(n) = x(n + N)
$$

## Even/odd signal

$$
x(t) = x(-t)
$$

$$
x(t) = - x(-t)
$$

$$
x_{even}(t) = \frac{x(t) + x(-t)}{2}
$$

$$
x_{odd}(t) = \frac{x(t) - x(-t)}{2}
$$

$$
x(t) = x_{even}(t) + x_{odd}(t)
$$

## complex signal

$$
x(t) = x_r(t) + j x_i(t) = x_m(t) e^{j x_p(t)}
$$

$$
x^{*}(t) = x_r(t) - j x_i(t) = x_m(t) e^{- j x_\rho(t)}
$$

$$
x_r(t) = \frac{x(t) + x^{*}(t)}{2}
$$

$$
x_i(t) = \frac{x(t) - x^{*}(t)}{2j}
$$

$$
x_m(t) = \sqrt{x^2_r(t) + x^2_i(t)}
$$

$$
x_\rho(t) = \arctan\frac{x_i(t)}{x_r(t)}
$$

## 10 basics signals

1. unit step

$$
\begin{aligned}
u(t) = \begin{cases}
    1&,t>0\\
    \frac{1}{2}&, t=0\\
    0&, t<0
\end{cases}
\end{aligned}
$$

$$
\begin{aligned}
u(n) = \begin{cases}
    1&,t\ge0\\
    0&, t<0
\end{cases}
\end{aligned}
$$

attention: CT $u(0) = 1/2$ , &emsp; DT $u(0)=1$

2. gate

$$
\begin{aligned}
    \Pi(t) = \begin{cases}
        1&|t|<\frac{1}{2}\\
        \frac{1}{2}&|t|=\frac{1}{2}\\
        0&|t|>\frac{1}{2}
    \end{cases}
\end{aligned}
$$

$$
\begin{aligned}
    \Pi_N(n) = \begin{cases}
        1&|n|\le N\\
        0&|n|> N
    \end{cases}
\end{aligned}
$$

relation with unit step signal:

$$
\Pi(t) = u\left(t + \frac{1}{2}\right) - u\left(t - \frac{1}{2}\right)
$$
