[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

>> first = live[live.birthord == 1]
others = live[live.birthord != 1]

first_weight = first.totalwgt_lb
others_weight = others.totalwgt_lb

import math

def CohenEffectSize(group1, group2):
    diff = group1.mean() - group2.mean()
    
    var1 = group1.var()
    var2 = group2.var()
    n1,n2 = len(group1),len(group2)
    
    pooled_var = (n1 * var1 + n2 * var2)/(n1 + n2)
    d = diff/ math.sqrt(pooled_var)
    return d

CohenEffectSize(others_weight,first_weight)

Cohen's D difference between groups = 0.088672927072602

Using Cohen's d for the weight of first babies compared to other babies, the differencce in means is about 0.089 standard deviations.  This difference is about 3x greater than the difference in preganancy length.  Overall, it is tough to tell if it is a signficant difference, but it is certainly more signficant than the preganany length difference."
