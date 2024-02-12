# Yield to maturity

## Definition of yield

Suppose an asset has price $P$ and positive fixed cash flows $C_1,C_2,\dots C_n$
at times $t_1,t_2,\dots t_n$. Its yield to maturity is the single discount rate
$y$ that makes the present value of the cash flows equal to $P$:

$$\frac{C_1}{\left(1+\frac{y}{2}\right)^{2t_1}}+\frac{C_2}{\left(1+\frac{y}{2}\right)^{2t_2}}+\dots\frac{C_n}{\left(1+\frac{y}{2}\right)^{2t_n}}=P.$$

## The coupon effect

**Proposition 1:** If the yield curve is not flat, then bonds with the same
maturity but different coupons will have different yield.

**Proposition 2:** If the yield curve is upward-sloping, then for any given
maturity, higher coupon bonds will have lower yields.

**Proposition 3:** If the yield curve is downward-sloping, then for any given
maturity, higher coupon bonds will have higher yields.

## Annuity formula

This formula gives the present value $P$ of an annuity of \$1 to be received for
$T$ years (or $2T$ semesters) at a annualized percentage rate $y$ (or $y/2$
semiannual rate).

$$P=\sum_{t=1}^{2T}{\left(1+\frac{y}{2}\right)}^{-t}=\frac{2}{y}\left(1-\frac{1}{(1+\frac{y}{2})^{2T}}\right).$$

## Closed-form yield-to-price formula

The closed-form formula gives the price $P$ of a 1-par $c$-coupon bond maturing
in $T$ years with yield-to-maturity $y$.

$$P(c,T)=\frac{c}{y}\left(1-\frac{1}{(1+\frac{y}{2})^{2T}}\right)+\frac{1}{(1+\frac{y}{2})^{2T}}.$$

- If $c=y$, then $P=1$, and this is par bond.

- If $c>y$, then $P>1$, and the bond is priced at a premium.

- If $c<y$, then $P<1$, and the bond is priced at a discount.

## Par rates

The par rate is the is the coupon rate that sets the price equal to par.

$$\frac{c_T}{2}d_{0.5}+\frac{c_T}{2}d_1+\dots+1d_T=1.$$

$$c_T=\frac{2(1-d_T)}{d_{0.5}+d_1+\dots+d_T}.$$
