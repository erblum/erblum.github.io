---
title: "Synchronous consensus with optimal asynchronous fallback guarantees"
collection: publications
category: conferences
permalink: /publication/2019-11-22-Sync-consensus-with-async-fallback
excerpt: "This paper (joint with Jonathan Katz and Julian Loss) initiates the study of the network-agnostic model, where the network may be either synchronous (with a higher number of faulty parties) or asynchronous (with a lower number of faulty parties), but parties don't know which. We show a protocol for Byzantine agreement that tolerates $$t_s$$ faults in the synchronous case and $$t_a$$ faults in the asynchronous case for any (fixed) $$t_s,t_a$$ such that $$2t_s+t_a<n$$, where $$n$$ is the number of parties, and prove that this tradeoff is optimal."
date: 2019-11-22
venue: "TCC '19: Theory of Cryptography Conference"
slidesurl: #'http://academicpages.github.io/files/slides2.pdf'
paperurl: 'https://eprint.iacr.org/2019/692.pdf'
citation: #"Erica Blum, Jonathan Katz, Julian Loss (2019). Synchronous Consensus with Optimal Asynchronous Fallback Guarantees. In: Hofheinz, D., Rosen, A. (eds) Theory of Cryptography. TCC 2019. Lecture Notes in Computer Science, vol 11891. Springer, Cham. https://doi.org/10.1007/978-3-030-36030-6_6"
---

This is the first paper in a line of work on *network-agnostic protocols*: protocols that are secure for up to $$t_s$$ corruptions when the network happens to be synchronous, and still provide "fallback" security for a lower threshold of $$t_a$$ corruptions when the network is asynchronous. The original paper focuses on Byzantine agreement, with follow-up work extending our techniques to [secure multiparty computation](https://eprint.iacr.org/2020/740.pdf) (Blum, Liu-Zhang, and Loss, CRYPTO '20) and [state machine replication](https://eprint.iacr.org/2020/142) (Blum, Katz, and Loss, Asiacrypt '21).