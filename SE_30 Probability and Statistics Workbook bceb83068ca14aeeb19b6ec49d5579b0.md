# SE_30 Probability and Statistics Workbook

Link to Portfolio: [https://alexanderkuebel.notion.site/SE_30-Probability-and-Statistics-Workbook-67901e3b7a684427bc75c05960f661e0]()

# Introduction

Confronting decision making in all areas of life, we have to make decisions in the present but there are unknown and uncertain future outcomes. So, whether we like uncertainty or not, we're stuck with it. The bad side about uncertainty is that it's a real pain for decision-making because we don't know for sure what's going to happen. Probability and statistics will allow us to quantify uncertainty and hopefully assist us in our decision-making.

## The Monty Hall Problem

Suppose you're on a game show, and you're given the choice of three doors: Behind one door is a car; behind the others, goats. You pick a door, say No. 1, and the host, who knows what's behind the doors, opens another door, say No. 3, which has a goat. He then says to you, "Do you want to pick door No. 2?" Is it to your advantage to switch your choice?

[Solving the Monty Hall Problem with bayesian updating]()

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Monty_open_door.svg.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Monty_open_door.svg.png)

Fig. 1: Monty open door. (2006). [Illustration]. [https://commons.wikimedia.org/wiki/File:Monty_open_door.svg](https://commons.wikimedia.org/wiki/File:Monty_open_door.svg)

## Decision Making Under Uncertainty

If we played this game multiple times, then as an optimal strategy it would always pay to switch door. Because in the long run, by having the strategy of switching, you would be winning on average twice as often as if you stuck with your original choice. So I don't promise you success in your decision making every single time. Uncertainty exists, and we can never know for sure what's going to happen in the future. So the best we can do is form our expectations of the future. Unfortunately, we have this inherent uncertainty we have to deal with. And, indeed, bad luck can affect all of us. But so, too, can good luck. But if we do play to the probabilities, we won't succeed always, but we can be confident that we will win far more often than we lose.

**Examples for decision making under uncertainty:**

- Study or not to study to increase the expectations for a good job offer
- marry or not to marry the partner
- invest or not to invest into the stock

These, among others, are decisions many of us face during our lives. Of course, decisions have to be taken in the present, with uncertain future outcomes.

**Nowadays, in the age of technology, we face two important implications for our decision making:**

1. Technology has made it possible to collect vast amounts of data – the era of big data
2. Technology has given many more people the power and responsibility to analyse data and make decisions on the basis of quantitative analysis

**Many institutions, companies are embracing data-driven decision-making as a source of competitive advantage.**

Decision-making is a process when one is faced with a problem or decision having
more than one possible outcome.

The reasonable outcomes from the decision are a function of both internal variables (which we can control) and external variables (which we cannot control), each of which cannot be expressed with certainty. Hence the outcome cannot be known in advance with certainty.

**For all decisions, we need to determine the influencing factors which could either be internal or external, such as...**

- demand and competitive supply
- availability of labour and materials

...**which are then used to derive expected results.** 

When evaluating all decision-making, we start with structuring the problem. Determine the possible criteria which could be used to evaluate the alternatives:

- qualitative analysis → E.g.:  Well, last time we brought a new product to the market, we priced it at £2 and we sold out on the first day. This time let’s price it higher.

    In a qualitative analysis, once we have determined a preliminary list of the factors which we think will affect the possible outcomes of the decision:

    - the management team ‘qualitatively’ evaluates how each factor could affect the decision
    - this discussion leads to an assessment by the decision-maker
    - the decision is made followed by implementation, if necessary

    a qualitative approach normally is susceptible to judgement and hence biases on the part of the decision-makers. ‘Gut instinct’ can lead to good outcomes, but in the long run is far from optimal.

- quantitative analysis → E.g.: What do we know about current market demand?

    once we have determined a preliminary list of the factors which we think will affect the possible outcomes of the decision, we need to ask the following questions:

    - What do we know?
    - How can we mine data that will help us analyze the factors and their effects each will have on the possible outcomes?

    In a quantitative analysis, the evaluation becomes a process of using mathematics and statistical techniques. These are used to find predictive relationships between the factors, the potential outcomes of the problem we are seeking to understand and the decision we are seeking to make.

    Our objective becomes to define mathematically the relationships which might exist. Next, we evaluate the significance of the predictive value of the relationships found.

## Uncertainty in the news

‘News’ is not ‘olds’. News reports new information about events taking place in the world – ignoring fake news!  Decisions are made in the present, with uncertain future outcomes. Hence many media reports will comment on the uncertainties being faced. Nowadays the black swan – low-probability, high-impact events influences our life and are important to consider for a decision making.

What I would ask myself, especially regards the black swan events, how much of the gathered data for predicting was collected in a quantitative, reliable way. So is it more, that we are not able to collect the data appropriately or is it more that this low probability events really hits us?

## Simplicity vs. Complexity - The need of models

Although we care about the real world, seek to understand it and make decisions in reality, we have an inherent dislike of complexity. Indeed, in the social sciences the real world is a highly complex web of interdependencies between countless variables.

So in order to make any sense of the real world, we will inevitably have to simplify reality. Our tool for achieving this is a model.

A model is a deliberate simplification of reality. A good model retains the most important features of reality and ignores less important details. (similar to unsupervised learning models in ML) That results into a trade-off - the benefit of simplifying a model from the complex real world, facing the consequence of it's simplification of reality. In the example, the benefit has to exceed the cost. Both, the costs and the benefits are very subjective regards our application area.

An Example would be an underground map of a city. A tourist who wants to travel from A to B has completely different expectations compared to the an engineer, that maintains the underground railway. 

Resolving this benefit–cost trade-off is subjective – further adding to life’s complexities.

## Safe to Assume?

Model → is this deliberate simplification of reality

Assumption, usually simplifying assumptions → beware assumptions we are having in mind while creating our model.

If you make a wrong or invalid assumption, then decisions you make in good faith may lead to outcomes far from what you expected.

The output of our models are only as good as the model itself, which includes the assumptions we attached to them.

In statistical models, we often make distributional assumptions, i.e. we assume a particular probability distribution (a concept introduced next week) for a particular variable.

# Quantifying Uncertainty With Probability

## Definitions

Experiments: random experiment which could lead to one **of several possible outcomes.** 

Outcome: result of the experiment

Sample space: **set of all possible** outcomes in an experiment. $S=\{\ldots\}$, with all the possible outcome in the curly brackets. E.g. rolling a dice 🎲 → $S=\{1,2,3,4,5,6\}$

Event or subset of the sample space: an Event which is of interest to us. E.g., we win if we roll a 6 → $A=\{6\}$.

probability: how likely a particular event is to occur. All probabilities are some value over the unit interval = $[0,1]$ or more formal $0 \leq P(A) \leq 1$. (Multiplying by 100 yields a probability as a percentage) Where ${P(A)=0}$ indicates an impossible event and ${P(A)=1}$ indicates a certain events. The probability of an occurring event from the sample space  $P({S})=1$. Because one of the options for sure will occur, so that statement is certain.

**How are probabilities assigned to the occurrence of subsets of the sample space?**

- subjectively → Subjective estimates are employed when it is not feasible to conduct experimentation or use theoretical tools. Doomsday Clock, very hard to quantify the probability.
- experimentation → conducting an experiment a very large number of times is resulting in the probability of that particular event → toss a coin extremely often
- theoretically

## Simple Probability Distributions

First we will consider the special case, where each of these outcomes is equally likely and the sample space contains only a finite number of outcomes.

$\mathbf{N}$  = possible outcomes, for rolling the dice → $\mathbf{N=6}$. $\mathbf{n}$ corresponds to the number of events / outcomes that fulfill the event of interest happening. The probability of this event is reflected by $\mathbf{\frac{n}{N}}$. More formaly:

$$P(A)=\frac{n}{N}=\frac{\text { number of outcomes in } A}{\text { total number of outcomes in the sample space } S}$$

The probability of A is the proportion of outcomes which belong to A out of all possible outcomes. So if we have the event of interest $\mathbf{A=\{6\}}$ the probability of occurrence equals to $\mathbf{\frac{1}{6}}$. We will distribute the probability of rolling a dice in a tabular form to visualize it in a different way:

- top row reflects every possible outcome of this experiment
- second row reflects the probability of occurrence
- X is a random variables, is a ‘mapping’ of the elementary outcomes in the sample space to real numbers. This allows us to attach probabilities to the experimental outcomes. → in our case the random variable is the value on top face
- as every (fair dice) dice has the same probability to occur, all possibilities have the likelihood of $\frac{1}{6}.$
- formal probability distribution:

$$\begin{array}{l|c|c|c|c|c|c}X=x & 1 & 2 & 3 & 4 & 5 & 6 \\\hline P(X=x) & 1 / 6 & 1 / 6 & 1 / 6 & 1 / 6 & 1 / 6 & 1 / 6\end{array}$$

Each possible value of the random variable assigned with the it's corresponding probability of occurrence. That example is restricted to equal distributed likelihoods per possible outcome. So the probability distribution answers the question "What is the probability of any of these values?". The random variables come in two distinct varieties:

- Discrete (⇒"count data"): random variables which take non-negative integer values, such as $0,1,2\dots$ For example the number of 1's in the rolling a dice experiment
- Continuous (⇒"measured data"): could be something like the real line $\mathbb{R}=(-\infty, \infty)$ or some subset like the unit interall.

Graphical distribution of the rolling the dice experiment:

The mathematical treatment of probability distributions depends on whether we are dealing with discrete or continuous random variables.  In the discrete case, we can associate with each ‘point’ in the sample space a probability which represents the chance of the random variable being equal to that particular value.

![https://cdn.mathpix.com/snip/images/OtooEJK1eSPhbxLm2dEA9ApeID0XzMPV18CEvH-Xhso.original.fullsize.png](https://cdn.mathpix.com/snip/images/OtooEJK1eSPhbxLm2dEA9ApeID0XzMPV18CEvH-Xhso.original.fullsize.png)

Fig. 2: Dr. James Abdey, University of Londond (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics) 

A probability distribution is the complete set of sample space values with their associated probabilities which must sum to 1 for discrete random variables.

For notational efficiency reasons, we often use a capital letter to represent the random variable. The letter $X$ is often adopted, but it is also possible to denote it by different capital letter. On the other hand a lower case letter indicates a particular value of the random variable. 

## Expectation of Random Variables

We will like further than the distribution as hole, to inspect the expectation on average of which value is going to occur. For that we will stick with the example of rolling a dice. The expectation, the mean and the average are all exchangeable synonyms for our topic under investigation. We will compute the probability-weighted average. That means that we consider each possibility of the variable and assign to each of them a weight. Mathematically that means to take each value of the variable, multiply it by its probability of occurrence, and add them all together. E.g., the dice experiment:

$$\mathrm{E}(X)=1 \times \frac{1}{6}+2 \times \frac{1}{6}+\cdots+6 \times \frac{1}{6}=3.5$$

Also if $3.5$ is not a member of the sample space it represents the long-run average. This is also called measure of central tendency (location), even if it's not an attainable value itself. This can again be visualized in a tabular way:

$$\begin{array}{l|c|c|c|c|c|c|c}X=x & 1 & 2 & 3 & 4 & 5 & 6 & \text { Total } \\\hline P(X=x) & 1 / 6 & 1 / 6 & 1 / 6 & 1 / 6 & 1 / 6 & 1 / 6 & 1 \\x P(X=x) & 1 / 6 & 2 / 6 & 3 / 6 & 4 / 6 & 5 / 6 & 6 / 6 & 21 / 6=3.5=\mu\end{array}$$

It's is very unlikely that after a large experiment the expectation value is exactly full-filled by the experiments, but with higher numbers of iterations the nearer the real average should move to the expectation value.

More formally the expectation value is also referred to as the population mean. For discrete random variables $E(X)$ is determined by taking the product of each value of $X$ and its corresponding probability. Then they are summed across all values of X,

$$\mathbf{E}(\boldsymbol{X})=\mu=\sum_{i=1}^{N} \boldsymbol{x}_{i} \boldsymbol{p}\left(\boldsymbol{x}_{i}\right)=\boldsymbol{x}_{1} \boldsymbol{p}\left(\boldsymbol{x}_{1}\right)+\boldsymbol{x}_{2} \boldsymbol{p}\left(\boldsymbol{x}_{2}\right)+\cdots+\boldsymbol{x}_{N} \boldsymbol{p}\left(\boldsymbol{x}_{N}\right)$$

where $x_1, x_2 \dots x_N$ are the possible values of the random variable X with corresponding probabilities $p(x_1), p(x_2)\dots p(x_N)$. 

**Another example with a roulette game:**

Let's assume it is a fair roulette wheel:

- 18 red numbers
- 18 black numbers
- 1 green number
- player bets on a red number

We will stick with the casino perspective, possible outcomes:

- loss of $-1$ if the red number comes up
- profit of $+1$ if a black number or a green number wins

Let's calculate the probabilities of the various events:

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/american-roulette-wheel-vector-13367259.jpeg](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/american-roulette-wheel-vector-13367259.jpeg)

Fig. 3: American roulette wheel vector image. (n.d.). [Illustration]. [https://www.vectorstock.com/royalty-free-vector/american-roulette-wheel-vector-13367259](https://www.vectorstock.com/royalty-free-vector/american-roulette-wheel-vector-13367259)

$$p(x)=\left\{\begin{array}{ll}18 / 37 & \text { for } x=-1 \\19 / 37 & \text { for } x=1 \\0 & \text { otherwise }\end{array}\right.$$

Now let's calculate the expectation of profits or losses:

$$\mathrm{E}(X)=\left(-1 \times \frac{18}{37}\right)+\left(1 \times \frac{19}{37}\right)=0.027$$

The expected outcome, 0.027, could never occur in a single play of this roulette game. Still, it indicates the expectation as a long run average. This means that for every euro that is staked by a customer on this roulette game, the casino can expect to win 2.7 cents. That's a 2.7% gain of all of the money which is staked by the customers.

**Expected value versus sample mean:**

The expected value or mean $E(X)$ of a probability distribution is similar to the sample mean $\bar{X}$ of a sample distribution. So $\bar{X}$ uses the sample proportions, $\widehat{p}\left(x_{i}\right)$, whereas $E(X)$ uses the population probabilities, ${p}\left(x_{i}\right)$.

## Bayesian Updating

> When the Facts Change, I Change My Mind. What Do You Do, Sir? - John Maynard Keynes

Bayesian updating is something we're all doing throughout our lives. We may not realize it, but we are updating our beliefs in light of new information.

**Example with the fair die, that is rolled:**

Baseline → Unconditionally, i.e. a priori (before we receive any additional information), we have:

$$P(A)=P(X=6)=\frac{1}{6}$$

New information → one is told that it will be for certain an even score, that means that all uneven numbers are eliminated in the sample space: $S'=\{\not 1, 2,\not 3, 4,\not 5,6\}$. For the event $B$  that even score occurs we have the probability of $P(B)=\frac{1}{2}$.

### Conditional Probability

conditioning refers to the receipt of new information

Coming back to our example: If we let $B$ denote the event that we get an even score, then we can write the probability of $A$ given $B$. 

The vertical line, this bar represents a conditioning situation 

$$P(A \mid B)=\frac{1}{3}$$

Probabilities will not always increase after getting new information as in our example. 

Formally the Bayes' theorem is calculated as:

$$P(A \mid B)=\frac{P(B \mid A) P(A)}{P(B)}$$

As still the likelihood of each possibility is the same and now we have $3$ possibilities, the probability of each element of the sample space increased to $\frac{1}{3}.$ More formally using the Bayes' theorem: 

$$ P(A \mid B)=\frac{P(B \mid A) P(A)}{P(B)}=\frac{1 \times 1 / 6}{1 / 2}=\frac{2}{6}=\frac{1}{3}$$

Let's assume that we instead consider the case where we are told that an odd score was obtained. Since even scores and odd scores are **mutually exclusive** (they cannot occur simultaneously) and **collectively exhaustive** (a die score must be even or odd - accumulated Probabilities will resolve in $1$), then we can view this as the complementary event, denoted $B^c$, such that:

$$B^{c}=\text { odd score }=\{1,3,5\} \quad \text { and } \quad P\left(B^{c}\right)=1-P(B)=1 / 2$$

Bayesian updating is the act of updating your (probabilistic) beliefs in light of new information.

### Solving the Monty Hall Problem with bayesian Updating

- Introduction to the problem

    You are taking part in a gameshow. The host of the show, who is known as Monty, shows you three outwardly identical doors. Behind one of them is a prize (a sports car), and behind the other two are goats.
    You are asked to select, but not open, one of the doors. After you have done so, Monty, who
    knows where the prize is, opens one of the two remaining doors.
    He always opens a door he knows will reveal a goat, and randomly chooses which door to open when he has more than one option (which happens when your initial choice contains the prize).
    After revealing a goat, Monty gives you the choice of either switching to the other unopened
    door or sticking with your original choice. You then receive whatever is behind the door you
    choose. What should you do, assuming you want to win the prize?

The doors are labelled as $A, B \:\text{and}\:C.$ The events are labelled as:

- the prize is behind the doors: $D_{A}, D_{B}, D_{C}$
- Monty opens the doors: $M_{A}, M_{B}, M_{C}$

Suppose you choose Door A first, and then Monty opens Door B (the answer works the same way for all combinations of these). So Doors A and C remain unopened.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/image-13.jpeg](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/image-13.jpeg)

Fig. 4: Pick a door - Monty Hall Problem. (n.d.). [Illustration]. [https://slidetodoc.com/presentation_image/5569651af67b14db213690a748333a81/image-13.jpg](https://www.notion.so/5569651af67b14db213690a748333a81)

To evaluate for which door we should decide to open next we need to compute the conditional probabilities of $P(D_A|M_B)$ and $P(D_C|M_B)$. If $P\left(D_{C} \mid M_{B}\right)>P\left(D_{A} \mid M_{B}\right)$ we should switch our decision from our original choice. We will use the Bayes' theorem for the probability computation. We will start with $P(D_C|M_B)$:

$$P\left(D_{C} \mid M_{B}\right)=\frac{P\left(M_{B} \mid D_{C}\right) P\left(D_{C}\right)}{P\left(M_{B} \mid D_{A}\right) P\left(D_{A}\right)+P\left(M_{B} \mid D_{B}\right) P\left(D_{B}\right)+P\left(M_{B} \mid D_{C}\right) P\left(D_{C}\right)}$$

Some information about the to assigning values:

1. As we know that initially the prizes are equally likely to be behind any of the doors, we have: 

    $$P\left(D_{A}\right)=P\left(D_{B}\right)=P\left(D_{C}\right)=1 / 3$$

2. If the prize was behind my initial chosen door $A$, monty chooses at random between the remaining doors, $B$ and $C.$ Hence $P(M_B|D_A)=\frac{1}{2}$.
3. If the price is behind a door I haven't chosen, Monty cannot open that door and must open the other one. Therefore $P(M_B|D_C)=1$ and $P(M_B|D_B)=0$. 

Now getting back to the computation of $P(D_C|M_B)$:

$$P\left(D_{C} \mid M_{B}\right)=\frac{1 \times 1 / 3}{1 / 2 \times 1 / 3+0 \times 1 / 3+1 \times 1 / 3}=\frac{2}{3}$$

The $P(D_B|M_B)=\frac{2}{3}$ enables us to compute $P(D_A|M_B)$ as follows: $1-P\left(D_{C} \mid M_{B}\right)=1 / 3$. (as $P(D_A|M_B)=0$ and so $P(D_B|M_B)=0$)

Regarding our computation we would have the highest chance to win if we switch the choice from our initial take to the door we haven't chosen yet. In our case that would be the door $C$.

The calculation applies to every combination of mine first choice and Monty's first choice. Therefore, we always are able to double the probability of winning the prize if we switch from the original choice to the door which wasn't opened yet.

**Facts about the Monty Hall Problem:**

- called a ‘cognitive illusion’ →  most common incorrect response is that the probabilities of the remaining doors after Monty’s choice are both 1/2, so that you should not switch.
- normally due to the 'no new information' reason → since we know in advance that Monty will open one door with a goat behind it, the fact that he does so appears to tell us nothing new and should not cause us to favour either of the two remaining doors - we remain with the probability of $\frac{1}{2}$ for each.
- Monty's choice doesn't introduces something new about the probability of our original choice, which remains at $\frac{1}{3}$. Still, it tells a lot about the other two doors. We can make sure, that behind the door Monty chose, there is no prize contained and the probability of this door gets 'inherited' by the door neither me nor Monty chose and increases to $\frac{2}{3}$.
- one can expect to win with a probability of $\frac{2}{3}$, i.e. you would win $\frac{2}{3}$ of the time on average.

## Parameters

Probability distributions differ from each other, different families of distributions have different features:

- discrete vs. continuous distributions
- among discrete distributions → finite versus an infinite number of possible values
- among continuous distributions → among continuous distributions: different sets of possible values (for example, all real numbers $x, x>0, \text { or } x \in[0,1]$); symmetric versus skewed distributions

These distributions are really families where each individual distribution within a family differ in having different values of the parameters of the distribution. These parameters for example determine the mean and the variance of a distribution. 

For a statistical analysis of a random variable $X$ we select an according family based on the properties of $X$ and use the observed data to choose (estimate) values for the parameters of that distribution. On that we will perform statistical inference. 

### Bernoulli-Trial

This specific trial is an experiment with only two possible outcomes. We will label the binary outcome by $1$ and $0$ and refer to them as success and failure. That has nothing to do with a good or bad outcome.

### Bernoulli-Distribution

It is the distribution of the outcome of one single Bernoulli-trail. This distribution of a random variable $X$ with the following probability function:

$$P(X=x)=\left\{\begin{array}{ll}\pi^{x}(1-\pi)^{1-x} & \text { for } x=0,1 \\0 & \text { otherwise. }\end{array}\right.$$

That means: $P(X=1)=\pi^{1}(1-\pi)^{1-1}=\pi$ and $P(X=0)=\pi^{0}(1-\pi)^{1-0}=1-\pi$

In a tabular form we could express this family of Bernoulli distribution as, where $0 \leq \pi \leq 1$ is the probability of ‘success’.

$$\begin{array}{l|c|r}X=x & 0 & 1 \\\hline P(X=x) & 1-\pi & \pi\end{array}$$

A parameter space represents all possible values of a parameter, like a sample space represents all possible values of a random variable. Therefore we must have $0 \leq \pi \leq 1$.

Such a random variable has a Bernoulli distribution with (probability) parameter π. This is often denoted as: ${X} \sim \operatorname{Bernoulli}(\pi)$. With that we can calculate it's expected value as the usual probability weighted average:

$$\mathbf{E}(\boldsymbol{X})=\mathbf{0} \times(\mathbf{1}-\boldsymbol{\pi})+\mathbf{1} \times \boldsymbol{\pi}=\boldsymbol{\pi}$$

π indicates the long-run average of successes if we would commit a large random sample from this distributions. Members within a distribution family differs in terms of the value of π. 

**Example of a fair coin toss:**

We will denote 'tails' by $1$ and head by $0$. As both option are equally likely to happen π = $0.5$.

$$\begin{array}{l|c|c}X=x & 0 & 1 \\\hline P(X=x) & 0.5 & 0.5\end{array}$$

which leads to the following expected value:

$$\mathrm{E}(X)=0 \times 0.5+1 \times 0.5=0.5$$

So I can expect the proportion of heads to be 0.5 after a large number of tosses.

## Distribution Zoo

### Bernoulli-Distribution

We already used the Bernoulli-Distribution for the previous example. This kind of distribution is a discrete one with two possible outcomes. Normally the outcomes are labelled by $n=0$ and $n=1$. Normally the probability that $n=1$ occurs it equal to $p$ and the probability that $n=0$ occurs is equal to $q=1-p$. Therefore the probability density function equals to:

$$P(n)=\left\{\begin{array}{ll}1-p & \text { for } n=0 \\p & \text { for } n=1\end{array}\right.$$

as we have seen before, that can also be written as: $P(n)=p^{n}(1-p)^{1-n}$. For the Bernoulli distribution we only have one parameter which is called $n$ in our case.

### Binomial distribution

A binomial distribution is equals to consecutive Bernoulli trials. Therefore $n$ indicates the number of the back-to-back trials. If $n=1$ the Binomial distribution would equal to a Bernoulli distribution. Therefore this kind of distribution is also a discrete probability distribution with formally formulated, a sequence of $n$ independent experiments (Bernoulli trials). The probability function with with the parameter $n$ and $p$ from the Bernoulli distribution would equal to:

$$P(x;p,n)=\left\{\begin{array}{cl}\left(\begin{array}{l}n \\x\end{array}\right) p^{x} *(1-p)^{n-x} & \text { if } x=0,1, \ldots, n \\0 & \text { otherwise }\end{array}\right.$$

Where $\left(\begin{array}{l}n \\x\end{array}\right)$ is the so-called binomial coefficient: the number of ways of choosing $x$ objects out of $n$ when sampling without replacing the objects and it's sequence doesn't matter. The bionomial coefficient is calculated by:

$$\frac{n !}{x !(n-x) !}$$

This distribution is also often written as: 

$$X \sim \operatorname{Bin}(n, p)$$

The binomial distribution is only applicable if the following conditions are fixed:

1. the number of trials / experiments $n$ is fixed
2. each trials / experiments or is independent from each other
3. each trials / experiments is in a boolean form (two outcomes)
4. the probability of $p$ per Bernoulli trial is fixed for each outcome

**Example:**

Let's assume the test for the german's driver license which requires to answer n = $20$ questions correctly with $4$ possible answers per question. Now we will compute $X \sim \operatorname{Bin}(20, p)$ for different $p's$.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled.png)

Fig. 5: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

### Poisson distribution

This distribution is very useful if we're interested in the number of occurrences of some phenomenon per unit of time or maybe per unit of distance. It is also a discrete probability distribution. With the information of how often on average an event is happening during the time horizon it is possible to compute the probabilities of the occurrence of an event which differs from the average.

To summarize the prerequisites of being able to apply the poisson distribution:

- an event can occur an unlimited number of times during the given interval
- each trials / experiments or is independent from each other in the given interval
- The occurrence of an event is constant and thus proportional to the length of the given interval

A common example of poisson process are visitors to a website where the average of visitors within a certain time horizon is known.

The poisson distribution probability function gives the probability of $k$ events in a time frame where the length of the time frame and it's average event per time is given:

$$P(k \text { events in time period })=e^{-\frac{\text { events }}{t \text { time period }}} * \frac{\left(\frac{\text { events }}{\text { time }} * \text { time period }\right)^{k}}{k !}$$

Normally the $\frac{\text { events }}{\text {time}} * \text{time period}$ term is simplified into $\lambda$. This is then the so called rate parameter. Then the probability function looks like:

$$P(k \text { events in interval })=e^{-\lambda} \frac{\lambda^{k}}{k !}$$

Intuition-wise Lambda is the expected number of events in the interval. Beforehand I have mostly mention it time frame, but the poisson distribution goes beyond the time component as long as there is an interval.

**Example:**

As we mentioned before we will use the visitors of a website as an example. We can model it with poisson because the visitors are independent, the average number of visitors per hour is constant and as we are doing an approximation, the visitors don't visit the site simultaneously. Let's start with defining the $\lambda$ parameter $\frac{\text { events }}{\text {time}} * \text{time period}$. We have one visitor every 6 minutes and we are analyzing a period of one hour. So $\lambda$ equals to $10$. A friend wants to bet with me that over the next hour there will be either 9 or 11 visitors. 

$$P(9 \text { visitors in } 1 \text { hour })=e^{-10} \frac{10^{9}}{9 !}= 0,1251=12.51 \%$$

$$P(11 \text { visitors in } 1 \text { hour })=e^{-10} \frac{10^{11}}{11 !}= 0,1137 =11.37 \%$$

$$P(9 \text { visitors in } 1 \text { hour }) +P(11 \text { visitors in } 1 \text { hour })=23,88 \%$$

The probability that he would win is about $23,88 \%$, so I would accept the bet.

### Beyond one probability distributions

Due to the breadth of the family of probability distributions, similarities or even identical features can be found. For example $\text{Bernoulli}(\pi)$ and $\text{Bin}(1,\pi)$. Some connections between distribution are asymptotic (approximate). That means that one distribution is (as close as possible) approximated by another under some limiting conditions. 

The probability distributions can be used to model some real-world occasions. Still, we have to keep in mind that the kind of models are not equal to reality, while a good model tries to approximate reality as close as possible. 

# Describing The World The Statistical Way

## Classification of Variables

### Measurable variables

If we are dealing with a variable where a generally recognised method exists for determining its value it is a measurable variable. Then the variable contains data which can be analyzed and also compared. It is possible to verify whether two variables are the same. most measurable variables can be split up into two types:

1. **Discrete Data**: countable things which can only take certain values. **Example: Rolling two dice**
2. **Continuous Data**: measurable things which can take any value (within a range), infinite possible values.  **Example: height of a person**

**Interval measurable variables**

Interval-level variables have nummerically equal distantance scales which represent a equal value of difference. The location zero point is not fixed and like the units of measurement both are abitrary. This allows comparisons of different values on the scale. Using a positive linear transformation of $y=a+bx$ transforms the scales while preserving ll the properties. The following statistical methods can be applied to this type of data:

- counting operations
- mean and standar deviation

- centile operations

**Example:** Temperature ****measured within three days can have the values of $**0, 10$** and **$20$** degrees**.** There is a constant $10$-degree differential between the measured values. That shows that the values are comparable. Still the temperature can be measured in different untis like degrees Celsius and degrees Fahrenheit.

**Ratio measurable variables**

Ratio-Level variables obtain all the properties of nominal, ordinal and intervall variables and have a fixed zero point. Only transformation of the type proportionate transformation of $y=bx$ are allowed where $b$ is a positive constant. All statistical techniques can be applied. 

**Example:** Temperature measurement with the kelvin scale. It uses the absolute zero as it's null point. (fixed zero-point)

### Categorical variables

Variables belonging to this category take values that are names or labels. While working with this variables it is common practice to convert the different categorical variables to numerical variables while assigning a number to each categorical variable.

**Nominal categorical variables**

For nominal variables the values serve only as labels for identifying classes. These values can also be used for identification purposes. (Passport number, Sprint start number) While assigning the values one have to keep in mind, that the values do not represent any order or sequence. Counting the different nominal categorical variables is the only arithmetic approach to work with this kind of data.

**Example**: Gender One gender  is not more or less gender than an other genders, the nominal categorical variables are just used for classifications purposes.

**Ordinal categorical variable**

An ordinal variables works with a ranking scale on which bases one can assume the relative extent to which the cases obtain some characteristics. One can deduce whether one case is larger or smaller than another, but not by which exact value. With these kind of data there are a lot of operations possibles like counting and others based on centiles. 

**Example:** Economic status with three categories (high, medium and low). Then one can assign this category to countries one is analyzing and afterwards it is possible to sort them.

## Data visualization

**Statistical analysis** helps us to summarize collected data to make it easier to understand and work with. That process is called **descriptive statistics**. It attempts to reduce the data to some key features for better communication which can take place in a graphical or numerical way. 

Furthermore **statistical inference** is used to draw conclusions out of the observed data and transfer it to a broader population.

Typically data is stored in a data matrix with the following properties:

- rows ⇒ different **units** (subjects or observations) in our example different countries
- number of units is the **sample size**, mostly denoted by $n$
- columns ⇒ **variables** that equals to different characteristics of the units

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%201.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%201.png)

Fig. 6: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

**The sample distribution:**

The sample distribution of a variable is a list of values of the corresponding variable which are observed within the sample to be suppressed and the counts of how often each value occurs. To visualize the sample distribution one can construct a frequency table.

Often also the proportion of variables or their relative frequency is computed to compare the relevance of the variables. Often the relative frequency is denoted by percentages. Normally it is calculated for one value of variable by:

$$\frac{\text{number of occurrences of an unique value of variable}}{\text{n sample size}}$$

The cumulative percentage for a value of a variable is the sum of percentages for that value and all previously calculated lower-numbered values. Because of this, the cumulative percentage is always 100 when the highest value is reached.

The gained insights by a sample distribution and their analysis can be communicated as described as an table (e.g. frequency table) but also as a graphical plot. (e.g. bar chart)

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%202.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%202.png)

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%203.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%203.png)

Fig. 7: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

In the case that we face a variable with width range of distinct values, we group them into non-overlapping intervals. With the help of the changed data we can produce a better visualization using a graph or a table. Mostly used for graph visualization is the histogram. In the following example we observe the step of accumulating the data within intervals and plotting them using an histogram.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%204.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%204.png)

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%205.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%205.png)

Fig. 8: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

## Associations between two variables

We have visualized the distribution for one variable. Now we can extend this by one (or more) variables and analyze its correlations. For example, a correlation would be the occurrence of a low value of one variable when another variable also has a low value. 

In the following we will look at some descriptive statistics methods to look at correlations between two variables. In most cases, we distinguish whether the variables can have 'few' or 'many' possible values.

1. **Scatterplots:** If both variables have 'many' variables we tend to use scatterplots. A scatterplot plots the values of each variable against each other as a point in a two-dimensional coordinate system. A scatter plot can also be extended my different categorical data if the circle plot varies for each category. (e.g.: by circle colour)

    ![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Gound_Living_Scatter_Plot.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Gound_Living_Scatter_Plot.png)

    Fig. 8: Scatter Plot. (n.d.). [Graph]. [https://www.data-to-viz.com/graph/scatter_files/figure-html/unnamed-chunk-1-1.png](https://www.data-to-viz.com/graph/scatter_files/figure-html/unnamed-chunk-1-1.png)

    The x-axis shows the partially ground living area of the sold apartment with the corresponding sale price on the y-axis.

2. **Boxplots:** If a variable has a few possible values and an other has many possible variables then side-by-side boxplots are recommended. Often they are used to compare the distribution of measurable variables across groups of data, e.g. a comparison of a measurable variable (kids mortality rate) across different levels of categorical variables. (countries/regions) Boxplots can also show outliers within that comparison. 

    ![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%206.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%206.png)

    Fig. 9: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

    The graph shows for example that the GDP per capita is very low in africa with some outliers. The vertical line of a plot indicates at it's maximum the maximum value of the variables and the lowest point shows it's minimum value. The box visualize the interquartile range from the lower quartile to the upper quartile. This interquartile range is divided by the median as a black line of the variable.

3. **contingency table:** If both variables have only a few possible outcomes the usage of a two-way contingency table (cross-tabulation) is recommended. The tables show the frequencies of each possible combination of values of two categorical variables. Normally the frequency is extended by the percentage within each row of column. 

    ![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/contingency_table_joint_probabilities.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/contingency_table_joint_probabilities.png)

    Fig. 10: Contingency Table Joint Distribution. (n.d.). [Graph]. [https://i2.wp.com/statisticsbyjim.com/wp-content/uploads/2021/02/contingency_table_joint_probabilities.png?resize=447%2C137&ssl=1](https://i2.wp.com/statisticsbyjim.com/wp-content/uploads/2021/02/contingency_table_joint_probabilities.png?resize=447%2C137&ssl=1)

    The row variables is a categorical variable showing whether the person's gender is mal or female. The column variable show how often the gender uses whether a Mac or PC.

Correlations between variables don't imply causality.

## Descriptive Statistics - Measures of Central Tendency

After illustrating how histograms and frequency tables can be used to describe the overall distribution of a variable, we now look at how descriptive statistics can be used to reduce one feature to a single number. That is also called summary descriptive statistics. For now we focus on the measures of central tendency which supports us by defining the centre of the distribution for us. The following metrics can be used:

- mean
- median
- mode

### Notation for variables

A variables normally is denoted by the single letter $X$ where any letter can be used as long as it is done consistently. The subscript of a letter denotes a single observation of a variable. Here, $X_i$ is represented where $i$ can take values of $1,2 \dots, n$. Here, $n$ corresponds to the sample size. It can also be formulated as $n$ for $i=1, \dots,n$.

If $X_1,X_2, \dots,X_n$ is a set of numbers. The sum of the numbers is written as:

$$\sum_{i=1}^{n} \boldsymbol{X}_{i}=\boldsymbol{X}_{1}+\boldsymbol{X}_{2}+\cdots+\boldsymbol{X}_{n} \:\text{or}\: \sum_{i} X_{i}\:\text{or just}\:\sum X_{i}.$$

### The mean

The mean (sample mean, arithmetic mean or average) is the most used measure metric for defining the central tendency of a variables within a distribution. The mean is denoted by a bar over the variable letter: $\bar{X}$. 

In words, the mean is the sum of all observations divided by the number of observations (sample size) and can be described mathematically as follows:

$$\bar{X}=\frac{\sum_{i=1}^{n} \boldsymbol{X}_{i}}{n}=\frac{1}{n} \sum_{i=1}^{n} \boldsymbol{X}_{i}$$

Using the example of the distribution of five numbers $1,3,5,8 \:\text{and}\:21$ we can calculate the mean as follows:

$$\frac{1+3+5+8+21}{5}=\frac{38}{5}=7,6$$

If we look again at the Frequency table mentioned earlier, it has 11 different values for the variable level of democracy which have a certain frequency in the data set described at $f_i$.

If we assume that $X$ can take $K$ different values $X_1,X_2 \dots,X_K$ as well as the corresponding frequencies $f_1,f_2,\dots,f_K$, therefore $\sum_{j=1}^{K} f_{j}=n$ and:

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%207.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%207.png)

Fig. 11: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

$$\bar{X}=\frac{\sum_{j=1}^{K} f_{j} X_{j}}{\sum_{j=1}^{K} f_{j}}=\frac{f_{1} X_{1}+\cdots+f_{K} X_{K}}{f_{1}+\cdots+f_{K}}=\frac{f_{1} X_{1}+\cdots+f_{K} X_{K}}{n}$$

For our example where $K=11$ is the calculation would look like:

$$\frac{35 \times 0 +12\times1+4\times2+\dots+32\times10}{35+12+4\dots+32}=\frac{0+12+8\dots+320}{155} \approx5.3$$

The mean of the level of democracy equals to approx. $5.3$  for the investigated sample. 

The sum of the deviations between the variable and the mean is $0$. Indicates by $\sum_{i=1}^{n}\left(\boldsymbol{X}_{i}-\overline{\boldsymbol{X}}\right)=\mathbf{0}$. As the mean is in the middle of the observation of the sample set the positive and negative values of the deviations $X_i-\bar{X}$ cancel out, when summed over the set.

### The median

If the subscripts of the sample values of $X$ are indicated with brackets around the index, they are ordered - normally they are ordered from the smallest to the largest, so that $X_{(1)}$ is the smallest value (minimum) and $X_{(n)}$ is the largest value (maximum). This order is know as **order statistics.**

The (sample) median denoted by $q_{50}$ of a variable $X$ is the value which is in the middle of a variable ordered in the order statistics. Its calculation is differentiated depending on whether the sample size is even or odd.

**Odd:** Since there is a unique value that lies in the middle, you only have to calculate the exact midpoint and this value then corresponds to the median.

$$q_{50}=X_{((n+1) / 2)}$$

If for example $n=7$ then $q_{50}=X_{(4)}$.

**Even:** If we have a sample size that is even, we take both values that are closest to the center of the sample size add them together and divide the sum by two.

$$q_{50}=\left(X_{(n / 2)}+X_{(n / 2+1)}\right) / 2$$

If for example $n=10$ then $q_{50}=\left(X_{(5)}+X_{(6)}\right) / 2$. 

Coming back to our prior example of the level of democracy of different countries, we will calculate its median. As we have a sample size of $n=155$, $q_{50}=X_{(78)}$. If we retrieve the value for $X_{(78)}$ we get the median of 6. The median can also be determined by the frequency table, because the median is the value for which the cumulative percentage first reaches $50 \%$.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%208.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%208.png)

Fig. 12: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

### Sensitivity to outliers

In general the mean is way more affected by outliers compared to the median, especially in quite small or large observations. Let's compare two small observations and observe how the mean changes if a number is added:

$X_1=[1,2,4,5,8]$

The mean for $X_1$ equals to $4.5$.

$X_2=[1,2,4,5,8,100]$

The mean for $X_2$ equals to $20$.

Due to median's property of being more sensitive to outliers it is pulled toward the longer tail of the distribution. That results in:

- the mean is larger than the median, for a positively-skewed distribution
- the mean is smaller than the median, for a negatively-skewed distribution
- the mean and median are equal, for an exactly symmetric distribution

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/skew_distributins.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/skew_distributins.png)

Fig. 13: Hermans, R. (2008). Diagrams illustrating negative and positive skew [Graph]. [https://commons.wikimedia.org/wiki/File:Negative_and_positive_skew_diagrams_(English).svg](https://commons.wikimedia.org/wiki/File:Negative_and_positive_skew_diagrams_(English).svg)

One then has the decision to what extent one wants to deal with the outliers. You can either keep them or remove them from the sample.

### The mode

The (sample) mode of variable is the values which occurs most often in the sample or with our notation has the highest frequency. For our data example for the level of democracy the mode of the level is $0$, which occurred $35$ times. This measurement metric is not useful for continuous values because there are basically infinitely many values that a variable can take. It is also possible that a variable is multimodal, which indicates there are several modes. 

## Descriptive Statistics - Measures of Spread

We have now discovered the measures of central tendency. Despite similar measures of central tendency, two distributions can be very different in that their values have a high dispersion (variation).

The two graphs on the right show distributions with a mean at $0$. Nevertheless, the variation within values is higher for the distribution shown with the solid line than for the distribution with the dashed line.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Two-Gaussian-distributions-with-the-same-mean-and-different-variances.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Two-Gaussian-distributions-with-the-same-mean-and-different-variances.png)

Fig. 14: Gangeh, M. (2013). Two Gaussian distributions with the same mean and different variances [Graph]. [https://i2.wp.com/statisticsbyjim.com/wp-content/uploads/2021/02/contingency_table_joint_probabilities.png?resize=447%2C137&ssl=1](https://i2.wp.com/statisticsbyjim.com/wp-content/uploads/2021/02/contingency_table_joint_probabilities.png?resize=447%2C137&ssl=1)

To calculate the dispersion of a sample set the sum of the squared deviations from the mean is used.

**Example:** If we have a sample set with $n=5$ and the following values $X = 1,2,3,5,9$ the mean equals to $\bar{X}=4$. Therefore the sum of the squared deviations from the mean equals  to:

$$(1-4)^2+(2-4)^2+(3-4)^2+(5-4)^2+(9-4)^2=40$$

### Variance and standard deviation

The (sample) variance and its square root, the sample deviation, are both based on $(X_i-\bar{X})^2$. Normally the sample variance of a variable is denoted by $S^2$ and defined as:

$$S^{2}=\frac{1}{n-1} \sum_{i=1}^{n}\left(\boldsymbol{X}_{i}-\overline{\boldsymbol{X}}\right)^{2}$$

The according sample standard deviation of $X$ is denoted by $S$ and equals to the positive square root of the sample variance:

$$S=\sqrt{\frac{1}{n-1} \sum_{i=1}^{n}\left(X_{i}-\bar{X}\right)^{2}}$$

The $S^2$ and $S$ of a sample distribution are the most used measures of dispersion. As the standard deviation, $S$ is measured in the same unit as $X$ it is more understandable and intuitive. Both have the property of never being negative and they are both only zero if all the $X_i$ observations are the same.

For our before-hands introduced example with $n=5$, $X = 1,2,3,5,9$, $\bar{X}=4$ and the sum of the squared deviations from the mean of $40$ we will look at the $S^2$  and $S$ metrics:

$$S^{2}=\frac{1}{n-1} \sum\left(X_{i}-\bar{X}\right)^{2}=\frac{40}{4}=10$$

$$S=\sqrt{S^{2}}=\sqrt{10}=3.16$$

The standard deviation of the distribution equals to $3.16$.

### Quantiles

As already introduced the median $q_{50}$ is dividing the sample into the 50% smallest and 50% largest parts an observation. We can vary the percentage split, for getting different quantiles (percentiles) which are denoted by $q_c$. The following quantalies are some common ones:

- first quartile, $q_{25} \:\text{or}\:Q_1$ is the value dividing the sample into the smallest 25% of the observations from the rest
- third quartile, $q_{75} \:\text{or}\:Q_3$ gives the 75% to 25% split.
- the minimum, the 0% quantile equals to $X_{(1)}$ and the maximum, also the so-called 100% quantile, equals to $X_{(n)}$.

The mentioned are more more general measures of a location of the sample distribution than metrics for defining the middle of a distribution. Two quantile-type statistics are commonly used:

- the range of a sample set where the minimum is subtracted from the maximum value to get all the range possible values. More formally the range equals to $X_{(n)}-X_{(1)}$. As it always takes the minimum and maximum value of a sample it is very sensitive to outliers.
- the interquartile range also called IQR focuses on the middle 50% of the distribution, so it is independent of outliers. Formally it can be expressed as $q_{75}-q_{25}=Q_{3}-Q_{1}$

### Boxplots

A boxplot, also called a box-whiskers plot, is a widespread tool to condense distribution properties using the concept of the introduced quantiles. If a whisker in one direction is longer in relation to the other in its direction, it indicates a skewed distribution. That skewness is also confirmed by the median line not being in the middle of the box. 

The details that can be retrieved from a box-plot are the following:

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/boxplot-stats.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/boxplot-stats.png)

Fig. 15: horizontal Boxplot. (n.d.). [Graph]. [https://lsc.studysixsigma.com/wp-content/uploads/sites/6/2015/12/1435.png](https://lsc.studysixsigma.com/wp-content/uploads/sites/6/2015/12/1435.png)

## Normal Distribution (Gaussian distribution)

There are different reasons why the normal distribution is the most used distribution to model variables as many of the variables are approximately normally distributed (height of humans) or that the mathematical properties are very convenient, and even if the variable itself is not normally distributed, often the sample distributions of a variable are normally distributed due to the **central limit theorem**.

The normal distribution equation where $\pi$ is the mathematical constant and $\mu$ (mean) and $\sigma^2$ (variance) are the parameters. 

$$f(x)=\frac{1}{\sqrt{2 \pi \sigma^{2}}} \exp \left[-\frac{(x-\mu)^{2}}{2 \sigma^{2}}\right] \quad \text { for }-\infty<x<\infty$$

For $\mu$ applies $-\infty<\mu<\infty$ and for $\sigma^2 > 0$. That results in an infinite amount of combinations for the distributions.

A random variable $X$ with this functions and its parameters is denoted by $X \sim N\left(\mu, \sigma^{2}\right)$. The mean can also be retrieved by the fact that the normal distribution is symmetric about $\mu$. That also indicates that the median of a normal distribution equals $\mu$. 

In a simplified manner, the $\mu$ determines the location of a curve and the variance $\sigma^2$ the spread or dispersion of a curve — the following graphic shows how the parameters influence the distribution.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/distributions_normal.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/distributions_normal.png)

Fig. 16: Normal Distribution PDF. (2008). [Graph]. [https://commons.wikimedia.org/wiki/File:Normal_Distribution_PDF.svg](https://commons.wikimedia.org/wiki/File:Normal_Distribution_PDF.svg)

### Linear transformations of normal distributions

A convenient property of the normal distribution is the possibility of linearly transform the distribution with $\boldsymbol{Y}=\boldsymbol{a} \boldsymbol{X}+\boldsymbol{b}$, where $a$ and $b$ are both constants. As long $X$ has a mean of $\mu$ and a variance of $\sigma^2$, $Y$ has a mean of $a\mu+b$ and variance of $a^2\sigma^2$. $Y$  takes over the property of $X$ of the normal distribution, more formally if $X \sim N\left(\mu, \sigma^{2}\right)$, then:

$$Y=a X+b \sim N\left(a \mu+b, a^{2} \sigma^{2}\right)$$

This result of remaining in the same family of distribution, even after the transformation is not true in general and something which is applicable specifically for the normal distribution.

Example with $a=1/\sigma$ and $b=-\mu/\sigma$, to get:

$$Z=\frac{1}{\sigma} X-\frac{\mu}{\sigma}=\frac{X-\mu}{\sigma} \sim N\left(\frac{1}{\sigma} \mu-\frac{\mu}{\sigma},\left(\frac{1}{\sigma}\right)^{2} \sigma^{2}\right)=N(0,1)$$

Z is the transformed variable of $X$ and equals to $Z=\frac{(X-\mu)}{\sigma}$ and is known as **standardized variable** or a z-score. As derived above, the distribution of the standardized variable is $N(0,1)$. So the $\mu=0$, the $\sigma^2=1$ and therefore also the standard deviation $\sigma=1$. This distribution is known as the standard normal distribution. 

The following figure shows the probabilities of the standard normal distribution where the shaded areas are $P(Z \leq-z)=P(Z \geq z)$ with the symmetry of the distribution about $0$.

With the standard normal distribution, it is very convenient to compute the probability of a range with computing as one can compute the probability of a range with the standardized normal distribution and afterward one can look up the given value in a z-score table to get the probability. 

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%209.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%209.png)

Fig. 17: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/z-table-example.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/z-table-example.png)

Fig. 18: Z table example. (n.d.). [Graph]. [http://qualityengineer.weebly.com/uploads/1/3/1/0/131059459/published/z-table-example.png?1584414181](http://qualityengineer.weebly.com/uploads/1/3/1/0/131059459/published/z-table-example.png?1584414181)

## Variance of random variables

Variance indicates how far a set of numbers is spread out from their mean, $\mu$. More formally, the variance is the expectation of the squared deviation of a random variable from its mean. The variance is a metric for measuring the dispersion of a distribution. We can differ between two types of variance:

The **sample variance** $S^2$ which refers to the dispersion in a sample dataset, is simply an average. An average over the squared deviation of the data in relation to the sample mean. The equation for computing the sample variance is the following:

$$S^{2}=\frac{1}{n-1} \sum_{i=1}^{n}\left(X_{i}-\bar{X}\right)^{2}.$$

The division by $n-1$ rather than only by $n$ is called an unbiased estimator and ensures that the sample variance estimates the population variance correctly on average. 

The **population variance** $Var(X)=\sigma^2$ , which measures the variance of the whole population as the name already indicates. The computation works quite similarly as we calculate the average squared deviation about the population mean. 

The population mean equals the prior introduced probability-weighted average: 

$${E}({X})=\sum_{i=1}^{{N}} {x}_{i} {p}\left({x}_{i}\right)$$

The concept of the expected value can be applied to functions of the random variable. If $X$ corresponds to the values $x_1,x_2\dots x_N$ with the probabilities $p(x_1),p(x_2),\dots p(x_N)$, then:

$$\mathrm{E}\left(\frac{1}{X}\right)=\sum_{i=1}^{N} \frac{1}{x_{i}} p\left(x_{i}\right) \quad \text { for all } x_{i} \neq 0$$

and also the following both:

$$\mathrm{E}(\ln (X))=\sum_{i=1}^{N} \ln \left(x_{i}\right) p\left(x_{i}\right) \\ \quad \text { for all } x_{i}>0$$

$$\mathrm{E}\left(X^{2}\right)=\sum_{i=1}^{N} x_{i}^{2} p\left(x_{i}\right)$$

If we use the function $(X-\mu)^2$ about the population mean, the expectation of this equals to:

$$\sigma^{2}=\operatorname{Var}(X)=\mathrm{E}\left((X-\mu)^{2}\right)=\sum_{i=1}^{N}\left(x_{i}-\mu\right)^{2} p\left(x_{i}\right)$$

As the expectation equals the probability-weighted average, we multiply the squared difference between $x_i$ and the population mean $\mu$ with the probability of occurrence of $x_i$. The sum equals $\sigma^2$ which represents the dispersion of a (discrete) probability distribution.

**Example:**

To illustrate the standard deviation and variance of a probability distribution, we refer back to the example explained earlier, with the roll of a fair die. We can compute the mean and variance as followed: 

$$\begin{array}{l|c|c|c|c|c|c|c}X=x & 1 & 2 & 3 & 4 & 5 & 6 & \text { Total } \\\hline P(X=x) & 1 / 6 & 1 / 6 & 1 / 6 & 1 / 6 & 1 / 6 & 1 / 6 & 1 \\x P(X=x) & 1 / 6 & 2 / 6 & 3 / 6 & 4 / 6 & 5 / 6 & 6 / 6 & 21 / 6=3.5=\mu \\(x-\mu)^{2} & 25 / 4 & 9 / 4 & 1 / 4 & 1 / 4 & 9 / 4 & 25 / 4 & \\(x-\mu)^{2} P(X=x) & 25 / 24 & 9 / 24 & 1 / 24 & 1 / 24 & 9 / 24 & 25 / 24 & 70 / 24=2.92\end{array}$$

That visualizes every individual result, we are gonna pick the number $1$ and compute the dedicated squared deviation and also the expectation of the squared deviation.

$$(x-\mu)^2=(1-3.5)^2=(-\frac{5}{2})(-\frac{5}{2})=\frac{25}{4}$$

$$(x-\mu)^2P(X=x)=\frac{25}{4} \cdot \frac{1}{6}=\frac{25}{24}$$

Hence $\mu=3.5$, $\sigma^2=E((X-\mu)^2)=2.92$ and therefore the standard deviation equals to $\sigma=\sqrt{2.92}=1.71$. 

### Probabilities for any normal distribution

If we want to calculate the probability of a range $a<b, P(a<X\leq b)$ within a normal distribution with $X \sim N(\mu,\sigma^2)$ for any $\mu$ and $\sigma^2$, we apply a transformation to all parts of the inequalities on the bases of:

$$\frac{{X}-{\mu}}{{\sigma}}={Z} \sim {N}({0}, {1})$$

The application of transformation results in:

$$\begin{aligned}P(a<X \leq b)=P\left(\frac{a-\mu}{\sigma}<\frac{X-\mu}{\sigma} \leq \frac{b-\mu}{\sigma}\right) &=P\left(\frac{a-\mu}{\sigma}<Z \leq \frac{b-\mu}{\sigma}\right) \\&=\Phi\left(\frac{b-\mu}{\sigma}\right)-\Phi\left(\frac{a-\mu}{\sigma}\right)\end{aligned}$$

where the new introduced symbol $\Phi(k)=P(Z\leq k)$ equals the cumulative probability for some value of $k.$ The introduced procedure is also called standardization.

The concept of cumulative probabilities indicates the likelihood that the value of a random variable falls within a specified range. Frequently, cumulative odds refer to the probability that a random variable is less than or equal to a specified value.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2010.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2010.png)

Fig. 19: cumulative probabilities. (n.d.). [Graph]. [https://i.stack.imgur.com/wWTai.png](https://i.stack.imgur.com/wWTai.png)

**Example**

We have $X$ which equals diastolic blood pressure of randomly selected people with the distribution of $X\sim N(74.2,127.87)$. We want to compute the probability of normal blood pressure $60 \leq X \leq 90$.

First, we apply the standardization to the normal distribution with $\mu=74.2, \sigma^2=127.87$ and $\sigma=11.31$ to get the standard normal distribution.

$$\frac{X-74.2}{11.31}=Z \sim N(0,1)$$

Our approach is to calculate two cumulative probabilities, first the probability of $P(X\leq90)$ and then we subtract $P(X\leq60)$ from it.

$$\begin{aligned}P(X \leq 90)=P\left(\frac{X-74.2}{11.31}\leq\frac{90-74.2}{11.31}\right)\\
=P(Z\leq 1.40)=\Phi(1.40)=0.9192\end{aligned}$$

and:

$$\begin{aligned}P(X \leq 60)=P\left(\frac{X-74.2}{11.31}\leq\frac{60-74.2}{11.31}\right)\\
=P(Z\leq -1.26)=\Phi(-1.26)=0.1057\end{aligned}$$

That results in the probability of:

$$P(60 \leq X \leq 90)=0.9192-0.1057=0.8135$$

To get a better intuition of our calculation, I have sketched a probability distribution and added the corresponding ranges that we calculate. Thus, by calculating the area up to the upper boundary and subtracting the lower boundary areas, we should find the area or probability for the interval we are looking for.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2011.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2011.png)

Fig. 20: Standard normal distribution boundaries

### Probabilities around the mean

All the normal distributions have common properties regarding their alignment of probabilities in relation to their mean and standard deviation.

- 68.3% of the total probability is within one standard deviation

    $P(\mu-\sigma<X<\mu+\sigma)=0.683$

- 95.4% (approx. 95%) of the probability is within two $\sigma$

    $P(\mu-2 \times \sigma<X<\mu+2 \times \sigma)=0.954$

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/1_IdGgdrY_n_9_YfkaCh-dag.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/1_IdGgdrY_n_9_YfkaCh-dag.png)

Fig. 21: Normal Distribution Probabilities Visualization. (n.d.). [Graph]. [https://miro.medium.com/max/24000/1*IdGgdrY_n_9_YfkaCh-dag.png](https://miro.medium.com/max/24000/1*IdGgdrY_n_9_YfkaCh-dag.png)

- 99.7 % of the probability is within three $\sigma$ - $P(\mu-3 \times \sigma<X<\mu+3 \times \sigma)=0.997$

Similar properties apply to the standard normal distribution $N(0,1)$ where $\mu=0$ and $\sigma=1$. As the parameters and the distribution are standardized it is possible to use the z-values as indicators and don't need the mean nor the standard deviation.

$$\begin{array}{l}P(-1 \leq Z \leq 1) \approx 0.683 \\P(-2 \leq Z \leq 2) \approx 0.950 \\P(-3 \leq Z \leq 3) \approx 0.997\end{array}$$

With that standardized basis it is very convenient to detect extreme values and outliers. Roughly speaking, everything outside ±2 can be classified as an outlier, everything above ±3 as an extreme outlier, and finally everything outside ±4 as a black swan event.

## Exercises - Describing the world the statisical way

This assignment gives you the opportunity to compute some simple descriptive statistics based on a small dataset, as shown below:

Four observations are obtained: $X=7, 9, 10, 11$. For these four values, derive the following:

the sample mean:

$$\frac{7+9+10+11}{4}=\frac{37}{4}=9,25$$

the sample median:

$$(9 + 10) / 2 = 9,5$$

show that $\sum\limits_{i=1}^4 (x_i - \bar{x}) = 0$:

$$(7-9,25)+(9-9,25)+(10-9,25)+(11-9,25)=0$$

compute the sample variance $s^2 = \frac{1}{4-1}\sum\limits_{i=1}^4 (x_i - \bar{x})^2$

$$\frac{1}{3} * ((2,25)^2 + (0,25)^2 + (0,75) ^ 2 + (1,75)^2)=2,916666667$$

compute the sample standard deviation $s = \sqrt{s^2}$

$$\sqrt{2,916666667}= 1,7078251277$$

compute $\bar{x} - 2\times s$

$$9,25 - 2 * 1,7078251277 =5,8343497447$$

compute $\bar{x} + 2\times s$

$$9,25 + 2 * 1,7078251277 = 12,6656502553$$

state how many of the four observations lie in the interval $(\bar{x} - 2\times s,\, \bar{x} + 2\times s)$

$$0\: \text{observations are within the interval}$$

# On Your Marks, Get Set, Infer!

## Introduction to Sampling

Statistics are often used in science to generalize data collected from a small sample of a population to a much larger population. This process is called sampling design and involves questions such as whether to use a sample at all, what process of sampling to use, what type of sample to use, and how large a sample to use.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/sample_and_population.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/sample_and_population.png)

Fig. 22: Population And Sample - Graphic Design. (n.d.). [Illustration]. [https://www.pngkey.com/detail/u2y3q8q8e6o0u2t4_population-and-sample-graphic-design/](https://www.pngkey.com/detail/u2y3q8q8e6o0u2t4_population-and-sample-graphic-design/)

Before we go in-depth, we have to introduce some relevant terminology. The population is the entire group that we want to investigate. A set of similar items characterizes the population that can then be compared among the individual units of the population. A subset of the population that represents the population is called a sample. That sample is selected for further investigation whose results infer new insights about the population as a whole. On the contrary, census is a systematic method for a complete enumeration as every individual unit of the population is researched.

As the needed prerequisite, the resource investment and the outcome differ between Census and Sampling. It is important to build an intuition whether the choice for an approach is appropriate for the defined objective. To the right, we see a summary of the key arguments that guide the data aggregation design.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2012.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2012.png)

Fig. 23: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

As the target population represents the collection of units of interest, the census refers to a total enumeration of the population. In the census, all the population units are investigated, and therefore no sampling error occurs while applying estimations of population parameters. For larger population size $N$ the implementation of a census becomes less and less feasible. 

Even for the implementation of a census, there are different other error sources as the non-sampling error. This type of error appears, for example, if the interviews misunderstand or bias the respondent of a survey.

We start a sample survey to gather new data about a population (tend to be based on samples rather than census) by selecting a certain number of population members to form the sample we want to investigate. This kind of sample survey can be executed by a variety of methods such as e-mail questionnaires, online questionnaires (ex. Google Forms), telephone or face-to-face interviews.

### Types of errors

The research goal normally is to retrieve as accurate as possible information of the sample population to generalize the insights to the population as a whole. For measuring the accuracy it is also of interest how large the variation between a true value of a parameter in the population of the variables of interest is compared to the measured value of the sample. For this evaluation, the metric **total error** is used. The total error consists of two different error types.

**Sampling error**

The sampling error occurs due to random variation in the sampling process by choosing randomized sampling units. For probability sampling, an estimation of the sampling error is feasible due to the statistical properties. 

**Non-Sampling error** 

The non-sampling error is attributable to unavoidable failures of the sampling scheme. This kind of error in general is very hard to quantify. The non-sampling error can be further divided into two categories:

- possible reasons for a **selection bias:** sampling frame not equal to target population, cases in which the sampling scheme is not strictly adhered to or non-response bias of parts of the target population
- possible reasons for a **response bias:** This can occur in all interactions between the questioner and the interviewee. Whether it is a directional phrase, a manner of posture, or the loss of questionnaires.

**Pilot survey** enables the questioner for both types of errors to control the error more effectively. It is possible to determine the standard error attached to different kinds of questions and also to investigate non-sampling questions as whether people understand the questionnaire or whether the interviewers worked well?

## Sampling techniques

Sampling describes the process in which the fraction of a population is selected. The sample should still represent the characteristics of the population. There are different methods to retrieve the sample units out of the larger population. The sampling techniques are divided into two major categories, one is the non-probability sampling techniques and the other is the probability sampling techniques.

### Non-probability sampling techniques

As the umbrella term already reveals individual units are selected by non-random criteria. Thereby not every individual has a chance of being included as the inclusion criteria are predefined. With this kind of techniques, it is impossible to measure the sampling error. In general, the application of a non-probability method is more economical and accessible, with the downside of having a higher risk of a sampling bias. 

We will look at four sampling methods using non-probability techniques. We will always use an illustrative example that includes a population of 25 students. In each case, 5 students are to be assigned to a class, which can be labeled using the letters A to E. The students are then assigned to a class. The numbers visualized with bold font are our selected units of the samples.

$$\begin{array}{|c|c|c|c|c|}\hline \mathrm{A} & \mathrm{B} & \mathrm{C} & \mathrm{D} & \mathrm{E} \\\hline 1 & 6 & 11 & 16 & 21 \\2 & 7 & 12 & 17 & 22 \\3 & 8 & 13 & 18 & 23 \\4 & 9 & 14 & 19 & 24 \\5 & 10 & 15 & 20 & 25 \\\hline\end{array}$$

**Convenience sampling**

This method obtains a sample of convenient elements. That happens because the selected units are at the right place at the right time. In the example of our classes the sample units consist of $16,17,18,19\: \text{and}\:20$ so basically all of the class D. That is the case because the survey with the students was committed in the time slot when class D was on campus.

$$\begin{array}{|c|c|c|c|c|}\hline \mathrm{A} & \mathrm{B} & \mathrm{C} & \mathrm{D} & \mathrm{E} \\\hline 1 & 6 & 11 & \mathbf{1 6} & 21 \\2 & 7 & 12 & {\mathbf{1 7}} & 22 \\3 & 8 & 13 & {\mathbf{1 8}} & 23 \\4 & 9 & 14 & {\mathbf{1 9}} & 24 \\5 & 10 & 15 & {\mathbf{2 0}} & 25 \\\hline\end{array}$$

The convenience sampling is the simplest in execution and, therefore, the most economical approach. However, as we have seen from our example, the person conducting the survey only has to come once. This, in turn, leads to a bias in selecting the units (perhaps the class consisted exclusively of medical students), which leads to a deterioration of the sample's representativeness.

**Judgemental sampling**

As the name suggests, in judgmental sampling, there is one person, usually an expert or the researcher, who decides who will be included in the sample. In our example, a researcher would categorize classes B and E as typical and convenient and would retrieve from their 5 students based on typicality and convenience. 

$$\begin{array}{|c|c|c|c|c|}\hline \mathrm{A} & \mathrm{B} & \mathrm{C} & \mathrm{D} & \mathrm{E} \\\hline 1 & \mathbf{6} & 11 & {1 6} & 21 \\2 & 7 & 12 & {1 7} & 22 \\3 & 8 & 13 & {{1 8}} & \mathbf{23} \\4 & 9 & 14 & {{1 9}} & \mathbf{24} \\5 & \mathbf{10} & 15 & {{2 0}} & \mathbf{25} \\\hline\end{array}$$

Similar to convenience sampling the judgemental sampling is quite a cost- and resource-efficient approach. But also the ability of generalization is quite low and it has the property of a subjective preprocessing due to the judgment of the researcher.

**Quota sampling**

Quota sampling is basically a restricted two-step judgemental or convenience sampling. We have quotas that control the distribution of the units of a sample over the different categories within a population as first step. The second step consists of selecting a sample element again based on convenience or judgment.

$$\begin{array}{|c|c|c|c|c|}\hline \mathrm{A} & \mathrm{B} & \mathrm{C} & \mathrm{D} & \mathrm{E} \\\hline 1 & \mathbf{6} & 11 & {1 6} & 21 \\\mathbf{2} & 7 & 12 & {1 7} & 22 \\3 & 8 & 13 & {{1 8}} & {23} \\4 & 9 & 14 & {{1 9}} & \mathbf{24} \\5 & {10} & \mathbf{15} & \mathbf{20} & {25} \\\hline\end{array}$$

In our particular case, a quota would refer to the restriction that every class has to be represented once within the sample. Within a class the individual are selected by  one of the methods introduced above.

Quota sampling is improving the representativeness as the sample can be controlled for certain characteristics, without really being able to guarantee it. It still suffers from selection bias as the second step relies on either the judgemental or convenience sampling.

**Snowball sampling**

At the snowball sampling the inital group of attendees are usually random selected and after the interview they are asked to identify others that fulfill the target population characteristics. So the sample increases by referrals. Applying it to our example we would start with No. 6 as interviewer which later on refers to No. 12, who refers to No. 20, No. 13 and No. 9.

$$\begin{array}{|c|c|c|c|c|}\hline \mathrm{A} & \mathrm{B} & \mathrm{C} & \mathrm{D} & \mathrm{E} \\\hline 1 & \mathbf{6} & 11 & {1 6} & 21 \\{2} & 7 & \mathbf{12} & {1 7} & 22 \\3 & 8 & \mathbf{13} & {{1 8}} & {23} \\4 & \mathbf{9} & 14 & {{1 9}} & \mathbf{24} \\5 & {10} & {15} & {20} & {25} \\\hline\end{array}$$

Snowball sampling is a simple and low-cost way to increase the chance of modelling a sample with desired properties in the population.

### Probability (random) sampling techniques

Probability sampling includes every member of the population to be possibly selected. For getting the best representation of the whole population, probability sampling techniques are state-of-the-art. These kinds of approaches also enables you to estimate the margins of sampling error. For executing probability sampling we need a sampling frame that consists of a list of all population elements. For the sampling frame we have to prove the following:  

- **adequate** to represent the target population?
- **complete** - are there any missing units?
- **accurate** -  are we researching dynamic populations?
- **convenient** - is the sampling frame readily accessible?

**Simple random sampling**

Every element in the population has a equal and known probability to be selected. That also implies that every element is selected independently of every other element. SRS is very simple and easy to execute. Nevertheless, the creation of the sampling frame may be associated with inaccuracies, such as lower precision and no guarantee of the representative of the sample.

In our previously given example of five classes, each with five students, the SRS would simply select five numbers between 1 and 25, regardless of class. This may result in random students of one class (in our example, class D) not being represented.

$$\begin{array}{|c|c|c|c|c|}\hline \mathrm{A} & \mathrm{B} & \mathrm{C} & \mathrm{D} & \mathrm{E} \\\hline 1 & \mathbf{6} & 11 & {1 6} & 21 \\{2} & 7 & {12} & {1 7} & 22 \\3 & 8 & \mathbf{13} & {{1 8}} & {23} \\4 & \mathbf{9} & 14 & {{1 9}} & {24} \\\mathbf5 & {10} & {15} & {20} & \mathbf{25} \\\hline\end{array}$$

**Systematic sampling**

In systematic sampling, you need a sampling interval, $i$, which determines how many population elements you skip from a random selected starting point until you take the next element into the sample. This process is repeated from the new point until one is with the interval steps through the entire population. The aforementioned interval is obtained by dividing the population size, $N$, by the sample size $n$, rounding to the nearest integer. 

Depending on the characteristics of the order, systematic sampling can vary the representativeness of the population. If the order of the elements is related to the characteristics under study, it improves them, but if the order leads to cyclic patterns, it can also worsen the representativeness.

For our example we want to have $5$ samples out of a population size of $25$.

$$i=\frac{N}{n}=\frac{25}{5}=5$$

Now we choose a random starting number between $1,5$. Let's say we choose $4$.

$$4,\\(4+5)=9,\\(9+5)=14,\\(14+5)=19 \\(19+5)=24$$

$$\begin{array}{|c|c|c|c|c|}\hline \mathrm{A} & \mathrm{B} & \mathrm{C} & \mathrm{D} & \mathrm{E} \\\hline 1 & {6} & 11 & {1 6} & 21 \\{2} &{7} & {12} & {1 7} & 22 \\3 & 8 & {13} & {{1 8}} & {23} \\\mathbf{4} & \mathbf{9} & \mathbf{14} & \mathbf{{1 9}} & \mathbf{24} \\5 & {10} & {15} & {20} & {25} \\\hline\end{array}$$

**Stratified sampling**

Stratified sampling consists of splitting the **population into subgroups, the so-called strata**. Each population element should be assigned exclusively to one subgroup. From the strata, sample elements are then selected for the sample using a random procedure, usually SRS.

Within a subgroup, the sample elements should be as heterogeneous as possible, with the elements differing as much as possible between subgroups, that is, being as heterogeneous as possible. In addition, the stratification factors should be as similar as possible to the characteristics of interest.

In **proportionate stratified sampling**, the proportion of stratum present in the sample should be proportional to how often the stratum occurs in the total population. **In disproportionate (optimal) stratified sampling** and the proportional ratio in the total population, the standard deviation of the distribution of the characteristic of interest among all the elements in that stratum is also taken into account.

Summarized, the stratified sampling maintains a high precision as it encounters all-important subpopulations, even if selecting the stratification factors is difficult.

In our example, it can be applied in that one random element is selected from each class A to E corresponding to our stratum.

$$\begin{array}{|c|c|c|c|c|}\hline \mathrm{A} & \mathrm{B} & \mathrm{C} & \mathrm{D} & \mathrm{E} \\\hline 1 & \mathbf{6} & 11 & {1 6} & 21 \\{2} & 7 & {12} & {1 7} & 22 \\3 & 8 & \mathbf{13} & {{1 8}} & {23} \\4 & {9} & 14 & \mathbf{19} & {24} \\\mathbf5 & {10} & {15} & {20} & \mathbf{25} \\\hline\end{array}$$

**Cluster sampling**

Cluster sampling consists of splitting the **population into subgroups, the so-called clusters**. Each population element should be assigned exclusively to one cluster. A random sample (based on probability sampling) of clusters is then selected. 

When using the one-stage cluster method, all elements of a cluster are included in the sample. In contrast, the two-stage cluster method selects elements from the elements within a cluster in a probabilistic manner.

Within a cluster, the individual elements should be as heterogeneous as possible, while the clusters should be as homogeneous as possible among themselves. In the best case, the clusters are a kind of smaller representation of the total population. In probability proportionate to size sampling, the clusters are sampled with probability proportional to size. In the next step, the likelihood of selecting an element out of the cluster varies inversely with the size of the cluster.

Although this sampling method is easy to implement, one must reckon with the disadvantages that the precision of the results is not really high.

In our example, between our five clusters A-E, we would randomly select three, from which we would select one to two individual elements.

$$\begin{array}{|c|c|c|c|c|}\hline \mathrm{A} & \mathrm{B} & \mathrm{C} & \mathrm{D} & \mathrm{E} \\\hline 1 & \mathbf{6} & 11 & {1 6} & 21 \\{2} & 7 & {12} & {1 7} & 22 \\3 & 8 & \mathbf{13} & {{1 8}} & {23} \\4 & {9} & 14 & \mathbf{19} & {24} \\5 & \mathbf{10} & {15} & \mathbf{20} & {25} \\\hline\end{array}$$

**Multistage sampling**

In multistage sampling, the sampling selection process is distributed over several successive stages. This is mainly used for substantial populations so that in the first step, we select larger groups, called primary units, to which sampling is applied again until we have the base units in the last step. 

In the example of cluster sampling, a number of main clusters would be selected in the first place, within which clusters would also arise again.Different sampling methods can be combined with each other.

For our example, it would mean a set of classes (e.g., A-Z). From these classes, a cluster is created, which includes the classes A-E. The cluster is again selected via, e.g., stratified sampling. From this cluster again via, e.g., stratified sampling, single elements are selected so that from cluster A-E, five single elements are fixed as a result.

## Sampling Distributions

The simple random sample processes result in randomly composing samples to eliminate selection bias. This leads to the fact that one cannot estimate which elements a sample contains.

To illustrate the concept of sampling distributions, let's examine the topic with an example, which has a population size of $N=6$ with the elements $A,B,C,D,E$ and $F$. Then, applying a random sample process without replacement from the units and with a sample size of $n=2$, we have $15$ different sample options:

$$\begin{array}{l}
\mathrm{AB}, \mathrm{AC}, \mathrm{AD}, \mathrm{AE}, \mathrm{AF}, \mathrm{BC}, \mathrm{BD}, \mathrm{BE} \\
\mathrm{BF}, \mathrm{CD}, \mathrm{CE}, \mathrm{CF}, \mathrm{DE}, \mathrm{DF}, \mathrm{EF}
\end{array}$$

Since we are applying SRS, each sample has a probability of selection of $\frac{1}{15}$.

Populations have properties that are of interest to us such as the mean $\mu$ or the variance $\sigma^2$, which are also called parameters. If the data of a population are not available, the parameter values are unknown.

In order to estimate these unknown parameter values on the basis of the known sample data, there is the so-called 'statistical inference'. We use a statistic (called estimator) to calculate a point estimate of the parameter values from the sample units. 

The variable we are interested in is monthly income, whose values are distributed over the total population $(n=6)$ as follows:

$$\begin{array}{l|c|c|c|c|c|c}\text { Individual } & \mathrm{A} & \mathrm{B} & \mathrm{C} & \mathrm{D} & \mathrm{E} & \mathrm{F} \\\hline \text { Monthly income in } € 000 \mathrm{~s} & 3 & 6 & 4 & 9 & 7 & 7\end{array}$$

For estimating the unknown population mean $\mu$  we will use the known sample mean $\bar{X}$, which is computable through:

$$\overline{{X}}=\frac{1}{n} \sum_{i=1}^{n} {X}_{i}$$

In our example we can of course calculate this, but it serves to illustrate how the process would look like if we did not know the parameters. An example of the sample mean of the combination 'AE' would look like this:

$$A=3000,\: E=7000\rightarrow \frac{3000+7000}{2}= €5000$$

Different combinations of samples lead to different sample means. In the following we list the sample means $\bar{x}$ of all possible combinations of samples of the values $\bar{X}$: (all values are in €000s)

$$\begin{array}{c|c|c|c|c|c|c|c|c}
\text { Sample } & \text { AB } & \text { AC } & \text { AD } & \text { AE } & \text { AF } & \text { BC } & \text { BD } & \text { BE } \\
\hline \text { Values } & 3,6 & 3,4 & 3,9 & 3,7 & 3,7 & 6,4 & 6,9 & 6,7 \\
\hline \bar{x} & 4.5 & 3.5 & 6 & 5 & 5 & 5 & 7.5 & 6.5
\end{array}$$

$$\begin{array}{c|c|c|c|c|c|c|c}\text { Sample } & \mathrm{BF} & \mathrm{CD} & \mathrm{CE} & \mathrm{CF} & \mathrm{DE} & \mathrm{DF} & \mathrm{EF} \\\hline \text { Values } & 6,7 & 4,9 & 4,7 & 4,7 & 9,7 & 9,7 & 7,7 \\\hline \bar{x} & 6.5 & 6.5 & 5.5 & 5.5 & 8 & 8 & 7\end{array}$$

The values of $\bar{X}$ have a range of $[3.5,8]$, depending on the sample values. Compared to the true population mean $\mu=6$, we thus have a high variance between the sample mean and population mean.

We will now illustrate how the maximum possible absolute deviation of the sample mean, and the population mean $|\bar{x}-\mu|$ behaves. 

$$\begin{array}{c|c|c|c}\max |\bar{x}-\mu| & \text { Range of } \bar{x} & \text { Number of samples } & \text { Probability } \\\hline 0 & \bar{x}=6 & 1 & 0.067 \\0.5 & 5.5 \leq \bar{x} \leq 6.5 & 6 & 0.400 \\1 & 5 \leq \bar{x} \leq 7 & 10 & 0.667 \\1.5 & 4.5 \leq \bar{x} \leq 7.5 & 12 & 0.800 \\2 & 4 \leq \bar{x} \leq 8 & 14 & 0.933 \\2.5 & 3.5 \leq \bar{x} \leq 8.5 & 15 & 1.000\end{array}$$

From this, we can conclude that, for example, the probability that the sample mean is equal to the population mean is $6.7 \%$ or that $80\%$ of the sample mean is within $1.5$ units of the population mean $\mu$.

We can also show every frequency for each possible value of $\bar{x}$ as frequency distribution:

$$\begin{array}{c|c|c}
\bar{x} & \text { Frequency } & \text { Relative frequency } \\
\hline 3.5 & 1 & 1 / 15=0.067 \\
4.5 & 1 & 1 / 15=0.067 \\
5.0 & 3 & 3 / 15=0.200 \\
5.5 & 2 & 2 / 15=0.133 \\
6.0 & 1 & 1 / 15=0.067 \\
6.5 & 3 & 3 / 15=0.200 \\
7.0 & 1 & 1 / 15=0.067 \\
7.5 & 1 & 1 / 15=0.067 \\
8.0 & 2 & 2 / 15=0.133
\end{array}$$

This frequency distribution equals the sampling distribution of $\bar{X}$. The sampling is a central concept in statistics to evaluate how good an estimator is. This metric evaluates how close the estimator is to the total population parameter of interest.

In summary, $\bar{X}$ is the estimator of the population mean $\mu$ and the value that $\bar{X}$ takes $\bar{x}$ is a point estimate.

## Sampling distribution of the sample Mean

With the parameters mean and variance of a sampling distribution we can assess how good an estimator is. 

### The sampling distribution mean

We will first look at the mean to create a reliable estimator. It should be noted that the average value of an estimator looping overall sample possibilities should be equal to the value of the population mean $\mu$. In reference to our previously presented example:

$$\begin{array}{c|c|c}\bar{x} & \text { Frequency } & \text { Product } \\\hline 3.5 & 1 & 3.5 \\4.5 & 1 & 4.5 \\5.0 & 3 & 15.0 \\5.5 & 2 & 11.0 \\6.0 & 1 & 6.0 \\6.5 & 3 & 19.5 \\7.0 & 1 & 7.0 \\7.5 & 1 & 7.5 \\8.0 & 2 & 16.0 \\\hline \text { Total } & 15 & 90.0\end{array}$$

The mean of the sampling distributions (the weighted average of all possible sampling distributions) corresponds to $\frac{90}{15}=6$ and therefore equals the population mean $\mu$. 

An important property that distinguishes the sampling distribution from other distributions is that it summarizes an entire sample rather than just an individual observation. The mean of the sampling distribution is called the expected value of the estimator, denoted by $E( \cdot )$. Hence the expected value of the sample mean is $E(\bar{X})$. 

As long the expected value equals to the parameter being estimated, the estimator is called an unbiased estimator. Our example is a good example of a population parameter being estimated by its sample counterpart because of $E(\bar{X})=6=\mu$. 

In the case of SRS the sample mean $\bar{X}$ always corresponds to an unbiased estimator despite the sample size $n$ or distribution of the population. 

### The sampling distribution variance

A working estimator is definitely relevant, but it does not say anything about the dispersion of the sampling distribution of the estimator. The estimator should be as close as possible to the true parameter value so that we have the smallest possible variance.

The sampling variance is defined as the mean of the squared deviations about the sampling mean. To recall our example:

$$\begin{array}{c|c|c|c|c}\bar{x} & \bar{x}-\mu & (\bar{x}-\mu)^{2} & \text { Frequency } & \text { Product } \\\hline 3.5 & -2.5 & 6.25 & 1 & 6.25 \\4.5 & -1.5 & 2.25 & 1 & 2.25 \\5.0 & -1.0 & 1.00 & 3 & 3.00 \\5.5 & -0.5 & 0.25 & 2 & 0.50 \\6.0 & 0.0 & 0.00 & 1 & 0.00 \\6.5 & 0.5 & 0.25 & 3 & 1.75 \\7.0 & 1.0 & 1.00 & 1 & 1.00 \\7.5 & 1.5 & 2.25 & 1 & 2.25 \\8.0 & 2.0 & 4.00 & 2 & 8.00 \\\hline & & \text { Total } & 15 & 24.00\end{array}$$

The sampling variance equals $\frac{24}{15}=1.6$. Since we also have the data on the total population, we can also calculate the population variance $\sigma^2$ for illustration:

$$\begin{array}{c|c|c|c|c}x & x-\mu & (x-\mu)^{2} & \text { Frequency } & \text { Product } \\\hline 3 & -3 & 9 & 1 & 9 \\6 & 0 & 0 & 1 & 0 \\4 & -2 & 4 & 1 & 4 \\9 & 3 & 9 & 1 & 9 \\7 & 1 & 1 & 2 & 2\end{array}$$

The population variance equals to $\sigma^2=\frac{24}{6}=4$. 

Now we can look at the relationship between $\sigma^2$ and the sampling variance. If sampling is performed without replacement, then the variance can be calculated and correlations can be inferred:

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/C1C2231A-991C-4239-ACB1-936FBCAF797F.jpeg](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/C1C2231A-991C-4239-ACB1-936FBCAF797F.jpeg)

Fig. 24: sampling variance

More formally:

$$\operatorname{Var}(\bar{X})=\frac{N-n}{N-1} \times \frac{\sigma^{2}}{n}$$

Therefore we get for our example:

$$\operatorname{Var}(\bar{X})=\frac{6-2}{6-1} \times \frac{4}{2}=1.6$$

Furthermore, we call the standard deviation of our sampling distribution the so-called standard error, which, as in the calculation of the standard deviation, is the root of the underlying variance:

$$\text { S.E. }(\bar{X})=\sqrt{\operatorname{Var}(\bar{X})}=\sqrt{\frac{N-n}{N-1} \times \frac{\sigma^{2}}{n}}=\sigma_{\bar{X}}$$

The sampling variance has some properties that can be derived from the equation. For example, it can be seen that as the sample size $n$ increases, the variance also decreases and the precision of the sample improves. It can also be seen that a very small fraction of $\frac{n}{N}$ makes the first part of the equation $\frac{N-n}{N-1}\approx1$ become irrelevant for the computation. In this case, the standard error depends exclusively on the sample size. Simplified, this could be stated as follows:

$$\operatorname{Var}(\bar{X})=\frac{N-n}{N-1} \times \frac{\sigma^{2}}{n} \approx \frac{\sigma^{2}}{n}=\frac{\operatorname{Var}(X)}{n}$$

Moreover, one can conclude that, as it seems intuitive if the variance within the population is large, the variance of the sampling distribution will be increased.

To illustrate this again with our example, here is the calculation of the sampling distribution with a sample size of $2$ and $4$.

$$\begin{array}{c|c|c}\bar{x} & n=2 & n=4 \\\hline 3.50 & 1 & - \\4.50 & 1 & - \\5.00 & 3 & 2 \\5.25 & - & 1 \\5.50 & 2 & 1 \\5.75 & - & 3 \\6.00 & 1 & 1 \\6.25 & - & 2 \\6.50 & - & 3 \\6.75 & - & 1 \\7.00 & 1 & - \\7.25 & - & 1 \\7.50 & 1 & - \\8.00 & 2 & -\end{array}$$

If $n=2:$

$$\operatorname{Var}(\bar{X})=\frac{6-2}{6-1} \times \frac{4}{2}=1.6$$

If $n=4:$

$$\operatorname{Var}(\bar{X})=\frac{6-4}{6-1} \times \frac{4}{4}=0.25$$

Even though increased precision is desirable, a larger sample size is associated with increased resource overhead.

### Sampling from the normal distribution

Since we found that the mean of $\bar{X}$ $E(X)$ corresponds to the variance $\frac{Var(X)}{n}$ for any population distribution of $X$, the question arises as to what form the sampling distribution takes. Since this depends on $X$ and is mostly unknown, it is mostly not definable. However, if $X$ already had a normal distribution, then $\bar{X}$ will also correspond to a normal distribution.

Thus, if we obtained $\left\{X_{1}, \ldots, X_{n}\right\}$ by random sampling of a normal distribution with mean$\mu$and $\sigma^2$, the sample distribution corresponds to the following:

$$\bar{X} \sim N\left(\mu, \frac{\sigma^{2}}{n}\right)$$

So ${E}(\bar{X})={E}(X)=\mu$, but only a multitude of samples will have the $\mu$ and not an individual sample. We have already seen this property in our previous examples. The formulas, as well as the effects of sample size on sampling distribution, remain as already mentioned.

We will now visualize what we have worked out with a diagram in order to understand the effects graphically. We will start from the following:

$$X \sim N(5,1)$$

$$\bar{X} \sim N(5,\frac{1}{n})$$

The following graphs show the sampling distribution with sample sizes of $n=5,\:n=20,\:\text{and}\:100 \:for \:\bar{X}$, centering at the mean of $5$.

We can see that the dispersion decreases as the sample size increases.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2013.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2013.png)

Fig. 25: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

## Confidence intervals

A point estimate is always a best estimate of an unknown parameter, such as, the population mean $\mu$, even if on average the sample mean is equal to the population mean. However, since the mean of a sample can vary, this estimate of a parameter based on the sample is always associated with uncertainty (imprecision). One tries to quantify this uncertainty by converting the point estimate into an interval estimate. 

Formally, an $x\%$  confidence interval covers the unknown parameter with $x\%$  probability over repeated samples.

The smaller the confidence interval is, the more reliable are their estimates. These intervals can be reduced by lowering the level of confidence associated with the interval, which of course reduces the quality of the estimations, or by increasing the sample size, which requires resources.

If we assume that we have either $(A)$ $\sigma$ or, for unknown $(B)$ $\sigma$, a large sample size (n $\geq$ 50), the formula for the endpoints of a confidence interval for a single sample mean corresponds to:

$$A.\quad\bar{x} \pm z \times \frac{\sigma}{\sqrt{n}}\:\: \:\text{and}\:\:\: 
B. \quad \bar{x} \pm z \times \frac{s}{\sqrt{n}}$$

$\bar{x}$ = the sample mean, $\sigma$ = population standard deviation, $s =$ sample standard deviation, $n =$  sample size and $z$ = confidence coefficient, which reflects the confidence level.

### Influences on the margin of error

We can see the confidence interval of a means as follows:

$$\text { best guess } \pm \text { margin of error }$$

Where $\bar{x}$ is the best guess (estimation) and the margin error corresponds to the already mentioned A or B, depending on the presence of $\sigma$. As the equation illustrates to us, the margin of error has three influencing variables , each of which affects its magnitude:

1. an increase of the sample size leads to an improvement of the precision of the point estimates and thus to a decrease of the confidence interval.

    $$\text { as } n \uparrow \quad\Rightarrow \text { margin of error } \downarrow \quad \Rightarrow \text { width } \downarrow$$

2. If the $\sigma$ or $s$ is increased, the variation within the population is also increased and the possibility of making suitable estimates is worsened, and the confidence interval is increased accordingly.

    $$\text { as } \sigma \uparrow \quad \Rightarrow \text { margin of error } \uparrow \quad\Rightarrow \text { width } \uparrow$$

3. Since an increase in the level of confidence is equivalent to a larger confidence coefficient, the corresponding interval also becomes larger.

    $$\text { as confidence level }  \uparrow \quad \Rightarrow \text { margin of error } \uparrow \quad\Rightarrow \text { width } \uparrow$$

### Confidence coefficients

For a $95\%$ confidence interval, the z-score is $1.96$. This leads to:

$$A. \quad \bar{x} \pm 1.96 \times \frac{\sigma}{\sqrt{n}} \quad \text{and} \quad B. \quad \bar{x} \pm 1.96 \times \frac{s}{\sqrt{n}}$$

Other degrees of confidence are also no problem, but require a different confidence coefficient. For a large $n$, the coefficient is obtained from the standard normal distribution. Um den coefficient zu berechnen, berechnet man die Fläche von dem Start der Verteilung bis zum positiven z-value. The resulting area is then used to reconstruct the corresponding z-value, which then corresponds to the z-score for the associated confidence interval. This can be seen in the following example for the confidence interval:

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/EDC30406-08B2-4452-AB8D-6D1266F0007C.jpeg](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/EDC30406-08B2-4452-AB8D-6D1266F0007C.jpeg)

Fig. 26: Distribution of sample mean and identifying area B

$$A_{L}=\frac{1+C L}{2}=\frac{1+0.95}{2}=\frac{1.95}{2}=0.975\\
$$

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2014.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2014.png)

Fig. 27: z-Table Cutout. (n.d.). [Graph]. [http://www.z-table.com/uploads/2/1/7/9/21795380/8573955.png?759](http://www.z-table.com/uploads/2/1/7/9/21795380/8573955.png?759)

As the section of the z-table shows, the z-score for $0.975$ equals to $1.96$.

We will now illustrate the concept again with an example. We use a designer jeans producing company, where we perform sampling to estimate the average price that retailers charge for the jeans.  A randomly selected sample of retailers, with an $\sigma$ of $3.25$ resulted in the following statistics:

$$\bar{x}=£ 25.75 \quad \text { and } \quad n=60$$

With a $95\%$ confidence interval for the mean of the retailer, the price lies in the interval of:

$$25.75 \pm 1.96 \times \frac{3.25}{\sqrt{60}} \Rightarrow(£ 24.93, £ 26.57)$$

When the size of the random sample from which we estimate $\bar{x}$ increases to $n=100$, the interval decreases despite the confidence of $95\%$ remaining the same.

$$25.75 \pm 1.96 \times \frac{3.25}{\sqrt{100}} \quad \Rightarrow \quad(£ 25.11, £ 26.39)$$

If we again take the first sample size of $n=60$ and set the standard deviation to $\sigma=3.75$, then the $95\%$ confidence interval becomes larger.

$$25.75 \pm 1.96 \times \frac{3.75}{\sqrt{60}} \Rightarrow(£ 24.80, £ 26.70)$$

If we again have the sample size of $n=60$ and assume that $\sigma=3.25$, a $99\%$ confidence interval is larger than with the same metrics and smaller confidences.

$$25.75 \pm 2.576 \times \frac{3.25}{\sqrt{60}} \quad \Rightarrow \quad(£ 24.67, £ 26.83)$$

# To p Or Not To p?

## Statistical Juries

In decision theory, hypotheses are often tested in a binary way, i.e. two hypotheses are compared. Here, $H_0$ corresponds to the null hypothesis, which is opposed to $H_1$, the so-called alternative hypothesis. The binary decision consists of reject $H_0$ or fail to reject $H_0$, which we will illustrate with a court trial example.

In a court case, someone is accused in a trial and with the help of an independent jury it is to be determined whether this person is innocent ($H_0$) or guilty ($H_1$). Since the presumption of innocence applies in our case, the null hypothesis corresponds to innocent. This presumption exists only until the jury feels it has enough evidence to prove the guilt of the accused person. In the statistical world, this is called the significance level, i.e., the amount of evidence needed to reject the null hypothesis $H_0$.

The jury follows certain decision rules to reach its verdict, considering, on the one hand, the incontinence of innocence to reject the null hypothesis (e.g., through a conviction) but also whether the failure to prove guilt over certain required evidence, which fails to reject the null hypothesis. It is important to note that the failure does not correspond to a proof of innocence but shows a lack of evidence.

One important note is still overdue, and that is that juries can also make wrong decisions that can have wider implications. Hypothesis testing is therefore always associated with the possibility of making mistakes, which we will explain further in the coming sections.

## Type I and Type II errors

In all hypothesis tests carried out, it is possible to come to wrong conclusions, which will lead to a wrong decision. One tries to minimize the probability of the occurrence of an error as best as possible. A distinction is made between a Type I error, which corresponds to the rejecting of $H_0$, although $H_0$ is true (false positive) and the Type II error, which corresponds to the failing to reject $H_0$, although $H_0$ is false. (false negative)

The probability of the occurrence of the Type I error is quantified with $\alpha$, the occurrence of the Type II error with $\beta$. Both errors are to be avoided, whereby the context often has a certain tolerance towards one of the two errors. Most of the time, the Type I error is considered to be more serious and thus there is a tendency to minimize it.

**The possible decision space for would be as follows:**

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Latex_Table.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Latex_Table.png)

Fig. 28: Decision matrix

If, as in our previous example, the null hypothesis corresponds to innocence, a Type I error case would convict someone who is in fact innocent.

The power of a test equals the probability that the test will reject a false null hypothesis which is evaluated by $1-\beta$. (complement of Type II error) Power is also the indicator of how good the ability of the test to reject a false $H_0$. Accordingly, try to find a test as powerful as possible for each test situation. Unlike $\alpha$, we cannot control the test power except to increase the sample size $n$, which inevitably leads to an improvement in accuracy. The executed concepts can be executed as conditional probabilities:

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/ql_b93c570d5e3b88dae461c04856818c9d_l3.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/ql_b93c570d5e3b88dae461c04856818c9d_l3.png)

Fig. 29: Decision boundaries

Therefore:

$$P\left(\mathrm{H}_{0}\right. not\: rejected \mid \mathrm{H}_{0} is\: true )=1-\alpha \\P\left(\mathrm{H}_{0}\right. rejected \mid \mathrm{H}_{0} is\: true )=\alpha\\
P\left(\mathrm{H}_{0}\right. not\: rejected \mid \mathrm{H}_{1} is\: true )=\beta\\
P\left(\mathrm{H}_{0}\right. rejected \mid \mathrm{H}_{1} is\: true )=1-\beta$$

Other things being equal, $\alpha$ increases as $\beta$ decreases and vice versa.

### Significance Level

Since we can define how high the probability of occurrence of the Type I error should be, we still have to specify it. Normally we test for a significance level of $100\alpha\%$ for the range of $\alpha$ from $\alpha \in[0,1]$. The default value of $\alpha$ equals to $\alpha = 0.05$. This value is adjusted depending on the hypothesis being tested.

If we use the levels and their intervals introduced in the confidence level topic as an example, then the significance level can be seen as the complementary part to the confidence level, as the following examples illustrate:

- 90 % confidence level ⇒ 10 % significance level
- 95 % confidence level ⇒ 5 % significance level
- 99 % confidence level ⇒ 1 % significance level

## P-values, effect size and sample size

We will now introduce the p-values that will help us determine whether we will retain or reject the null hypothesis. The p-value is a unit of measurement to enumerate the discrepancy between the established null hypothesis $H_0$ and the data evidence. It corresponds to the probability of the event that the "test statistic" takes the observed value or more extreme (i.e., improbable) values below $H_0$. Simplified, you can remember the following:

- a small p-value indicates a null hypothesis $H_0$, which is not supported by the data
- a large p-value indicates a null hypothesis $H_0$ supported by the data

P-values is thus a risk metric for whether to reject the null hypothesis.

**Example:**

Given is an experiment that describes the average income (in €000s) within a community. The income is modeled as follows: $N(\mu,25)^2$ and a random sample of $n=25$ is taken and examined, resulting in $\bar{x}=17$. Independent of the data obtained, three economists make the following statements, which we will interpret.

- Christine Lagarde claims the mean income is $\mu=16$
- Yi Gang claims the mean income is $\mu=15$
- Jay Powell claims the mean income is $\mu=14$

We assess the statements based on the following distribution: $\bar{X} \sim N\left(\mu, \sigma^{2} / n\right)=N(\mu, 1)$.

If Christine Lagarde's statement should be true corresponds: $\bar{X} \sim N(16,1)$. Thus, the observed results $\bar{x}=17$ deviate one standard deviation from $\mu$. This can be considered a typical deviation from the distribution. Nevertheless, there is a small inconsistency between the statement and the data evidence, as the following graph illustrates.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/16_17_p_value.jpg](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/16_17_p_value.jpg)

Fig. 30: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

If Yi Gang's statement is true, thea distribution would look like this $\bar{X} \sim N(15,1)$. The observed value $\bar{x}=17$ now looks a bit extreme, as this is two $\sigma$ away from $\mu$. Thereby the inconsistency of the statement and the data evidence, which is again illustrated by the graph.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/15_17_p_value.jpg](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/15_17_p_value.jpg)

Fig. 31: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

If the statement of Jay Powell should be true, $\bar{X} \sim N(14,1)$. The observed value $\bar{x}$ is extremely extreme, since it is already three standard deviations from $\mu$. Consequently, there is an extremely strong inconsistency between the statement and the evidence based on the data, as it is again shown by the graph.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/14_17_p_value.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/14_17_p_value.png)

Fig. 32: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

Thus, it follows from the statements made:

$$\begin{array}{l}\text { under } \mathrm{H}_{0}: \mu=16, P(\bar{X} \geq 17)+P(\bar{X} \leq 15)=P(|\bar{X}-16| \geq 1)=0.3173\\\text { under } \mathrm{H}_{0}: \mu=15, P(\bar{X} \geq 17)+P(\bar{X} \leq 13)=P(|\bar{X}-15| \geq 2)=0.0455\\\text { under } \mathrm{H}_{0}: \mu=14, P(\bar{X} \geq 17)+P(\bar{X} \leq 11)=P(|\bar{X}-14| \geq 3)=0.0027 \text { . }\end{array}$$

In summary, we reject the hypotheses $\mu=14$ and $\mu=15$ that have been established, since, for example, if the hypothesis  $\mu=14$ were true, we would only obtain a $\bar{x}=17$ with a probability of $0.003$. However, since this has already occurred in a single experiment, the warp is perfectly fine. On the other side, we cannot reject the hypothesis  $\mu=16$, but this does not check its truthfulness, but only does not allow its falsifiability. A statistical test is incapable of accepting a hypothesis.

$$\text { not reject } \neq \text { accept }$$

### Interpretation of p-values

Normally, statistical analyses on data are taken from computers that return a p-value based on the hypothesis test to work with. There are universal regularities for this p-value. In the previous topic concerning the type 1 error, we found that by choosing significance levels $\alpha \in [0,1$ we can control its occurrence. Since the P-values are also probabilities, we can simply compare the values to the preselected benchmark significance level $\alpha$. Since the p-value clarifies whether we should reject our null hypothesis, there is a decision rule that looks like this for the example of $\alpha = 0.05$:

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/p_value_decision.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/p_value_decision.png)

Fig. 33: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

Our decision to reject $H_0$ is true if the condition $p \text { -value } \leq \alpha$ is satisfied. SThus, the size of the p-value is crucial for the rejection or retention of a hypothesis, and because of this, we delve into its two main influencing factors, the effect size and the sample size.

### Effect size influence

The effect size reflects the difference between the expected value when the null hypothesis is true and the value obtained by the experiment. With an increasing difference between the expectation and the observations, the data evidence becomes inconsistent with the $H_0$, making it more likely to be rejected. Simplistically, as the effect size increases, the p-value decreases, which increases the probability of obtaining a p-value below $\alpha.$

**Example:**

Given is an experiment in which a coin is tossed 100 times and the observed number of heads is counted. If we had a result of 50 times heads, we would not doubt that it is a fair coin. Still, there are other options:

- somewhat sceptical that the coin is fair if you observe 40 or 60 heads
- even more sceptical that the coin is fair if you observe 35 or 65 heads
- highly sceptical that the coin is fair if you observe 30 or 70 heads

Thus, the greater the difference between the number of heads and tails that occur (effect size), the greater the evidence that the coin is not fair. So if we test the following:

$$\mathrm{H}_{0}: \pi=0.5 \text { vs. } \mathrm{H}_{1}: \pi \neq 0.5$$

where $\pi=P(\text{heads})$ and for a sample size of $n=100$, we expect 50 times heads and 50 times tails. Since the sample size is fixed, it can be shown that the p-value is strongly dependent on the effect size:

$$\begin{array}{c|c|c|c|c}\text { Observation } & \text { Expectation } & \text { Effect size } & p \text { -value } & \text { Decision if } \alpha=0.05 \\\hline \text { 50 heads \& 50 tails } & \text { 50 heads \& 50 tails } & 0.5-0.5=0 & 1 & \mathrm{H}_{0} \text { is not rejected } \\\text { 55 heads \& 45 tails } & \text { 50 heads \& 50 tails } & 0.55-0.5=0.05 & 0.3682 & \mathrm{H}_{0} \text { is not rejected } \\60 \text { heads \& } 40 \text { tails } & 50 \text { heads \& 50 tails } & 0.6-0.5=0.1 & 0.0569 & \mathrm{H}_{0} \text { is not rejected } \\\text { 70 heads \& 30 tails } & 50 \text { heads \& 50 tails } & 0.7-0.5=0.2 & <0.0001 & \mathrm{H}_{0} \text { is rejected } \\\text { 80 heads \& 20 tails } & 50 \text { heads \& 50 tails } & 0.8-0.5=0.3 & \approx 0.0000 & \mathrm{H}_{0} \text { is rejected }\end{array}$$

One can understand from the example how there is an inverse relationship between the effect size and the p-value.

The example is also an example of a sensitivity analysis, where the sole influence of the effect size on the p-value is analyzed by the fixed sample size.

### Sample size influence

Other things being equal, an increase in sample size should lead to an improvement in the representativeness of the random sample, making the sample population more representative of the total population.

In the context of the coin toss, the observed proportion of heads should converge toward the true probability of heads $\pi$ when $n \rightarrow \infty$. Now we will take a closer look at the influence of the sample size on the p-value. Whereby the p-value decreases as the sample size increases while the effect size remains constant and is not equal to zero.

Remaining with the coin toss example, we illustrate an experiment with at a fixed effect size of $0.1$:

$$\begin{array}{c|c|c|c|c}\text { Observation } & \text { Expectation } & \text { Sample size } & p \text { -value } & \text { Decision if } \alpha=0.05 \\\hline \text { 6 heads \& 4 tails } & \text { 5 heads \& 5 tails } & n=10 & 0.7539 & \mathrm{H}_{0} \text { is not rejected } \\\text { 12 heads \& 8 tails } & \text { 10 heads \& 10 tails } & n=20 & 0.5034 & \mathrm{H}_{0} \text { is not rejected } \\\text { 18 heads \& 12 tails } & \text { 15 heads \& 15 tails } & n=30 & 0.3616 & \mathrm{H}_{0} \text { is not rejected } \\\text { 60 heads \& 40 tails } & 50 \text { heads \& } 50 \text { tails } & n=100 & 0.0569 & \mathrm{H}_{0} \text { is not rejected } \\150 \text { heads \& } 100 \text { tails } & 125 \text { heads \& } 125 \text { tails } & n=250 & 0.0019 & \mathrm{H}_{0} \text { is rejected }\end{array}$$

One can understand from the example how there is an inverse relationship between the sample size and the p-value.

To disprove a null hypothesis $H_0,$ one needs a small enough p-value (maller than $\alpha$). The weight of a test increases with an increase in sample size, so that the null hypothesis can be rejected or retained on the basis of more qualitative evidence, although this is always accompanied by increased data collection efforts.

**Example:**

Given is $\left\{X_{1}, \ldots, X_{20}\right\}$ that can take values between 1 and 0, which correspond to the results of a coin toss. The coin is tossed a total of 20 times, with the following:

$$P\left(X_{i}=1\right)=\pi=1-P\left(X_{i}=0\right) \quad \text { for } \pi \in(0,1)$$

In doing so, we test the following null hypothesis: $\mathrm{H}_{0}: \pi=0.5 \quad \text { vs. } \quad \mathrm{H}_{1}: \pi \neq 0.5$

Suppose that we have obtained $17 \:X_is$ with the value of $1$. We will now check if we would discard $H_0$, at a given significance level of $1 \%$. 

Let $T=X_{1}+\cdots+X_{20}$, where $T \sim \operatorname{Bin}(20, \pi)$. $T$ corresponds to our test statistic, where we have a $t=17$ for our observations. Thus, we need to calculate the range that is even more extreme than $17$, for the null hypothesis to hold and the associated probability of $\mathrm{E}(T)=n \pi=20 \times 0.5=10$. Since the $3$, is just as extreme as the $17$, the even more extreme values correspond to the following:

$$\begin{array}{lllll}0, & 1, & 2, & 18, & 19 & \text { and } & 20\end{array}$$

Thus, the p-value can be calculated as follows:

$$\begin{aligned}\left(\sum_{i=0}^{3}+\sum_{i=17}^{20}\right) P_{\mathrm{H}_{0}}(T=i) &=\left(\sum_{i=0}^{3}+\sum_{i=17}^{20}\right) \frac{20 !}{(20-i) ! i !}(0.5)^{i}(1-0.5)^{20-i} \\&=2 \times(0.5)^{20} \sum_{i=0}^{3} \frac{20 !}{(20-i) ! i !} \\&=2 \times(0.5)^{20} \times\left(1+20+20 \times \frac{19}{2 !}+\frac{20 \times 19 \times 18}{3 !}\right) \\&=0.0026 .\end{aligned}$$

Since the p-value of $0.0026$ is less than the significance level of $0.01$, the null hypothesis is rejected in this example.

## Testing a population mean claim

We perform a hypothesis test on the population mean in the following. A water bottle manufacturer claims that water bottles are filled with 500 ml of water on average. We will model the quantity of water in a bottle with $X$ and an associated distribution of $X \sim N\left(\mu, \sigma^{2}\right)$. We will test the following hypothesis:

$$\mathbf{H}_{\mathbf{0}}: \boldsymbol{\mu}=\mathbf{5 0 0 \mathbf { m l }} \quad \text { vs. } \mathbf{H}_{\mathbf{1}}: \boldsymbol{\mu} \neq \mathbf{5 0 0 m l}$$

If we consider a random sample of $n=100$ and we assume that $\sigma$ corresponds to $10\text{ml}$, we can conclude the distribution as follows:

$$\bar{X} \sim N\left(\mu, \frac{\sigma^{2}}{n}\right)=N\left(\mu, \frac{(10)^{2}}{100}\right)=N(\mu, 1)$$

If within the observed sample the mean equals to $\bar{x}=503 \text{ml}$, we can understand that $\bar{x}=503 \neq 500=\mu$, where the value $500$, is the tested value in the null hypothesis. Accordingly, we will check whether the difference between $\bar{x}=503\text{ml}$ and $\mu=500\text{ml}$ is due to a sampling error or has a statistically significance and thus the null hypothesis must be rejected. The calculation of the p-value, will tell us about this, where we standardize $\bar{X}$ as a first step:

$$Z=\frac{\bar{X}-\mu}{\sigma / \sqrt{n}} \sim N(0,1)$$

$\bar{X}$ thus corresponds to our test statistic, taking into account both the effect size $\bar{X}-\mu$ and the sample size $n$. With our sample data, we get the corresponding statistical value:

$$\frac{503-500}{10 / \sqrt{100}}=3$$

The p-value corresponds to the probability of our test statistic value or even more extreme value relative to our null hypothesis $H_0$. Extreme in this context means a z-score $>$ 3 or $<$ -3. Given the symmetry of the distribution at zero, we can express it as follows:

$$p \text { -value }=P(Z \geq|3|)=0.0027$$

Since the p-value is smaller than our significance level of $5\%$ $(0.0027<0.05)$, we reject the null hypothesis. Thereby, the evidence is very strong that $\mu \neq 500$. 

Finally, we evaluate our decision options again:

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/decision_space.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/decision_space.png)

Fig. 34: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

Since we discarded $H_0$, this can be called one of the following two options:

- we have correctly rejected $H_0$
- we have committed a Type I error

Although the p-value was very small, a Type I error cannot be excluded, although it would be very unlikely. We cannot make any statements with full certainty due to the value of the p-value.

## The central limit theorem

We have already worked out that random samples result from a normal distribution, again in a sampling normal distribution of $\bar{X}$. Due to the mathematical theorem, the central limit theorem (CLT), this can be applied to random samples of almost all distributions, as long as the variance of the distribution is finite.

Given $\left\{X_{1}, X_{2}, \ldots, X_{n}\right\}$ as a random sample from the population distribution, which holds the mean of $\mathrm{E}\left(X_{i}\right)=\mu<\infty$ and the variance of $\operatorname{Var}\left(X_{i}\right)=\sigma^{2}<\infty$. If $\bar{X_n}$ is equal to the sample mean calculated by the sample size of $n$, then:

$$\lim _{n \rightarrow \infty} P\left(\frac{\overline{\boldsymbol{X}}_{n}-\mu}{\sigma / \sqrt{n}} \leq z\right)=\Phi(z)$$

This is true for any $z$, where $\Phi(z)=P(Z \leq z)$ corresponds to a cumulative probability of a standard normal distribution.

The sign $\lim _{n \rightarrow \infty}$ stands for an asymptotic result, whose evidence also increases with an increase of the sample size $n$, in the best case when the sample size is infinite. Simplified, the CLT states that for a random sample from almost any distribution with a mean $\mu$ and a variance $\sigma^2$, the following is true:

$$\overline{\boldsymbol{X}} \sim N\left(\mu, \frac{\sigma^{2}}{n}\right)$$

if $n$ is large enough. Therefore $\bar{X}$ can be said to be asymptotically normally distributed., with mean $\mu$ and variance $\frac{σ^2}{n}$.

### The wide reach of the CLT

CLT can also be applied beyond random sampling for the following two reasons:

- there are more general versions of CLT that do not require independent and identically distributed (IID) observations of $X_i$
- also the basic version can be used broadly, since $X$ can also be a function of the original variables of the data. As an example, if $X$ and $Y$ are a random variable of the sample, one can also apply the CLT there:

    $$\sum_{i=1}^{n} \frac{\log \left(X_{i}\right)}{n} \text { or } \sum_{i=1}^{n} \frac{X_{i} Y_{i}}{n}$$

Therefore, the CLT can also be used to infer sampling distributions for a lot of statistics that initially do not look at all like $\bar{X}$ for a single random variable in a sample.

### Definition of a 'large n'

Wie bereits erwähnt, wird die normal approximation durch CLT zuverlässiger mit steigender sample size $n$. The rule of thumb whether a sample size is large enough depends largely on the population distribution of $X_i$. For symmetric distributions a small $n$ is sufficient, whereas for skewed distributions the opposite is true. For many distributions already $n>50$ is sufficient for the approximation to be accurate.

**Example (skewed distribution):**

In the following example we simulate random sample of the different sample sizes:

$$n=1,5,10,30,100 \text { and } 1000$$

from the Exponential$(0.25)$ distribution, for which $\mu=4$ and $\sigma^2=16$ holds. In the experiment, 10,000 independent random samples were generated for each sample size, with the respective histograms and normal approximating distribution ($N(4,\frac{16}{n})$ shown below:

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2015.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2015.png)

Fig. 35: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2016.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2016.png)

Fig. 36: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

The plots show two key points, firstly that a skewed distribution, as can be seen at $n=1$, by increasing the sample size, a normal distribution-like distribution is obtained and secondly that a sample size of $n=30$ can already model the normal approximation quite well.

**Example (Bernoulli distribution):**

In the following experiment, we again take $10,000$ independent random samples of size $n=1,5,10,30,100 \text { and } 1000,$ sampling from the Bernoulli($0.2$) distribution, for $\mu=0.2$ and $\sigma^2=0.16$. Although the distribution of $X_i$ is not continuous and can take only two values, the sampling distribution $\bar{X}$ can be estimated from the normal distribution for a large enough $n$. 

$\bar{X}$  is equal to the sample proportion of the value $X=1$, where $m$ corresponds to the number of observations for $X_i=1$:

$$i, \bar{X}=\sum_{i=1}^{n} X_{i} / n=m / n$$

The following graphs show the observations and the normal approximation when the sample size is increased:

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2017.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2017.png)

Fig. 37: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2018.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2018.png)

Fig. 38: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

From the plots one can conclude that also non-continuous conviction of $X_i$ with a large $n$ can be well represented by the normal approximation. Moreover, the distribution converged towards $n\left(\mu, \sigma^{2} / n\right)$ and the variation (compare plot 5 and 6) decreases with an increasing $n$.

### Sampling distribution of the sample proportion

In the preceding example with Bernoulli sampling, the sample mean can be written as the sample proportion of successes $P$. Since we know from the CLT that the following holds approximately at large $n$:

$$\bar{X} \sim N\left(\mu, \frac{\sigma^{2}}{n}\right)$$

and we can model the Bernoulli distribution $X \sim \text{Bernoull}(\pi)$ as follows:

$$\mathbf{E}(X)=0 \times(1-\pi)+1 \times \pi=\pi=\mu$$

$$\operatorname{Var}(X)=\pi(1-\pi)=\sigma^{2}$$

we can state the following for n towards infinity $(n \rightarrow \infty)$:

$$\bar{X}=P \rightarrow N\left(\mu, \frac{\sigma^{2}}{n}\right)=N\left(\pi, \frac{\pi(1-\pi)}{n}\right)$$

Since the sample proportion is equal to the sample proportion on average, we can state that:

$$\mathbf{E}(\overline{\boldsymbol{X}})=\mathbf{E}(\boldsymbol{P})=\boldsymbol{\pi}$$

Finally, the sampling variance moves towards zero when the sample size moves towards infinity, as also illustrated by the graphs of the last experiment:

$$\operatorname{Var}(\boldsymbol{P}) \rightarrow \mathbf{0} \quad \text { as } \boldsymbol{n} \rightarrow \infty$$

## Proportions: confidence intervals and hypothesis testing

We will apply the approximate sampling distribution of sample proportion to statistical inference for proportions:

$$\bar{X}=P \rightarrow N\left(\mu, \frac{\sigma^{2}}{n}\right)=N\left(\pi, \frac{\pi(1-\pi)}{n}\right)$$

**Confidence intervals**

As we are already working we can define the confidence interval for a mean as follows:

$$\text { best guess } \pm \text { margin of error }$$

Since sample proportion is a special case of sample means, this is also applicable to proportion. Thereby applies: $\text { point estimate }=p$, where $p$ is the observed sample fraction and corresponds to the margin of error $\text { confidence coefficient } \times \text { standard error}$. The confidence coefficient is still a z-value, which we have already introduced via the corresponding table.

This gives the estimated standard error of:

$$\sqrt{\frac{p(1-p)}{n}}$$

and the confidence interval of a proportion is given as:

$$p \pm z \times \sqrt{\frac{p(1-p)}{n}}$$

**Example:**

In polls, a sample size of around $1000$ is usually chosen, since this leads to a margin of error of about three percentage points, which is an acceptable corridor for most people. If we assume that $630$ out of $1000$ within a random sample decide for 'yes' in a binary vote, we get the following sample proportion:

$$p=\frac{630}{1000}=0.63$$

Using a $95\%$ confidence interval for the true proportion $\pi$ who would vote 'yes', we get the following corridor:

$$0.63 \pm 1.96 \times \sqrt{\frac{0.63 \times 0.37}{1000}}=0.63 \pm 0.03 \quad \Rightarrow \quad(0.60,0.66) \quad \text { or } \quad(60 \%, 66 \%)$$

Thus, we can demonstrate the three percentage point margin of error.

**Example - Hypothesis testing:**

In the following, we will test the hypotheses:

$$\mathrm{H}_{0}: \pi=0.4 \text { vs. } \mathrm{H}_{1}: \pi \neq 0.4$$

with a random sample of $n=1000$ and the resulting sample proportion of $p=0.44$. For the hypothesis test, we standardize $P$:

$$Z=\frac{P-\pi}{\sqrt{\pi(1-\pi) / n}} \sim N(0,1)$$

Since the test statistic considers both the effect size $P-\pi$ and the sample size $n$, it is important to have a large enough $n$, which is the case with $n=1000$. If we use our sample data we get the following statistical value:

$$\frac{0.44-0.4}{\sqrt{0.4 \times(1-0.4) / 1000}}=2.58$$

The p-value corresponds to the probability of our test-statistic value or a more extreme value as a condition to $H_0$. Due to the symmetry of the normal distribution, it can be expressed as follows:

$$p \text { -value }=P(Z>2.58 \text{ and } Z < -2.58)=P(Z \geq|2.58|)=0.0099$$

According to our p-value decision rule and under the conclusion that our results are statistically relevant, we reject the null hypothesis $H_0$ at a significance level of $\alpha=0.5$ due to our p-value of $0.0099$ (since it is smaller than $0.5$). After rejecting a hypothesis, we again have the possible type 1 error, which is very unlikely due to the very small p-value.

## Exercise

You are to test the claim by a mineral water bottle manufacturer that its bottles contain an average of 1000 ml (1 liter).  A random sample of n = 12 bottles resulted in the measurements (in ml): 992, 1002, 1000, 1001, 998, 999, 1000, 995, 1003, 1001, 997 and 997.

It is assumed that the true variance of water in all bottles is $\sigma^2$ = 1.5, and that the amount of water in bottles is normally distributed.

Test the manufacturer's claim at the $1 \%$ significance level (you may use Excel to calculate the $p$ **value).  Also, briefly comment on what the hypothesis test result means about the manufacturer's claim, and if an error might have occurred which type of error it would be.

- PROMPT

    **PROMPT**

    You are to test the claim by a mineral water bottle manufacturer that its bottles contain an average of 1000 ml (1 litre).  A random sample of n = 12*n*=12 bottles resulted in the measurements (in ml): 992, 1002, 1000, 1001, 998, 999, 1000, 995, 1003, 1001, 997 and 997.

    It is assumed that the true variance of water in all bottles is \sigma^2 = 1.5*σ*2=1.5, and that the amount of water in bottles is normally distributed.

    Test the manufacturer's claim at the 1% significance level (you may use Excel to calculate the p*p*-value).  Also, briefly comment on what the hypothesis test result means about the manufacturer's claim, and if an error might have occurred which type of error it would be.

    In summary, the assignment requires:

    - the calculation of the sample mean from the raw observations
    - the formulation of the hypotheses,  and

        H0

        H1

    - calculation of the test statistic value
    - calculation of the $$p$-value$
    - a decision of whether or not to reject

        H0

    - an inferential conclusion about what the test result means
    - indication of which type of error might have occurred.

    mean from observation

    No uploaded file

    **PROMPT**

    The assignment requires:

    ![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2019.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2019.png)

    - the formulation of the hypotheses,  and

        H0

        H1

    The null hypothesis corresponds to H_0: mu=1000ml

    H_1:\mu \neq1000ml

    **PROMPT**

    The assignment requires:

    - calculation of the test statistic value

    (998,75-1000)/((1,5)^(1/2) / (12^(1/2))) = -3,54

    **PROMPT**

    The assignment requires:

    - calculation of the $$p$-value$

    p-value= P (Z > 3.540 and Z < 3.54) = 0,0004001

    **PROMPT**

    The assignment requires:

    - a decision of whether or not to reject

        H0

    We reject the null hypothesis H0 because at our significance level of 1% 0,0004001 < 0.0.

    **PROMPT**

    The assignment requires:

    - an inferential conclusion about what the test result means

    That means that the difference between hypothesis and results are statistically relevant and therefore the hypothesis has to be rejected.

    **PROMPT**

    The assignment requires :

    - indication of which type of error might have occurred.

    A type 1 error might have occurred although the chances are pretty low it is not possible to exclude this option.

# Applications

## Decision Tree Analysis

Decision Tree analysis is a modelling technique to evaluate decision under uncertainty whereby the future outcome is also uncertain. We are confronted with such situations every day, such as whether we should invest in a certain stock, meal etc. or not. In the following, we will look at a decision analysis of a single non-strategic decision maker. 

**Example:**

As an example, we use an ice cream manufacturer whose sales can be either high ($\$300,000$ - excluding incidentals) or low ($\$100,000$ - excluding incidentals). The sales are mutually exclusive and collectively exhaustive for simplicity. One must decide whether to take advantage of an advertising campaign for $\$100,000$. If one chooses to do so, the probability is $0.9$ instead of $0.6$ for high sales. Since an advertising campaign cannot guarantee success, it only increases the probabilities. We can now consider the possible conditional probabilities:

$$\begin{array}{l}P(\text { high sales } \mid \text { no advertising })=0.6 \\P(\text { low sales } \mid \text { no advertising })=0.4\\
P(\text { high sales } \mid \text { advertising }) =0.9 \\
P(\text { low sales } \mid \text { advertising })=0.1
\end{array}$$

A standard decision tree includes the following components:

- Decision node $\square$ → decision maker has to make a choice
- chances nodes $\bigcirc$ → resolution of uncertainty
- branches → available choices to the decision-maker or possible outcome if uncertainty is resolved
- probability → indicated at the branches leading from chance node
- payoffs → results at the end of the final branches

In addition, a decision still has the following properties:

- no loops
- one initial node
- at most one branch between any two nodes
- connected paths
- decision-maker has information on all preceding events at decision node, in particular on the resolution of uncertainty.

The decision tree for our example looks like:

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/decision_tree.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/decision_tree.png)

Fig. 39: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

The decision tree starts with a decision node, advertise or not advertise. This decision is followed by the chances node, which connects the decision to an outcome with the associated probabilities. To solve the decision tree, we calculate the expected monetary value (EMV) of each option and decide on the maximum expected profit. The EMV is the expected value and so we apply the probability-weighted average.

$$\begin{aligned}\mathrm{E}(\text {advertise}) &=0.9 \times £ 200,000+0.1 \times-£ 200,000 \\&=£ 160,000\\
\mathrm{E}(\text {not advertise}) &=0.6 \times £ 300,000+0.4 \times-£ 100,000 \\
&=£ 140,000 .
\end{aligned}$$

The strategy to be selected includes choosing the advertising campaign, as the expected payoff is higher. ($\$160.000>\$140.000$) However, it is also important to understand that the expected value is long-term and other short-term results can occur. In doing so, one tries to quantify the associated risk.

## Risk

The previous example was only based on choosing the option with the maximum expected profit without considering the risk. 

### Degrees of risk

**Risk averse** refers to the choice of a certain outcome $\$x$ over a risky outcome with a mean (EMV) of  $\$x$. 

In the following example, we see that although the EMV of the risky asset is greater than the outcome of the safe asset, due to risk aversion the decision maker chooses the safe asset.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Screen_Shot_2021-07-22_at_13.35.50.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Screen_Shot_2021-07-22_at_13.35.50.png)

Fig. 40: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

**Risk-loving** refers to the choice of a risky outcome $\$x$ with a mean (EMV) of  $\$x$ over a certain outcome of $\$x$ as the example shows.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Screen_Shot_2021-07-22_at_13.44.25.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Screen_Shot_2021-07-22_at_13.44.25.png)

Fig. 41: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

**Risk-neutral** refers to a choice for which it is indifferent between a sure payoff and an uncertain outcome with the same expected monetary value.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Screen_Shot_2021-07-22_at_13.46.47.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Screen_Shot_2021-07-22_at_13.46.47.png)

Fig. 42: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

The **certainty equivalent** is a guaranteed return that someone would accept now, rather than taking a chance on a higher, but uncertain, return in the future.

### Risk premium

The risk premium of a project is defined as: $\mathbf{E M V}-\mathbf{C E}$. The risk premium thus corresponds to the amount that would be paid to obtain the safe return instead of the expected payoff of the risky return. The profiles can be determined as: 

$$\begin{array}{l}\mathrm{CE}<\mathrm{EMV} \Rightarrow \text { risk-averse } \\\mathrm{CE}=\mathrm{EMV} \Rightarrow \text { risk-neutral } \\\mathrm{CE}>\mathrm{EMV} \Rightarrow \text { risk-loving. }\end{array}$$

## Linear Regression

Linear regression analyses are one of the most common statistical techniques to model the relationship between a dependent variable $y$ and one or more regressors (also covariates or independent variables) $x_1,\dots,x_p$. In doing so, one tries to obtain insights about the dependence of $y$ on $x_1,\dots,x_p$ and to predict the non-oberserved variable $y$ based on the observed $x_1,\dots x_p$. In the following examples, we will only consider a $p=1$.

**Example:**

In one example, sales of pizzas $y$ from 10 pizza restaurants are strongly correlated with the number of students $x$ in the associated neighborhood. The plot shows the sales in thousand of US-Dollar in a period of three months and the number of students in thousand in their neighbourhoods.

We plot $y$ against $x$ and draw a straight line through the middle of the data points.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Screen_Shot_2021-07-22_at_15.01.16.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Screen_Shot_2021-07-22_at_15.01.16.png)

Fig. 43: Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

This is to be calculated with the formula: $y=\alpha+\beta x+\varepsilon$, where $\epsilon$ corresponds to the random error term, $\alpha$ to the intersection with the $y$-axis and $\beta$ to the slope of the line. Knowing $x$, the number of student populations within a neighborhood, sales can be estimated as follows:

$$\widehat{\boldsymbol{y}}=\boldsymbol{\alpha}+\boldsymbol{\beta} \boldsymbol{x}$$

### The simple linear regression model

Now we illustrate the simple linear regression model. The paired observations $\left(x_{1}, y_{1}\right), \ldots,\left(x_{n}, y_{n}\right)$ are drawn from the model $y_{i}=\alpha+\beta x_{i}+\varepsilon_{i}$, where the following holds:

$${E}\left(\varepsilon_{i}\right)={0} \text { and } \operatorname{Var}\left(\varepsilon_{i}\right)=\sigma^{2}>0.$$

The presented model has three parameter: $\beta_0, \beta_1$ and  $\sigma^2$

**Example:**

We can apply the simple linear regression model to the study of the correlation of two financial returns. As example a regression on the stock returns $y$ and the returns of the underlying market index $x$. This is also called the capital asset pricing model (CAPM).

When the difference between the stock prices is small, the difference is defined as:

$$\text { return }=\frac{\text { current price - previous price }}{\text { previous price }} \approx \log \left(\frac{\text { current price }}{\text { previous price }}\right)$$

Even though the daily prices are not independent of each other, the daily return can be seen as a sequence of uncorrelated random variables.

The CAPM is the simple pricing model in finance which equals to the following, where $y_i$ is the stock return and $x_i$ is a market return at time $i$.

$$y_{i}=\alpha+\beta x_{i}+\varepsilon_{i}$$

**total risk of the stock:**

$\frac{1}{n} \sum_{i=1}^{n}\left(y_{i}-\bar{y}\right)^{2}\\=\frac{1}{n} \sum_{i=1}^{n}\left(\widehat{y}_{i}-\bar{y}\right)^{2}+\frac{1}{n} \sum_{i=1}^{n}\left(y_{i}-\widehat{y}_{i}\right)^{2}$

**firm specific risk:**

$$\frac{1}{n} \sum_{i=1}^{n}\left(y_{i}-\widehat{y}_{i}\right)^{2}$$

**market-related (or systematic) risk:**

$$\frac{1}{n} \sum_{i=1}^{n}\left(\widehat{y}_{i}-\bar{y}\right)^{2}=\\\frac{1}{n} \widehat{\beta}^{2} \sum_{i=1}^{n}\left(x_{i}-\bar{x}\right)^{2}$$

Now follow some supplementary notes:

$\beta$ measures the market-related risk of the stock, which is unavoidable as it can't be diversified away with hedging as it would be possible with a firm specific risk. Variance is a simple measure of risk in finance. 

Beta equals a simple measure of the risk of that stock with respect to the market index. By definition the market index has $\beta=1$. If we now compare the development of $\beta$ and its correlation with stock performance, we obtain the following correlations:

For $\beta=1$:

$$\text { if the market index } \uparrow \text { by } 1 \% \text { , then the stock } \uparrow \text { by } 1 \% \\
\text { if the market index } \downarrow \text { by } 1 \% \text { , then the stock } \downarrow \text { by } 1 \%$$

For $\beta=2$:

$$\text { if the market index } \uparrow \text { by } 1 \% \text { , then the stock } \uparrow \text { by } 2 \% \\
\text { if the market index } \downarrow \text { by } 1 \% \text { , then the stock } \downarrow \text { by } 2 \%$$

For $\beta=0.5$:

$$\text { if the market index } \uparrow \text { by } 1 \% \text { , then the stock } \uparrow \text { by } 0.5 \% \\
\text { if the market index } \downarrow \text { by } 1 \% \text { , then the stock } \downarrow \text { by } 0.5 \%$$

In summary, $\beta>1$ implies an increased risk for this specific stock as market movements are amplified in the stock's returns and vice versa.

## Linear programming

Linear programming represents one of the most widespread quantitative business model methods, which can be applied as soon as limited resources can be allocated differently and one tries to identify their optimal distribution.

### Optimization methods

The optimization models have a wide range of common features:

**decision variables** → the values that have to be known and chosen upfront

**objective function** → ****find their optimum (maximize or minimize)

**constraints** → constraints and restrictions which must be satisfied

### Solving optimization problems

The first step is to define the decision variables, the objective, and the constraints and how they are related to each other so that a suitable formula can be established.

This is followed by optimization resulting in the feasible solution, which includes a solution that satisfies all constraints, and a feasible region, which is the set of all feasible solutions.

Third, sensitivity analysis is performed to determine the degree to which the final solution is sensitive to each parameter.

**Example**

A manufacturer of chocolate bars has two different bars, for each of which resources are to be determined to maximize profits. Here, chocolate bar A takes 10 grams of cocoa and one minute of production time, where product B takes 5 grams of cocoa and 4 minutes of production time. Combined, both have 2,000 grams of cocoa and 480 production time per day. If we assume that all the chocolate bars are sold, the manufacturer makes a profit of 10 cents on product A and 20 cents on product B.

The decision variables for the optimization are the following:

$$\text{x= quantity of type A bars}\\
\text{y= quantity of type B bars}$$

The objective functions $10 x+20 y$ has to be maximized regarding the constraints, where $y$ and $x$ are non-negative:

$$\begin{aligned}10 x+5 y &=2000 \quad(\operatorname{cocoa}) \\x+4 y &=480 \quad \text { (machine time). }\end{aligned}$$

The two lines intersect when both constraint equations are true:

$${1 0 x}+{5 y}={2 0 0 0} \text { and } {x}+{4 y}={4 8}$$

We put each possible solution from the previous condition into the objective function resulting in the following:

$$\begin{array}{l}(0,0) \text { , with profit } 10 x+20 y=0 \\(0,120), \text { with profit } 10 x+20 y=2400 \\(200,0) \text { , with profit } 10 x+20 y=2000 \\(160,80) \text { , with profit } 10 x+20 y=3200\end{array}$$

The optimal distribution of resources is to produce 160 units of product A and 80 units of product B, so that we can expect a profit of 3200 cents.

## Monte Carlo Simulation

The uncertainty about possible paths of realization is omnipresent and unavoidable. The question of whether or not to do a master's, invest in these stocks or not, these will always be accompanied by uncertainty. Trying out different options is often costly and usually cannot be accomplished with available resources.

The Monte Carlo simulation simulates different hypothetical realization paths where the result variables that are examined correspond to a random variable with a probability distribution. Using the mean and variance, we can quantify the expected outcome and risk and present different perspectives and its probability so that one can make more risk-conscious decisions based on it.

To perform a Monte Carlo simulation we proceed as follows:

1. Associate a (pseudo-)random number generator for each input variable.
2. Assign a range of random numbers for each input variable (according to some assumed probability distribution).
3. For each input variable:
    1. generate a random number
    2. from the random number, select the respective variable value.
4. Calculate the outcome, $x$, and record it.
5. Repeat $3$ and $4$, until the desired number of iterations, $N$, is reached.
6. Draw a histogram of the outcomes and determine the mean and variance of the simulated
outputs:

    $$\bar{x}=\frac{1}{N} \sum_{i=1}^{N} x_{i}$$

    and

    $$s^{2}=\frac{1}{N-1} \sum_{i=1}^{N}\left(x_{i}-\bar{x}\right)^{2}$$

    The mean equals to the estimate of the expected outcome, while the variance is the measure of the associated risk.

**Example**

In the following link you can find a Monte Carlo simulation written in python and different realization paths considering the possible evolution of the price of the SPDR S&P 500 Trust ETF.

[GitHub - ak4win/monte-carlo-simulation: A monte carlo simulation for the spy ETF](https://github.com/ak4win/monte-carlo-simulation.git)

## Hyper-parameter Optimization and in particular bayesian optimization for deep learning model

Since bayesian optimization models constrain the hyper-parameter values based on previous results, an optimal configuration is found within a smaller number (compared to GS & RS) of iterations. Within bayesian optimization, there are a number of different methods to model the distribution of the objective function using different models as surrogate functions, such as Gaussian process (GP), random forest (RF), or tree-structured parzen (TPE) estimators models. The last two methods (RF & TPE) can also optimize conditional hyper-parameters such as the cost function and the associated learning rate. 

- conditional hyper-parameter

    A hyper- parameter may need to be used or tuned depending on the value of another hyper-parameter

However, since each future optimization step at the bayesian optimization relies on the previous results, parallelization is hardly feasible.

- objective function

    the function we are trying to maximize or minimize

- surrogate function

    a probabilistic model of the objective function, that is then searched efficiently with an acquisition function before candidate samples are chosen for evaluation on the real objective function

- acquisition function

    Technique by which the posterior is used to select the next sample from the search space

### Optimization problems

Most real-world optimization problems fall into the constrained optimization problems. That means that we optimize our objective function with respect to certain constraints which normally are denoted by a constrain function. 

As example we try to minimize the objective function $\min _{x} f(x)$
  with respect to the inequality constraint function $\:g_{i}(x) \leqslant 0, \quad i=1,2, \ldots, m$  and the equality constraint function $h_{j}(x), j=1,2, \ldots, p$ where $X$ is the domain of $x$. ($x \in X$).

The constraints limit the search space that is investigated. The resulting space is called feasible region. In our example the feasible region $D$ of $x$ can be represented by: $D=\left\{x \in X \mid g_{i}(x) \leqslant 0, h_{j}(x)=0\right\}$. 

- unconstrained optimization problems

    In the unconstrained optimization problems, the variable $x$ can take any value within the real numbers, consequently there are no restrictions to the acceptable values. We can understand an example of such optimization by the example of minimization: $\min _{x \in \mathbb{R}} f(x)$.

Summarized one can consider the following:

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Uberschrift_hinzufugen.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Uberschrift_hinzufugen.png)

Fig. 44: constrained optimization problem

The goal of an optimization procedure is therefore to find the optimal set of decision variables $x$ to minimize or maximize an objective function with respect to the constraints.

### Finding the global optimum

One of the biggest challenges in optimizing for a global optimum is getting stuck in a local optimum and accepting that as the optimization result. In a simplified example, it would look like this:

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/thumb-surrogate-optimization.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/thumb-surrogate-optimization.png)

Fig. 45: Surrogate Opimization. (n.d.). [Graph]. [https://it.mathworks.com/videos/surrogate-optimization-1535996187824.html](https://it.mathworks.com/videos/surrogate-optimization-1535996187824.html)

Für eine decision Variable $x$ mit der zugehörigen feasible region $D$ ist ein Punkt das globale Minimum, wenn der Punkt $x^{*} \in D$ folgendes erfüllt: $f\left(x^{*}\right) \leqslant f(x) \forall x \in D$. Für ein lokales Minimum hingegen trifft für ein Punkt $x^*$ in einer neighborhood $N$ folgendes zu: $f\left(x^{*}\right) \leqslant f(x) \forall x \in N \cap D$. 

For a decision variable $x$ with associated feasible region $D$, a point is the global minimum if the point $x^{*} \in D$ *satisfies the following:*  $f\left(x^{*}\right) \leqslant f(x) \forall x \in D$. For a local minimum, on the other hand, the following is true for a point $x^*$ in a neighborhood $N$: $f\left(x^{*}\right) \leqslant f(x) \forall x \in N \cap D$  $$.

For convex functions there is only one optimum, therefore one can always go along the direction of minimization of the objective function to find this optimum.

- Proof whether a function is a convex function

    A function $f(x)$ is convex if for $\forall x_{1}, x_{2} \in X, \forall t \in[0,1]$ the following is true:

    $$f\left(t x_{1}+(1-t) x_{2}\right) \leqslant t f\left(x_{1}\right)+(1-t) f\left(x_{2}\right)$$

    where $X$ is the domain of decision variables and $t$ is a coefficient in the range of $[0,1]$.

An optimization problem is only a convex optimization problem when the objective function $f(x)$ is a convex function and the feasible region equals to a convex set.

- convex set

    an affine space over the reals, is convex if, given any two points, it contains the whole line segment that joins them

    ![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Convex_polygon_illustration1.svg.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Convex_polygon_illustration1.svg.png)

However, most machine learning models are non-convex optimization problems and thus inappropriate optimization methods might get stuck in a local minimum. Some traditional optimization methods are not applicable to the complex problems, because they persist exactly in these local minima. As an example, there is gradient descent, which always moves in the negative direction of the gradient function to reach the minimum, without being able to guarantee that this also corresponds to the global minimum.

### Hyper-parameter optimization problem statement

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Uberschrift_hinzufugen_(1).png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Uberschrift_hinzufugen_(1).png)

Fig. 46: Optimization process

The hyper-parameter can obtain continuous (e.g., learning rate), discrete (e.g., number of layers), binary (e.g., whether to use dropout) or categorical (e.g., loss function) values. As a complement, there are also conditional hyper-parameters that are optimized only when a condition is met, such as the degree of a dropout, you must optimize only when dropout is enabled.

In general, in a hyper-parameter optimization problem, one would like to obtain: $x^{*}=\arg \min _{x \in X} f(x)$. Where $f(x)$ is the objective function to be minimized; $x$ corresponds to the hyper-parameter configuration resulting in the optimum of $f(x)$ and a hyper-parameter can take any value within the search space $X$. The HPO tunes the hyper-parameter to achieve a iotimal configuration within the given budget. The mathematical expression of the function varies based on the objective function of the selected ML algorithm and the performance metric function. 

When optimizing a model configuration, however, the available time is often the limiting characteristic. Since the ML model must be trained again for each configuration and then checked for performance via the validation set, it can be quite a long process depending on the duration of the training.

The basic building blocks of the HPO process are as follows:

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Uberschrift_hinzufugen_(2).png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Uberschrift_hinzufugen_(2).png)

Fig. 47: Process of the hyper-parameter optimization

### The application of BO

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/1_BDhUV6VLxZRZ7ue-wPPOlw.gif](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/1_BDhUV6VLxZRZ7ue-wPPOlw.gif)

Fig. 48: Bayesian Optimization. (n.d.). [Animation]. [https://miro.medium.com/max/1838/1*BDhUV6VLxZRZ7ue-wPPOlw.gif](https://miro.medium.com/max/1838/1*BDhUV6VLxZRZ7ue-wPPOlw.gif)

Unlike grid and random search, bayesian optimization incorporates the previous result of the hyper-parameter configuration into the evaluation of the exploration of the next configurations. This method consists of two basic components. One is the surrogate model, which tries to model the objective function using the results already obtained, which also includes a predictive distribution.

On the other hand, there is the acquisition function, which decides where to sample the next value based on the trade-off, exploration of areas where no values have been sampled yet and exploration of areas where it looks promising due to already sampled values and its posterior distribution.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Uberschrift_hinzufugen_(3).png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Uberschrift_hinzufugen_(3).png)

Fig. 49: Process of Bayesian Optimization

For our implementation the Gaussian process (GP) is used as surrogate model for the objective function modeling. If we assume a realization of GP by the function $f$ with mean $\mu$ and covariance $\sigma^2$, we can assume that the predictions correspond to the normal distribution:

$$p(y \mid x, D)=N\left(y \mid \hat{\mu}, \hat{\sigma}^{2}\right).$$

$D$ corresponds to the configuration space of the different hyper-parameters, such as the depth of a neural network or their number of nodes, and $y=f(x)$ corresponds to the evaluation result of each hyper-parameter value $x$. After the predictions of a run, the confidence intervals generated by GP are used to select new points to be examined.  The acquisition function used is upper confidence bounds (USB).

The objective of the Bayesian optimization is minimizing the loss applying the model to the validation dataset while the maximum number of epochs to train one model equals to 25. The maximum amount of testing different configurations equals to 10, as the bayesian method converges faster than other state-of-the Art methods. The number of randomly initial points to evaluate a good starting point equals to three. The Trade-off factor of balancing exploration and exploitation equals to 2.6. Every trials is executed two times to reduce variance among the the trials. The implementation for a Stacked Auto-Encoder with Convolutional-Restricted Boltzmann Machine Layers and a Stacked-RNN Auto-Encoder is in the following repository.

[hyperparameter-optimization/optimization.py at 7cf06a3b437fc0fc04a0887d623aac93e7950bf6 · ak4win/hyperparameter-optimization](https://github.com/ak4win/hyperparameter-optimization/blob/7cf06a3b437fc0fc04a0887d623aac93e7950bf6/optimization.py#L78)

[GitHub - ak4win/hyperparameter-optimization](https://github.com/ak4win/hyperparameter-optimization)

## Variational Auto-Encoder

I am working with a research team to compress time-series data while maintaining a good reconstruction rate. For this we use the concept of the auto-encoder, specifically a further development of the variational auto-encoder (VAE). In the following the concept of the VAE and the implementation is illustrated.

### 'Intractable' distribution

In computer science *any* problem is intractable when finding any solution to it will cost more than polynomial time, that is its lower time complexity bound is exponential. 

Further reading [this article](https://stackoverflow.com/questions/43820240/what-does-a-tractable-distribution-mean#:~:text=Intractable%20distributions%20take%20equal%20to,is%20long...).).

Thus a distribution might be called intractable if it takes at least exponential time to calculate any of its probabilities. It might possibly also be referring to the intractability of integrating over the distribution.

### Multivariate distribution

A multivariate distribution is the accumulation of multiple random variables. For a bivariate distribution that contains the normally distributed random variables $X$ and $Y$ one can put the possible values onto a plain and show their probabilities in a third dimension.

Further reading → [this paper](https://www.stat.uchicago.edu/~stigler/Stat244/ch3withfigs.pdf).

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Lgucc.gif](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Lgucc.gif)

Fig. 50: marginal distribution animation. (n.d.). [Animation]. [https://mathematica.stackexchange.com/questions/27083/visualization-of-bivariate-distributions](https://mathematica.stackexchange.com/questions/27083/visualization-of-bivariate-distributions)

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2020.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2020.png)

Fig. 51: Multivariate Normal Distribution. (2013). [Graph]. [https://commons.wikimedia.org/wiki/File:MultivariateNormal.png](https://commons.wikimedia.org/wiki/File:MultivariateNormal.png)

When trying to calculate a probability of this multivariate distribution, it is necessary to integrate over each dimension if the distribution is continuous.

$$P(a<X<b \quad \text { and } \quad c<Y<d)=\int_{c}^{d} \int_{a}^{b} f(x, y) d x d y$$

It will necessarily be true of any bivariate density that:

$$f(x, y) \geq 0 \quad \text { for all } \quad x, y$$

and

$$\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} f(x, y) d x d y=1.$$

For discrete distributions:

$$p(x, y)=P(X=x \quad \text { and } \quad Y=y)$$

$$\sum_{\text {all } x} \sum_{x \text { all } y} p(x, y)=1$$

## Marginal distribution

If one has two random variables $X$ and $Y$ (e.g the probability for rolling a dice each) the marginal probability is the likelihood of $X=A$ regardless of $Y$. That means one is only interested in the behavior of $X$ without any dependance to $Y$. This is called *marginal* probability because in a probability table one could find it in the margins.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2021.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Untitled%2021.png)

Fig. 52: marginal distribution matrix. (n.d.). [Matrix]. [https://www.statisticshowto.com/probability-and-statistics/statistics-definitions/marginal-distribution/](https://www.statisticshowto.com/probability-and-statistics/statistics-definitions/marginal-distribution/)

The marginal probability $P(X=A)$ can be calculated 

$$P(X=A) = \sum_{y \epsilon Y}P(X=A|Y=y)$$

Therefore the marginal distribution can be derived by the same process for each possible value of $X$ instead of only for the single event $A$. ([Further reading](https://machinelearningmastery.com/joint-marginal-and-conditional-probability-for-machine-learning/))

### Information and Entropy

**Information** tries to quantify the amount of (surprising/new) information in a statement. In terms of probability the information of a distribution at a given point $x$ can be calculated by

$$I(x) = log_2 P(x)$$

the logarithm of basis two is chosen because it allows for a representation of bits as a quantity (remember that bits are nothing more than counting something in a binary way). It can be observed that when a probability is very high, the information in it is very low - it doesn't contain any surprising new knowledge.

**Entropy** is the expected Information of a distribution. It is

For discrete distributions one can sum over all of the values of the random variable $X$

$$H = \sum_{x\epsilon X}{P(x)\ log_2 P(x) } = \sum_{x\epsilon X}P(x) \ I(x)$$

For continuous distributions one has to integrate, given the infinite possible values of $X$.

$$H = \int_{-\infty}^{\infty}{P(x)\ log_2 P(x) } = \int_{-\infty}^{\infty} P(x) \ I(x)$$

### Kulbeck-Leibler Divergence

Kulbeck-Leibler Divergence (KL-Divergence) is a measure of similarity between two distributions of a random variable. It is important to mention that $D_{KL}$ is always with respect to one of the two distributions. Therefore it is - unlike distance - asymmetric: the distance between $P$ to $Q$ is not the same as between $Q$ to $P$.

$$D_{KL}(q||p) = \sum_{x \epsilon X} q(x) \ log_2\frac{q(x)}{p(x)} = \sum_{x \epsilon X} q(x) \ log_2(q(x)-p(x))$$

For continuous distributions one has to integrate instead of sum over the values.

The second equation intuitively shows that the $log$ part of the product is concerned with the absolute distance between distribution $q$ and distribution $p$. Multiplying with $q(x)$ on the left side is what makes this operation asymmetric. It assigns greater importance only to those values that are likely to happen in distribution $q$ even though they might be quite likely in distribution $p$. 

When trying to assimilate $p$ to $q$ KL Divergence can be interpreted as the expected information loss when using $p$ instead of $q$.

We have implemented the KL Divergence for loss calculation of our reconstruction.

The KL-divergence is applied for learning the distribution of the train data which prevents the model from over-fitting. For the standard deviation vector log $\sigma^2$ and the mean vector of $\mu^2$ the KL-divergence looks like the following:

$$K L=-0.5 \times\left(1+\log \sigma^{2}-\mu^{2}-\exp \left(\log \sigma^{2}\right)\right)$$

MSE is also known as the reconstruction term, and it represents the accuracy of the reconstruction and penalizes outliers more than small deviations as the formula indicates:

$$m s e=\frac{\sum_{i=1}^{n}\left(x_{i}-x_{i}^{\prime}\right)^{2}}{n}$$

The two components are offset against each other, and their ratio to each other is regulated with the help of an equilibirium factor $\lambda$, the so-called loss weighting. The factor can take a value between zero and one and the final loss function looks as follows:

$$loss =m s e+\lambda * K L$$

```python
def add_loss(self, model, inputs, outputs, z_mean=None, z_log_var=None):
        assert (self.use_sampling is True and z_mean is not None) or (
            self.use_sampling is False and z_mean is None
        )
        assert (self.use_sampling is True and z_log_var is not None) or (
            self.use_sampling is False and z_log_var is None
        )

        reconstruction_loss = self.loss_function(K.flatten(inputs), K.flatten(outputs))
        reconstruction_loss *= self.sequence_length

        if self.use_sampling is True:
            kl_loss = 1 + z_log_var - K.square(z_mean) - K.exp(z_log_var)
            kl_loss = K.sum(kl_loss, axis=-1)
            kl_loss *= -0.5
        else:
            kl_loss = 0

        vae_loss = K.mean(reconstruction_loss * self.loss_weighting + kl_loss)
        model.add_loss(vae_loss)
```

- Deriving D_KL

    Take as given that the KL-divergence between two univariate gaussians can be expressed as (taken from [here](https://stats.stackexchange.com/questions/7440/kl-divergence-between-two-univariate-gaussians)):

    $$D_{KL} = \frac{1}{2} \ log(2\pi \Sigma_2) \ \ \ \ + \ \ \ \ \frac{\Sigma_1 \ + (\mu_1 - \mu_2)^2}{2\Sigma_2} \ \ \ \ \ \ - \frac{1}{2} log(1 + log(2\pi \Sigma_1) $$

    $$= -\frac{1}{2}\left[-log(2\pi \Sigma_2) \ \ + \ \ 1  \ \ + \ \ \log(2\pi \Sigma_1) \right] \ \ \  + \ \ \ \frac{\Sigma_1 \ + (\mu_1 - \mu_2)^2}{2\Sigma_2}$$

    $$-\frac{1}{2}\left[1 +log\left(\frac{2\pi \Sigma_1}{2\pi \Sigma_2}\right) \right] \ \ \  +  \ \ \ \frac{\Sigma_1 \ + (\mu_1 - \mu_2)^2}{2\Sigma_2}$$

    If one of the distributions is the standard gaussian, $\Sigma_2=1$ and $\mu_2=0$. Keep in mind that $log(1) = 0$

    $$= -\frac{1}{2}\left[1 + \log \left(\frac{\Sigma_1}{1} \right) \right] \ \ \  + \ \ \ \frac{\Sigma_1 \ + (\mu_1 - 0)^2}{2*1}$$

    $$= -\frac{1}{2} + -\frac{1}{2}\log (\Sigma_1 ) \ \  + \ \ \frac{1}{2}( \Sigma_1 \ + \mu_1^2)$$

    $$-\frac{1}{2} (1 + log(\Sigma_1) -\Sigma_1 - \mu_1^2)$$

### Variational Inference

When dealing with probability distributions and encountering an intractable distribution $P$ one can try to assimilate a tractable distribution $q$ such as Gaussian or Bernoulli that is close enough to $P$ but easier/possible to deal with.

There are two common methods to assimilate such a distribution to $P$:

- Markov Chain Monte-Carlo methods such as Gibbs sampling or Metropolis-Hastings
- Variational inference

Variational inference will almost never find the optimal solution, however it is far more suitable for multidimensional distributions and can therefore be applied in real life more often.

VI treats the assimilation process as an optimization problem as it tries to discover the global minimum of $D_{KL}(P||q)$ by finding a $q$ in the family of $Q$. This is done by setting *variational parameters,* hence the name of the process. These parameters might be different depending on which distribution one deals, they might be mean and variance.

A variational Auto-encoder (VAE) provides a probabilistic manner for describing an observation in the latent space. The encoder is outputting a probability distribution for each latent attribute.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Screen-Shot-2018-06-20-at-2.46.16-PM_(1).png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Screen-Shot-2018-06-20-at-2.46.16-PM_(1).png)

Fig. 53: Jordan, J. (n.d.). Variational Auto-Encoder [Illustration]. [https://www.jeremyjordan.me/content/images/2018/06/Screen-Shot-2018-06-20-at-2.46.16-PM.png](https://www.jeremyjordan.me/content/images/2018/06/Screen-Shot-2018-06-20-at-2.46.16-PM.png)

If we assume that there is a hidden variable $z$ that generates observation $x$, and we would like to know $z$ characteristics, but we only know $x$ we could calculate this as follows:

$$p(z \mid x)=\frac{p(x \mid z) p(z)}{p(x)}$$

However, since the calculation of $p(x)$:

$$p(x)=\int p(x \mid z) p(z) d z$$

is very difficult as it usually turns out to be an intractable distribution. To estimate this distribution, we apply variational inference.

Here we approximate the non-computable distribution by another distribution that is tractable. We choose the parameters so that they are as similar as possible to $p(z|x)$. Through KL-divergence, we try to move this self-generated distribution as close as possible to the intractable distribution. 

This is implemented in the following repository. We have two fully connected layers, which compute the mean and variance of the latent attributes, which are then sampled using the reparameterization trick. For the sampling we use five latent attributes for each of which a normal distribution is created.

```python
### Sampling using reparameterization trick
def sample_from_latent_space(self, args):
        z_mean, z_log_var = args
        batch = K.shape(z_mean)[0]
        dim = K.int_shape(z_mean)[1]
        # by default, random_normal has mean=0 and std=1.0
        epsilon = K.random_normal(shape=(batch, dim))
        return z_mean + K.exp(0.5 * z_log_var) * epsilon
```

```python
### Sampling in the Auto-Encoder Latent-Space
z_mean = Dense(5, activation=self.encoder_activation, name="z_mean")(out_dense1)
z_log_var = Dense(5, activation=self.encoder_activation, name="z_log_var")(
                    out_dense1
                )
z = Lambda(self.sample_from_latent_space, output_shape=(5,), name="z")(
                    [z_mean, z_log_var]
                )
```

[](https://github.com/Ahmed-Eldably/Hyperparameters-Optimization-Methods/blob/401ab74006ea21fdf932b5cdafde7d5741695188/models/CBN_VAE.py#L87)

### Graphical models

Probabilistic Graphical Models present a way to model relationships between random variables. They are statistical models that encode complex joint multivariate probability distributions using graphs. By knowing the graph structure of a PGM, one can solve tasks such as inference (computing the marginal distribution of one or more random variables) or learning (estimating the parameters of probability functions). One can even try to learn the structure of the graph itself, given some data.

There are two bigger areas of different graphical models, one the one side the undirected graphs and on the other side the directed graphs.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Graphical_Models_David_Barber.gif](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Graphical_Models_David_Barber.gif)

Fig. 54: Barber, D. (2012). Bayesian Reasoning and Machine Learning (1st ed.). Cambridge University Press. [http://www.cs.ucl.ac.uk/staff/d.barber/brml/](http://www.cs.ucl.ac.uk/staff/d.barber/brml/)

Graphical models can be used for tractable estimation of multivariate probability distributions and are an important ingredient for causal statistical inference. They can also be used to build predictive models (e.g. Conditional Random Fields in natural language processing, Max-Margin Markov Networks). Since graphical models particularly make complex probability distributions computationally tractable to infer they are often employed to model complex hierarchical models. They can be combined with models in deep learning (e.g. Deep Boltzmann machines) as Yann Lecun points out below. 

In our project, we implemented a type of RBMs called Downsampling Convolutional Restricted Boltzmann Machines.

![SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Convolutional-RBM-with-max-pooling.png](SE_30%20Probability%20and%20Statistics%20Workbook%20bceb83068ca14aeeb19b6ec49d5579b0/Convolutional-RBM-with-max-pooling.png)

Fig. 55: Mixed handwritten and printed digit recognition in Sudoku with Convolutional Deep Belief Network - Scientific Figure on ResearchGate. Available from: [https://www.researchgate.net/figure/Convolutional-RBM-with-max-pooling_fig2_307545305](https://www.researchgate.net/figure/Convolutional-RBM-with-max-pooling_fig2_307545305) 

[](https://github.com/Ahmed-Eldably/Hyperparameters-Optimization-Methods/blob/401ab74006ea21fdf932b5cdafde7d5741695188/models/CBN_VAE.py#L101)

## List of references

American roulette wheel vector image. (n.d.). [Illustration]. [https://www.vectorstock.com/royalty-free-vector/american-roulette-wheel-vector-13367259](https://www.vectorstock.com/royalty-free-vector/american-roulette-wheel-vector-13367259)

Barber, D. (2012). Bayesian Reasoning and Machine Learning (1st ed.). Cambridge University Press. [http://www.cs.ucl.ac.uk/staff/d.barber/brml/](http://www.cs.ucl.ac.uk/staff/d.barber/brml/)

Bayesian Optimization. (n.d.). [Animation]. [https://miro.medium.com/max/1838/1*BDhUV6VLxZRZ7ue-wPPOlw.gif](https://miro.medium.com/max/1838/1*BDhUV6VLxZRZ7ue-wPPOlw.gif)

Contingency Table Joint Distribution. (n.d.). [Graph]. [https://i2.wp.com/statisticsbyjim.com/wp-content/uploads/2021/02/contingency_table_joint_probabilities.png?resize=447%2C137&ssl=1](https://i2.wp.com/statisticsbyjim.com/wp-content/uploads/2021/02/contingency_table_joint_probabilities.png?resize=447%2C137&ssl=1)

cumulative probabilities. (n.d.). [Graph]. [https://i.stack.imgur.com/wWTai.png](https://i.stack.imgur.com/wWTai.png)

Dr. James Abdey, University of London (n.d.). Probability and Statistics: To p or not to p? [MOOC]. Coursera. [https://www.coursera.org/learn/probability-statistics](https://www.coursera.org/learn/probability-statistics)

Falkner, S., Klein, A. & Hutter, F.. (2018). *BOHB: Robust and Efficient Hyperparameter Optimization at Scale*. Proceedings of the 35th International Conference on Machine Learning, in Proceedings of Machine Learning Research. 80:1437-1446 Available from [http://proceedings.mlr.press/v80/falkner18a.html](http://proceedings.mlr.press/v80/falkner18a.html).

Fischer, A., & Igel, C. (2012). An Introduction to Restricted Boltzmann Machines. Progress in

Pattern Recognition, Image Analysis, Computer Vision, and Applications, 14–36. [https://doi.org/10.1007/978-3-642-33275-3_2](https://doi.org/10.1007/978-3-642-33275-3_2)

Gangeh, M. (2013). Two Gaussian distributions with the same mean and different variances [Graph]. [https://i2.wp.com/statisticsbyjim.com/wp-content/uploads/2021/02/contingency_table_joint_probabilities.png?resize=447%2C137&ssl=1](https://i2.wp.com/statisticsbyjim.com/wp-content/uploads/2021/02/contingency_table_joint_probabilities.png?resize=447%2C137&ssl=1)

Hermans, R. (2008). Diagrams illustrating negative and positive skew [Graph]. [https://commons.wikimedia.org/wiki/File:Negative_and_positive_skew_diagrams_(English).svg](https://commons.wikimedia.org/wiki/File:Negative_and_positive_skew_diagrams_(English).svg)

horizontal Boxplot. (n.d.). [Graph]. [https://lsc.studysixsigma.com/wp-content/uploads/sites/6/2015/12/1435.png](https://lsc.studysixsigma.com/wp-content/uploads/sites/6/2015/12/1435.png)

Jordan, J. (n.d.). Variational Auto-Encoder [Illustration]. [https://www.jeremyjordan.me/content/images/2018/06/Screen-Shot-2018-06-20-at-2.46.16-PM.png](https://www.jeremyjordan.me/content/images/2018/06/Screen-Shot-2018-06-20-at-2.46.16-PM.png)

Kingma, D.P., & Welling, M. (2014). *Auto-Encoding Variational Bayes.* CoRR, abs/1312.6114.

Liu, J., Chen, F., Yan, J., & Wang, D. (2019). CBN-VAE: A Data Compression Model with Efficient Convolutional Structure for Wireless Sensor Networks. Sensors, 19(16), 3445. [https://doi.org/10.3390/s19163445](https://doi.org/10.3390/s19163445)

marginal distribution animation. (n.d.). [Animation]. [https://mathematica.stackexchange.com/questions/27083/visualization-of-bivariate-distributions](https://mathematica.stackexchange.com/questions/27083/visualization-of-bivariate-distributions)

marginal distribution matrix. (n.d.). [Matrix]. [https://www.statisticshowto.com/probability-and-statistics/statistics-definitions/marginal-distribution/](https://www.statisticshowto.com/probability-and-statistics/statistics-definitions/marginal-distribution/)

Monty open door. (2006). [Illustration]. [https://commons.wikimedia.org/wiki/File:Monty_open_door.svg](https://commons.wikimedia.org/wiki/File:Monty_open_door.svg)

Monty hall problem - Encyclopedia of Mathematics. (n.d.). Encyclopedia of Mathematics. Retrieved May 29, 2021, from [https://encyclopediaofmath.org/wiki/Monty_hall_problem](https://encyclopediaofmath.org/wiki/Monty_hall_problem)

Multivariate Normal Distribution. (2013). [Graph]. [https://commons.wikimedia.org/wiki/File:MultivariateNormal.png](https://commons.wikimedia.org/wiki/File:MultivariateNormal.png)

Normal Distribution PDF. (2008). [Graph]. [https://commons.wikimedia.org/wiki/File:Normal_Distribution_PDF.svg](https://commons.wikimedia.org/wiki/File:Normal_Distribution_PDF.svg)

Normal Distribution Probabilities Visualization. (n.d.). [Graph]. [https://miro.medium.com/max/24000/1*IdGgdrY_n_9_YfkaCh-dag.png](https://miro.medium.com/max/24000/1*IdGgdrY_n_9_YfkaCh-dag.png)

Pick a door - Monty Hall Problem. (n.d.). [Illustration]. [https://slidetodoc.com/presentation_image/5569651af67b14db213690a748333a81/image-13.jpg](https://www.notion.so/5569651af67b14db213690a748333a81)

Population And Sample - Graphic Design. (n.d.). [Illustration]. [https://www.pngkey.com/detail/u2y3q8q8e6o0u2t4_population-and-sample-graphic-design/](https://www.pngkey.com/detail/u2y3q8q8e6o0u2t4_population-and-sample-graphic-design/)

Scatter Plot. (n.d.). [Graph]. [https://www.data-to-viz.com/graph/scatter_files/figure-html/unnamed-chunk-1-1.png](https://www.data-to-viz.com/graph/scatter_files/figure-html/unnamed-chunk-1-1.png)

Statistics and Probability. (n.d.). Khan Academy. Retrieved May 29, 2021, from [https://www.khanacademy.org/math/statistics-probability](https://www.khanacademy.org/math/statistics-probability)

Surrogate Opimization. (n.d.). [Graph]. [https://it.mathworks.com/videos/surrogate-optimization-1535996187824.html](https://it.mathworks.com/videos/surrogate-optimization-1535996187824.html)

Yang, L., & Shami, A. (2020). On hyperparameter optimization of machine learning algorithms: Theory and practice. Neurocomputing, 415, 295–316. [https://doi.org/10.1016/j.neucom.2020.07.061](https://doi.org/10.1016/j.neucom.2020.07.061)

Z table example. (n.d.). [Graph]. [http://qualityengineer.weebly.com/uploads/1/3/1/0/131059459/published/z-table-example.png?1584414181](http://qualityengineer.weebly.com/uploads/1/3/1/0/131059459/published/z-table-example.png?1584414181)

z-Table Cutout. (n.d.). [Graph]. [http://www.z-table.com/uploads/2/1/7/9/21795380/8573955.png?759](http://www.z-table.com/uploads/2/1/7/9/21795380/8573955.png?759)

- Follow-up topics

    ## Follow-up topics:

    **How to calculate the p-value**

    **Causal inference**

    [https://en.wikipedia.org/wiki/Causal_inference#:~:text=Causal inference is the process,component of a larger system.&text=Causal inference is said to,causality theorized by causal reasoning](https://en.wikipedia.org/wiki/Causal_inference#:~:text=Causal%20inference%20is%20the%20process,component%20of%20a%20larger%20system.&text=Causal%20inference%20is%20said%20to,causality%20theorized%20by%20causal%20reasoning).

    **Monte Carlo Simulation**

    [6. Monte Carlo Simulation](https://www.youtube.com/watch?v=OgO1gpXSUzU)

    **random walk theory** [https://www.investopedia.com/terms/r/randomwalktheory.asp](https://www.investopedia.com/terms/r/randomwalktheory.asp)

[Self-Reflection - Alexander Kuebel, alexander.kuebel@code.berlin, WS21, SE_30 Probability & Statistics, Data compression algorithms for streaming sensor signals in industrial, resource-constraint networks using autoencoder (neural networks)](https://www.notion.so/Self-Reflection-Alexander-Kuebel-alexander-kuebel-code-berlin-WS21-SE_30-Probability-Statisti-9f13a05159b6491cae20c36bd1ee762d)