# Conditional sign changes at dilation three halves

Assume RH and rational linear independence of the distinct positive ordinates of the nontrivial zeta zeros. At $b=3/2$ the ordinary-prime deficit takes both signs arbitrarily far out.

Let $W_b(t)$ equal $b(1-1/t)$ for $1<t\le b$, $b^2/t-1$ for $b<t<b^2$, and zero elsewhere. Define $P_b(y)=\sum_{p\ {\rm prime}}(\log p)W_b(p/y)$ for $y>0$, with natural logarithms. Its expected main term is $b(b-1)y\log b$. Write $B_b=2\sqrt b(\sqrt b-1)^2$ for the asymptotic prime-square contribution, $D_b(y)=b(b-1)y\log b-P_b(y)$ for the deficit and $H_b(s)=(b^s-1)(b^s-b)/(s(s-1))$ for the Mellin transform.

The general extremal formula gives $\limsup D_b(y)/\sqrt y=B_b+L_b$ under RH and $\liminf D_b(y)/\sqrt y=B_b-L_b$ with the additional independence hypothesis, where $L_b=\sum_\rho|H_b(\rho)|$ is the sum of the absolute zero coefficients. The executable proves $B_b-L_b<-0.0015$ and $B_b+L_b>0$ at $b=3/2$. Both signs therefore occur beyond every finite bound. Under RH alone this argument gives a lower bound of negative sign, which leaves the occurrence of negative values open. [Derivation of the general extremal formula](https://github.com/leecrossley/prime-band-extrema/tree/v1.0.0)

## Verification

The written phase argument uses Kronecker's theorem for the negative extremum. The executable checks the signs of the two constants. Finding an explicit negative value remains open here.

The recorded run used Python 3.9.6 on arm64 macOS. The verifier requires Python 3.9 or later and uses only the standard library.

```sh
bash verify-release.sh
```

The command checks the release manifest, reruns the arithmetic, and compares its output with the recorded result.

[Recorded verification output](evidence/check.txt) · [SHA-256 manifest](SHA256SUMS) · [Tagged publication](https://github.com/leecrossley/prime-band-three-halves-oscillation/releases/tag/v1.0.0)

## Related result

[Finite certificate at the same dilation](https://github.com/leecrossley/prime-band-three-halves-finite/tree/v1.0.0)
