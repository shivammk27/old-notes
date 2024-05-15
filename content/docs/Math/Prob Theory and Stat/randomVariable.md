---
title: Random Variable
type: docs
---

## Random Variable

Random variable is a function which maps the outcome of a simple random experiment to a real number.
denoted by capital italized roman characters like {{< katex >}}X{{< /katex >}} or {{< katex >}}Y{{< /katex >}}.

Suppose that a coin is tossed twice so that the sample space is {{< katex >}}S={HH, HT, TH, TT}{{< /katex >}}. Let {{< katex >}}X{{< /katex >}} represent the number of heads that can come up. With each sample point we can associate a number for {{< katex >}}X{{< /katex >}} as shown below.

| Sample point | HH  | HT  | TH  | TT  |
| ------------ | --- | --- | --- | --- |
| X            | 2   | 1   | 1   | 0   |

### Types of Random Variable

- Discrete
  - can take finite or countably infinite number of values
  - probability distribution PMF :
    {{< katex >}}
    \begin{cases}
    P(X=x) &\text{if }  x ∈ Ω \\
    0 &\text{if } x ∉ Ω
    \end{cases}
    {{< /katex >}}
- Continuous
  - takes on a noncountably infinite number of values
  - probability distribution PDF : {{< katex >}}P(a \leq X \leq b) = \int_{a}^{b} f(x) dx{{< /katex >}}

### Probability Function
A probability function is a mathematical function that provides probabilities for the possible outcomes of the random variable, {{< katex >}}X.{{< /katex >}} It is typically denoted as {{< katex >}}f(x){{< /katex >}}.
1. **Probability Mass Function** \
A probability mass function (PMF) is a function that gives the probability that a discrete random variable is exactly equal to a certain value. In other words, it maps each possible outcome of a discrete random variable to its probability of occurrence.\
If {{< katex >}}X{{< /katex >}} is discrete, then {{< katex >}}f(x) = P(X=x){{< /katex >}}. In other words, the PMF for a constant,{{< katex >}}x{{< /katex >}} , is the probability that the random variable {{< katex >}}X{{< /katex >}} is equal to {{< katex >}}x{{< /katex >}}. \
Properties of PMF :
    - {{< katex >}} {f(x) ≥ 0}{{< /katex >}} for x in sample space otherwise 0.
    - {{< katex >}} {\sum_{x}^{} f(x) = 1}{{< /katex >}}.

2. **Probability Density Function**\
If the random variable is a continuous random variable, the probability function is usually called the probability density function (PDF). Contrary to the discrete case, \
{{< katex >}}f(x) \neq P(X=x){{< /katex >}}
Properties of PDF :
    - {{< katex >}} {f(x) ≥ 0}{{< /katex >}} for x in sample space otherwise 0.
    - Area under the curve is equal to 1.

3. **Cumulative Distribution Function**\
A cumulative distribution function (CDF), usually denoted 
{{< katex >}}F(x){{< /katex >}}, is a function that gives the probability that the random variable, {{< katex >}}X{{< /katex >}}, is less than or equal to the value {{< katex >}}x{{< /katex >}}.



### Discrete Probability Distributions

Let {{< katex >}}X{{< /katex >}} be a discrete random variable, and suppose that the possible values that it can assume are given by {{< katex >}}x1, x2, x3, . . . ,{{< /katex >}} arranged in some order. Suppose also that these values are assumed with probabilities given by :

{{< katex >}}
P(X=x_k) = f(x_k),k = 1, 2, 3, 4,...
{{< /katex >}}

It is convenient to introduce the probability function, also referred to as probability distribution, given by :

{{< katex >}}P(X=x) = f(x){{< /katex >}}

For {{< katex >}}x=x_k{{< /katex >}} this reduces to (1) while for other values of {{< katex >}}x, f(x) = 0{{< /katex >}}.
In general, {{< katex >}}f(x){{< /katex >}} is a probability function if
1. {{< katex >}} {f(x) ≥ 0}{{< /katex >}}
2. {{< katex >}} {\sum_{x}^{} f(x) = 1}{{< /katex >}}
   where the sum is taken over all possible values of {{< katex >}}x{{< /katex >}}.

### Expected Value and Variance of a Discrete Random Variable
Expected value or mean of discrete random variable is denoted by {{< katex >}}\mu = E(X) = \sum x_i{f(x_i)}{{< /katex >}}. \
Formula basically says multiply each value by its respective probability and add all of them together.\
\
Variance of a discrete random variable is given by {{< katex >}}\sigma = Var(X)=(\sum x_i-\mu)^2{f(x_i)}{{< /katex >}}
Formula basically says take each value of x, subtract the expected value, square that value and multiply that value by its probability. Then sum all of those values.

--- 
1. https://www.gs.washington.edu/academics/courses/akey/56008/lecture/lecture4.pdf
2. http://users.stat.umn.edu/~helwig/notes/RandomVariables.pdf
3. http://www.stat.yale.edu/Courses/1997-98/101/ranvar.htm
4. https://www.stat.pitt.edu/stoffer/tsa4/intro_prob.pdf
5. https://byjus.com/maths/random-variable/
6. https://online.stat.psu.edu/stat500/lesson/3/3.1
