# Part Two
**Measures of interest rate risk and hedging**
**IR risk** of a security is measured by how much its price changes as interest rates change.
We need to know under different IR changing scenario, how our Portfolio will change.
Two types of formulations to model to model the changing of IR:
1. One-factor model:
   *Assumption*  changes in the rates for different terms are fully determined by the change in a single IR factor, the 10-year par rate.
2. Multi-factor model: use two or more factors, e.g. two-factor approach: level factor + slope factor => description of term structure movement

# One-factor Risk Metrics and hedges
Main concepts: DV01, duration and convexity
## DV01
P(y), the price-rate function , y is an IR factor.
DV01 = - dP/(dy/0.01%), DVO1 is an acronym for dollar value of an 01 (i.e. of .01%). The minus sign is used to make sure that we always have a positive DV01
**Attention** Most market participants use DV01 to mean yield-based DV01. Yield-based DV01 assumes that the yield-to-maturity of a particular security changes by one bps. To avoid confusion, some market participants have different names for DV01 measures according to the assumed change in rates.

## A Hedging application: A futures option
Say a market maker has sold the option TYU0C 120 and he will stand to lose money if rates fall, purchasing futures can hedge the resulting exposure.  The DV01 of the two securities can be used to figure out exactly how many futures should be bought against the short option position.
We want to have a match of DV01 for two portfolios.
F1*DV01_1 = F2*DV01_2
There are securities for which DV01 is negative, most notably in mort- gage derivatives.
In reality, the market maker would sell the options at some premium to their fair value。

## Duration
Duration measures the percentage change in the value of a security for a unit change in rates.
D= -1/p*dp/dy .

## Convexity
As interest rate sensitivity changes with the level of rates, we use convexity to measure this sensitivity.
C = 1/p*d^2p/dy^2 which is related to the second order derivative of the price-rate function.

## Hedging example
Duration hedging is local that is valid in a particular neighbourhood of rates. As rates move, the quality of the hedge deteriorates.
Short convexity: the hedged position loses whether rates rises or fall because the option is more convex than the bond
A long convexity is long volatility while a short convexity position is short volatility.
![Image of Yaktocat](https://github.com/ShanCheng1994/Book_Note/tree/master/Fixed_Income_Tuckman/fig/test.png)
