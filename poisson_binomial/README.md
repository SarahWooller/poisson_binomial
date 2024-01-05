# Poisson Binomial


The Poisson binomial distribution is the discrete probability distribution of a sum of independent Bernoulli trials that are not necessarily identically distributed. That is, it is the number of successes in a sequence of n independent yes/no experiments where the success probabilities vary.

The package contains a single class PoissonBinomial.

Parameters: p : array-like
			the probabilities of success for each of the Bernouilli trials

Attributes: pmf : array-like	probability mass function
			the probability of n successes where 0<=n<=len(p)
cdf			:	array-like, 	cumulative distribution function
			the probability of n or less successes where 0<=n<=len(p)


Methods: 

x_or_less(x) :	float,		probability of achieving x or less successes  
x_or_more(x) :	float,		probability of achieving x or more successes

The class PoissonBinomial implements a closed-form expression for the cdf of the Poisson binomial distribution,derived in "On computing the distribution function for the Poisson binomial distribution" by Yili Hong (2013).

The approach is based on finding the discrete fourier transform function for the characteristic function (CF) for the Poisson binomial distribution.

