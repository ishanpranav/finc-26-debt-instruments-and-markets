# Coupon bonds and zeroes

## Discount factors

Let $d_t$ denote the price today of a 1-par, $t$-year zero-coupon bond.

## Law of one price

Let $P(c,T)$ represent the price of a $c$-coupon bond maturing in $T$ years with
semi-annual payments.

$$P(c,T)=\frac{c}{2}d_{0.5}+\frac{c}{2}d_1+\dots+\left(1+\frac{c}{2}\right)d_T.$$

$$P(c,T)=d_T+\frac{c}{2}\sum_{t=0}^{2T}{d_t}.$$

Here `A:A` contains the coupons, and `B:B` contains discount factors. This gives
the formula for `C100`, the coupon price:

```excel
=(A100/2)*SUM(B$1:B99)+(1+A100/2)*B100
```

## Price–yield relation

$$P(c,T)=\frac{c}{2}\left(1+\frac{y}{2}\right)^{-1}+\frac{c}{2}\left(1+\frac{y}{2}\right)^{-2}+\dots+\left(1+\frac{c}{2}\right)\left(1+\frac{y}{2}\right)^{-2T}.$$

$$P(c,T)=\left(1+\frac{y}{2}\right)^{-2T}+\frac{c}{2}\sum_{t=0}^{2T}{\left(1+\frac{y}{2}\right)^{-t}}.$$

## "Fundamental theorem"

Suppose a debt instrument pays fixed cash flows $C_1, C_2,\dots C_n$. at times
$t_1, t_2,\dots t_n$. This instrument is identitical to a portfolio of $C_1$
similar $t_1$-year zeroes, $C_2$ similar $t_2$-year zeroes, and so on (up to
$C_{n}$ similar $n$-year zeroes).

By the law of one price, the price $P$ of such an asset is given by:

$$P=\sum_{j=1}^{n}{K_jd_{t_j}}.$$

## Deriving zero prices from coupon bond prices

Let $d_T$ be the price of a $T$-year zero.

$$d_T=\frac{P(c,T)-\frac{c}{2}\sum_{t=0}^{T-0.5}{d_t}}{1+\frac{c}{2}}.$$

## Annual _vs._ semi-annual compounding

Let $r$ be the semi-annually compounded rate and $r_a$ be the annually
compounded rate.

$$\left(1+\frac{r}{2}\right)^2=1+r_A.$$

## Zero rates

The $t$-year zero rate $r_t$ is the discount rate such that $d_t$ is the present
value of \$1 to be received at time $t$.

$$d_t=\left(1+\frac{r_t}{2}\right)^{-2t}.$$

$$r_t=2\left(d_t^{-\frac{1}{2t}}-1\right).$$

Here `C1` contains the par value, `B:B` contains the zero rates, and `A:A`
contains the maturities. This gives for the formula for `D100`, the zero price:

```excel
=$C$1/(1+B100/2)^(2*A100)
```

Here `B:B` contains the zero price, `C1` contains the par value, and `A:A`
contains the maturities. This gives the formula for `D100`, the zero rate.

```excel
=2*((1/(B100/$C$1))^(1/(2*A100))-1)
```
