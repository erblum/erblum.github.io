---
title: "Asynchronous byzantine agreement with subquadratic communication"
collection: publications
category: conferences
permalink: /publication/2020-11-16-Subquadratic-ABA
excerpt: 'This work (co-authored with Jonathan Katz, Chen-Da Liu-Zhang, and Julian Loss) presents asynchronous Byzantine agreement (BA) protocols with expected sub-quadratic communication complexity tolerating an almost-optimal number of adaptive corruptions.'
date: 2020-11-16
venue: "TCC '20: Theory of Cryptography Conference"
paperurl: 'https://eprint.iacr.org/2020/851.pdf'
citation: #"Erica Blum, Jonathan Katz, Chen-Da Liu-Zhang, and Julian Loss. 2020. Asynchronous Byzantine Agreement with Subquadratic Communication. In Theory of Cryptography: 18th International Conference, TCC 2020, Durham, NC, USA, November 16–19, 2020, Proceedings, Part I. Springer-Verlag, Berlin, Heidelberg, 353–380. https://doi.org/10.1007/978-3-030-64375-1_13"
---

Understanding the communication complexity of Byzantine agreement (BA) is a fundamental problem in distributed computing. In particular, for protocols involving a large number of parties (as in, e.g., the context of blockchain protocols), it is important to understand the dependence of the communication on the number of parties $$n$$. Prior to our work, adaptively secure BA protocols with $$o(n^2)$$ communication were known in the synchronous and partially synchronous settings, but no such protocols were known in the fully asynchronous case.

We show asynchronous BA protocols with (expected) subquadratic communication complexity tolerating an adaptive adversary who can corrupt $$f<(1-\epsilon)n/3$$ of the parties (for any $$epsilon$$). One protocol assumes initial setup done by a trusted dealer, after which an unbounded number of BA executions can be run; alternately, we can achieve subquadratic amortized communication with no prior setup. We also show that some form of setup is needed for (non-amortized) subquadratic BA tolerating $$\Theta(n)$$ corrupted parties. (In concurrent work, [Cohen, Keidar, and Spigelman](https://arxiv.org/abs/2002.06545) also present a protocol for adaptively secure subquadratic BA. Their work makes use of different assumptions: they consider a non-standard network model that places a mild restriction on the adversary's ability to reorder messages, but on the other hand are able to forgo the stronger computational assumptions and trusted dealer used by our approach.)

As a contribution of independent interest, we show a secure-computation protocol in the same threat model that has $$o(n^2)$$ communication when computing no-input functionalities with short output (e.g., coin tossing).
