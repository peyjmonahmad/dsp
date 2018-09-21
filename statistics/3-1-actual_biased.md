[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>> 
resp = nsfg.ReadFemResp()
pmf = thinkstats2.Pmf(resp.numkdhh,label='numkdhh')

def BiasPmf(pmf, label):

    new_pmf = pmf.Copy(label=label)
    
    for x,p in pmf.Items():
        new_pmf.Mult(x,x)
    
    new_pmf.Normalize()
    return new_pmf

observed = BiasPmf(pmf,label='biased')

thinkplot.Pmfs([pmf,observed])

thinkplot.Config(xlabel='Class size',ylabel='PMF')

thinkplot.show()

/Users/peyjmonahmad/Desktop/Screen\ Shot\ 2018-09-20\ at\ 5.46.32\ PM.png 