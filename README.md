
# Statistical Distributions and Use cases in Data Analysis



Data scientists have to choose probability distributions routinely and decide which one us for an analytics experiment. Probability distributions are like building blocks for statistical analysis, just like data structures are to computer programming. There are literally thousands of distributions to study, most of them may not be very common though. In the upcoming series of lessons, we shall look at some key distributions that you might come across with.

![](dists1.jpg)
## Objectives:

* Understand the concept of statistical distributions
* Differentiate between discrete and continuous distributions
* Understand commonly used distributions and their use cases




### So What is a "Statistical Distribution" ?

The statistical distribution of a given set of data set is a listing or **function** showing all the possible values of the data and how often they occur. 

For example, when a categorical distribution of data is organized, we can get , say the number or percentage of individuals in each group. When a distribution of numerical data is organized, we can show it as graphs and charts to examine the shape, center, and amount of spread in the data as we saw in measures in center and spread lessons. Based on the variation of their attributes, data distributions can take many shapes and forms. Below, we shall look into some popular distributions and learn how to distinguish between them visually. 

As an example, recall the Bernoulli distribution that we saw in previous section. Flipping a fair coin has two outcomes, heads or tails. Before the flip, we believe there is a 1 in 2 chance, or 0.5 probability, of heads and tails. That’s a probability distribution over the two outcomes of the flip. If you can follow this notion, you already know the Bernoulli distribution.  

### Common Distributions

Bernoulli is the most basic distribution and a number of other, slightly more complex distributions evolve from Bernoulli as shown in the diagram below:

![](dists.png)

These distributions are described using their Probability density function (PDF).The horizontal axis in each chart is set of possible numeric outcomes. The vertical axis describes the probability of outcomes. 


### Discrete Distributions

Some distributions are discrete i.e. their outcomes must be integers like 2 or 6 (think of age in terms of years). These distributions show outcomes as **sparse** lines  (space between them), and the line height is the probability of that outcome as shown in the chart above. 

#### Binomial/Bernoulli

Binomial/Bernoulli distributions are examples of discrete distributions. The uniform distribution shown above with a flat probability of outcomes (all options are equally poissble) is another another common discrete distribution. Imagine rolling a fair dice. The outcomes 1 to 6 are equally likely. Such a distribution can be defined for any number of outcomes and hence is a discrete distribution. 

In conducting a political opinion poll, choosing a voter at random to ascertain whether that voter will vote "yes" in an upcoming referendum is also an example of Bernoulli distribution. 


#### Poisson
What about the count of visitors visiting a company website each minute? 

You could think of this as a binomial distribution with each second as a Bernoulli trial in which a customer calls or doesnt (1 or 0). However, as the company company knows, when the site goes down, 10 or even a thousand people can call in at exactly the same second.  One way around this would be to reduce the trial size from one second to say, 100th of a second. O, if it still doesnt solve the problem, we would need even smaller time segments. We can take this approach to infinitely small time intervals in which the probability of a call is infinitesimal. The limiting result is the Poisson distribution.

The Poisson distribution is what you must think of when trying to count events over a time given the continuous rate of events occurring. When things like visitors arriving on a website, or customers arrive at a store, or clients waiting to be served in some kind of queue, think **“Poisson”**.

#### Geometric
Geometric distribution arises from simple Bernoulli trials. You would consider this when asking questions like "How many times does a flipped coin come up tails before it first comes up heads?". The count of tails follows a geometric distribution. Like the Bernoulli distribution, it’s parameterized by p only, because the number of failure trials is the n outcome itself.

So if the binomial distribution answers “ How many successes?”, the geometric distribution is “How many failures until I succeed?” OR "How many visitors visist our website before a product is sold"?. "How many emails we send out before we get a customer response" etc. 

### Continuous Distributions

A continuous distribution describes the probabilities of the possible values of a **continuous** random variable.  Probabilities of continuous random variables are defined as the area under the curve of its PDF. Thus, only ranges of values can have a nonzero probability. The probability that a continuous random variable equals some value is always zero. 

#### The Normal or Gaussian distribution, 

A normal distribution is the single most important distribution for data analysis. Its bell shape is instantly recognizable as seen in the diagram above. A normal distribution turns up very often while dealing with real world data. 

If we take values and sum them, the distribution of their sum follows the normal distribution. The more things that are summed, the more their sum’s distribution matches the normal distribution. This is known as Central Limit Theorem and we shall go through this in detail in later parts of the course. In this sense, A normal distribution relates to all other distributions. e.g., the sum of Bernoulli trials follows a binomial distribution, and as the number of trials increases, that binomial distribution becomes more like the normal distribution.

Normal distributions are used to describe many real world datasets that follow "normality" including heights, weights of different people, errors in some measurement, marks in a test etc. 

---

#### So is that all about distributions ??

The phenomena of statistical distributions carries a lot more depth and detail. This lesson gives you an initial introduction to different distributions. The significance and applications of these distributions will come with time as we proceed with analytics activities. For now, we shall carry on looking at the normal distribution in more detail in the upcoming lessons. Other distributions will be covered in detail in the statistics section later in the course. To conclude, how about a paranormal distribution .

<img src="https://i.redd.it/1ocin3p925zz.jpg" width = 300>


## Summary

In this lesson, we built on intuition for Bernoulli/Binomial distribution and introduced some new discrete and continuous distributions. We also saw some simple applications of these distributions while answering an analytical question. The normal distribution and its detailed description is coming ahead. 
