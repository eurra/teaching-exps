# When the problem is the problem

Sometimes, The coding part of solving a specific problem is not the main struggle when learning programming, but to clearly understand the problem itself that is being solved. The more beginner the learner, more time is spent on learning the language concepts and mechanics, commonly over basic problems. The more advanced is the learner, more time is spent on problems rather than languages, so the addressed problems can become more hard. I commonly illustrate this situation to early-years students with this graph:

<img src="learning-graph.jpg" width="700"/>

The green curve means the struggle of the learner when using programming languages, while the blue one means his capabilities for solving problems through programming. This graph represents the *successful* learning process: at some point in time, the blue curve should surpass the green one, i.e., the *language domination point*. At this point, the learner can further concentrate more on the problems than the tool (the programming language), thus his problem solving skills can develop faster.

On the other side, learners may get in the following situation:

<img src="learning-graph-2.jpg" width="700"/>

which is the inverse one. The learner stagnate on understanding the language, and the problem solving skills never develop. These are commonly the situation of student dropouts. The ideal process should motivate the green curve to descend as quickly as possible.

For advanced students, I commonly spend more time addressing problems on more advanced subjects. In the past I had the opportunity of teaching optimization topics related to my past research, particularly *heuristic algorithms*. These tools are suited for finding good solutions (non necessarily optimal) of very complex combinatorial problems, i.e. the ones in which you need to set values to a very large number of variables, and from that, calculate some kind of quality metric that tells you the solution fitness. In formal terms, these problems are commonly represented and know as *Constraint Satisfaction Problems (CSP's)*. So, to understand heuristic algorithms, previously one must understand CSPs.

And guess that, to teach and to understand CSPs is hard! That is because, formally speaking, a CSP is expressed through a mathematical model that abstract all the components of the domain. For example, consider the *Multidimensional 0-1 Knapsack Problem (MKP)*, a CSP whose explanation can be summarized as follows:

- There is a set of *knapsacks*, each one with a specific *resource capacity*.
- There is a set of *items* that can be selected in a specific solution.
- When a item is selected, it consumes a specific amount of resources *for each knapsack*, and this quantity can be different for each knapsack.
- Each item yields a specific *profit* when selected.
- The goal of the problem is to find a subset of items that yields maximum profit without exceeding the resource capacities for all the knapsacks.

The formal mathematical model for the above description is the following:

Maximize $z = \sum_{j=1}^{n}{c_j x_j}$, subject to:

$\sum_{j=1}^{n}{a_{ij} x_{ij}} \le b_i, \qquad i \in M = \{1,2,...,m\}$

$x_j \in \{0,1\}, \qquad j \in N = \{1,2,...,m\}$

with $M$ the set of knapsacks, $N$ the set of items, $c_j$ is the profit that yields the $j$ item, $a_{ij}$ is the amount of resources that the item $j$ consume from knapsack $i$ when selected and $b_i$ is the resource capacity of the knapsack $j$.



[MKP Viewer](https://html-preview.github.io/?url=https://github.com/eurra/teaching-exps/blob/main/csp/mkp-viewer/index.html)