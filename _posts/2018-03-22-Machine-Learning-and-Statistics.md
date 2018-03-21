---
layout: post
mathjax: true
title: Machine learning and statistics – an ode to Warren Sarle
published: true
---

Going back to the 1990s, when I was new to the world of neural networks, one of the first places to visit when it came to discourse and learning was the [USENET]( https://en.wikipedia.org/wiki/Usenet)  newsgroup called [comp.ai.neural-nets]( https://groups.google.com/forum/#!forum/comp.ai.neural-nets). 

Every newsgroup worthy of following then had an FAQ, and comp.ai.neural-nets was no exception. It had one that was considerably detailed and maintained by one Warren Sarle. The FAQ became the go-to place for a quick reference into all things about neural networks. It grew over time and was [distributed in seven parts]( ftp://ftp.sas.com/pub/neural/FAQ.html).
Warren was from the SAS Institute and naturally (and highly probably!) a statistician by training. And that’s where the FAQ benefitted from his input. As an undergraduate working on a final-year project in the world of higher-order optimisation for multi-layered perceptrons, I took a fascination to Warren’s take on the connection between statistics and neural networks. In particular I’ll provide a  cut-and-paste of the paragraph that connects neural networks to statistical models: _
1. Feedforward nets with no hidden layer (including functional-link neural nets and higher-order neural nets) are basically generalized linear models.
2. Feedforward nets with one hidden layer are closely related to projection pursuit regression.
3.	Probabilistic neural nets are identical to kernel discriminant analysis.
4. Kohonen nets for adaptive vector quantization are very similar to k-means cluster analysis.
5. Kohonen self-organizing maps are discrete approximations to principal curves and surfaces.
6. Hebbian learning is closely related to principal component analysis.

He also caveated the two following items as having _no close relatives in the statistics literature_ then:
1. Reinforcement learning (although this is treated in the operations research literature on Markov decision processes).
2. Stopped training (the purpose and effect of stopped training are similar to shrinkage estimation, but the method is quite different).

Warren was very specific when using words like _identical_ and _closely related_. I subsequently found a paper that Warren self-referenced called “Neural Networks and Statistical Models” \[1\]that was published in 1994. Here’s a verbatim from the paper on terminology:

<style>
.tablelines table, .tablelines td, .tablelines th {
        border: 1px solid black;
        }
</style>
| **Statistical term** | **Neural network literature** |
| variables| features |
| independent variables | inputs |
| predicted values | outputs |
| dependent variables | targets or training values |
| residuals | errors |
| estimation | training or learning |
| estimation criterion | error or cost function |
| observations | patterns or training pairs |
|parameter estimates | synaptic weights |
| interactions | higher order neurons |
| transformations | functional links |
| regression and discriminant analysis | supervised learning |
| data reduction | unsupervised learning |
| cluster analysis | competitive learning |
| interpolation and extrapolation | generalisation |
{: .tablelines}

Some of the terms on the right-hand side of the table have expanded in the new frontier of machine learning. For example supervised learning does mean more than regression these days. And would you refer to the higher order neurons in deep learning networks as _interactions_? However the spirit of the paper still holds and Warren had clearly demonstrated that many a term used by the machine learning community did exist for several decades or centuries before being re-coined. I have since used the content of this paper as an intro to many of my machine learning talks. 

![ Neural Networks and Statistical Models paper by Warren Sarle, 1994]({{ site.baseurl }}/images/Article_002-Warren-Sarle-paper.png "Neural Networks and Statistical Models by Warren Sarle, 1994")
Figure 1. An extract from Warren Sarle's paper \[1\]

Machine learning very much takes a computational approach to a problem, where else statistics is much more systematic and analytical. Before the recent breakthroughs in deep learning, machine learning was very much seen as the wild west of computational prediction with limited applications. The outcome of that is what, I believe, produced the disconnect with statistics.

When I started on my Ph.D. journey in the mid-1990s I believed that I needed to learn statistics, thanks to Warren’s paper. I was fortunate that the University had recently introduced a researcher training programme, that effectively allowed me to sit through a 1-year course in statistics that would contributes compulsory units towards a Ph.D. (the final thesis was still key). The course was given at the masters level, so included key subjects on multivariate statistics, statistical modelling, hypothesis testing etc., which I still find invaluable these days. When it came to me supervising Ph.D. student myself, I always stressed the importance of a strong grounding in statistics.

As the field of data science is commoditised, specialisations in statistics seem to play a less important role. I am of the opinion that a good data scientist will require some grounding in statistics. I would be interested to know your thoughts, and where you stand. Do you agree or disagree with me? If you are data scientist and lack a good grounding in statistics, do you feel it harder to do your job? Do you think our next generation of data scientist is sufficiently equipped, or should we aim to train them up? 

And finally, whatever happened to Warren Sarle? Answers on a postcard.

##References
\[1\] Sarle, W.S. (1994), "Neural Networks and Statistical Models," Proceedings of the Nineteenth Annual SAS Users Group International Conference, Cary, NC: SAS Institute, pp 1538-1550. [Download from CiteSeerX]( http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.27.699)
