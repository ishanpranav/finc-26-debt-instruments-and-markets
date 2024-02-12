# Duration

The (modified) duration of a debt instrument is the *percent* change in its
price given a 100-basis-point (1-percentage-point) change in interest rate.

For example, a debt instrument with a duration of 7 will gain about 7 percent in
value if interest rates fall 100 basis points.

$D_{\text{mod}}\equiv-\frac{1}{V}\cdot\frac{\partial V}{\partial y}$

## Money duration

Let $D_{\$}$ represent the dollar-duration of a debt instrument with value $V$ and yield $y$.

$D_{\$}=-\frac{\partial V}{\partial y}\approx-\frac{\Delta V}{\Delta y}.$

Thus $\Delta V\approx-D_{\$}r$.

## Portfolio money duration

The money duration ${D_{\$}}_P$ of a portfolio $P$ is the the money duration
${D_{\$}}_i$ of each security $i$ in the portfolio.

Let $V_P$ be the value of the portfolio and $V_i$ be the value of each security $i$.

__Proof.__ $$V=\sum_{i\in P}{V_i},$$ $$\Delta V_P=\sum_{i\in P}{\Delta V_i},$$
$$\frac{\Delta V_P}{\Delta y}=\sum_{i\in P}{\frac{\Delta V_i}{\Delta y}},$$
$${D_{\$}}_P=\sum_{i \in P}{{D_{\$}}_i}.\,\square$$

## Portfolio duration

The duration $D$ of a portfolio $P$ with value $V_P$ is the value-weighted
average of the duration $D_i$ of each security $i$ with value $V_i$. 

Let $w_i$ be the weight of each security $i$ in the portfolio.

__Proof.__ $$D=\frac{{D_{\$}}_{P}}{V_P},$$
$$D=\frac{\sum_{i\in P}{{D_{\$}}_i}}{\sum_{i\in P}{V_i}},$$
$$D=\frac{\sum_{i\in P}{D_iV_i}}{\sum_{i\in P}{V_i}},$$
$$D=\frac{\sum_{i\in P}{D_iV_i}}{\sum_{i\in P}{V_i}},$$
$$D=\sum_{i\in P}{w_iD_i}.\,\square$$
