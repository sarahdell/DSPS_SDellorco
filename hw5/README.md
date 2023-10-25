I worked on this homework discussing it with Masooma, Rayta, Paula, Miles and Christian. I also discussed it with Willow over slack and at her office hours.

This homework discusses various ways to create fits. We discuss normal linear fits, machine learning linear fits, using different likelihood functions (L1, L2, Chi-Squared), 
stochastic gradient descent method, and MCMC. We used these methods for a linear regression model and a broken power law model. In Part 4, we discuss AIC and BIC model 
comparison, in which we compared the linear and broken power law models. Using the AIC and BIC values, I found that the linear model was a better fit since the linear AIC 
and BIC values were smaller than the broken power law AIC and BIC values. We also tested which model was a better function using the likelihood ratio test. The null 
hypothesis of this test is that the simpler model (in this case the linear model) is a better fit for the data. Using a threshold of 0.05, we got a p-value larger than the 
threshold, meaning we fail to reject the null hypothesis, and it is inconclusive whether the linear or broken power law regression is a better fit for the data. 

The hardest part was Part 3, which was generating the fits for the broken power law model using stochastic gradient descent and MCMC. There were a lot of small things that
could go wrong with that code that would ruin all the results, so problem-shooting when something was off really took a long time because you had to go through it with a
fine-toothed comb.

The easiest part of this homework was Part 2, which was interpreting the outputs from Dr. Bianco’s code. I still feel more confident in doing the statistics parts of these
assignments than I do the coding parts, so it was nice to have a section where it was mostly interpreting graphs rather than coding problems.

In this homework, a new thing I learned was about AIC and BIC. We hadn’t talked about it in class, so I had to learn it through the provided slides while doing Part 4.
