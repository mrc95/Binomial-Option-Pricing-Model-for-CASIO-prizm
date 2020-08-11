# Binomial-Option-Pricing-Model-for-CASIO-prizm
These files allows you to easily determinate american and european options price using your CASIO prizm on spreadsheet mode.  Copy and past them in the main memory directory —> SSHEET. 
— For any inquires please contact me at m.lingua95@gmail.com —


The binomial approach is a discrete valuation model for European/American options on derivative securities, it was first suggested by William Sharpe in 1978. However, this methodology is normally associated with the paper by John Cox, Stephen Ross, and Mark Rubinstein in 1979.  This method divides the time until option maturity into discrete intervals and presumes that, during each of these intervals, the price of the asset - e.g., the stock - follows a binomial process moving from its initial value. These files allows to calculate the option price by simply using few parameters as inputs:

- strike = strike price of the option
- S(0) = current underlying price / value (at t=0)
- risk free interest rate
- sigma = volatility of S
- delta T = is calculated as the option maturity expressed as a year fraction and divided by the number of intervals of the lattice (eg 5 months using 4 intervals = 5/12/4 = 0,4166/4 = 0,10416)
- div = dividend amount
- div date = dividend date, expressed in the same way as delta T
- VA div = present value of the dividend (at t=0)
- external int rate (ATTENTION: default is set to 0, just change it if working with dividend yields currency pairs or futures. For stocks known dividend yield, set the external int rate = dividend yield; for currency pairs it indicates the external currency risk free int rate; if working with futures input the same value of the risk-free interest rate (see the model formulas)).

The following parameters will be automatically calculated by the spreadsheet and shouldn’t be filled:
- u is the up parameter
- d is the down parameter
- p is the risk neutral probability

When working with stocks which pay dividends, the stochastic tree has to be filled with the present value (calculated at any node) of the dividend. Otherwise, fill it with 0 for every cell. 
Scrolling down you will be able to see the stochastic, deterministic, stochastic and deterministic tree, the option value tree with early exercise on any node and the European and american option value calculated for 3 different time intervals (3, 4 and 5 but it Can be extended with smaller/bigger timeframes).
