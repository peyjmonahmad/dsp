[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>> 
import random

x = []
for i in range(1000):
    i = random.random()
    x.append(i) 

rand_pmf = thinkstats2.Pmf(x)
rand_cdf = thinkstats2.Cdf(x)

thinkplot.Pmf(rand_pmf)
thinkplot.show(xlabel='numbers',ylabel='pmf')

thinkplot.Cdf(rand_cdf)
thinkplot.show(xlabel='numbers',ylabel='cdf')

Yes, the distribution is uniform.  Which can be seen from both of these plots.

