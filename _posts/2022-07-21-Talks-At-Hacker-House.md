---
toc: true
layout: post
description: "ethCC 2022, Paris, HackerHouse by WindRanger, EduDAO, BitDAO"
categories: [notes, talks]
title: "MEV/Flashbots talks at the HackerHouse "
---

> Talks at the HackerHouse, Paris 2022
> WindRanger, EduDAO, BitDAO
> Chaired by Tina, Steward/Researcher at Flashbots


## Cross-domain MEV & the crucial conundrum of proposer selection - Christopher Goes

- tendermint has a weird proposer sharing algorithm
    - each validator has a counter
    - decremented by current stake each height
- Github link cwgoes/tm-proposer-idris
- MEV attacks abound
- randomised proposer selection
    - super linear returns to centralisation
- cross chain MEV is a hard prob to solve, lol
    - cross-domain anticorr incentives
    - Shared mempools?
- > “Cosmos is going to be a lot of fun next year…”

Question: What if the total capital to realise the arbitrage doesn’t exist.
	- You’re bridging it
	- The block proposer gets to choose
	- Is the value of L1 tokens the MEV they can capture?


## Tarun Chitra - Towards Theory of Maximal Extractable Value
> Even rotten sandwiches can taste good in a while

**Link to paper is [here](https://people.eecs.berkeley.edu/~ksk/files/MEV_CFMM.pdf)**

- Thought: Do you ever find utilitarian MEV?
- Constant function market makers
    - e.g. uniswap
- sandwich attack with . have slippage limits
    - invariant functions
    - price and quantity impact can be the same
    - One assumption that is always made: almost all arbitragers are risk neutral, money losing arbs are when someone didn’t compute the backwards trade correctly
        - g is continuous and monotonically increasing
- The amount of quantity: concavity of the tasing function implies price and quantity slippage limits are equivalent

- How do we say this in quantity space (min max price)
    - is the slippage limit less than the ratio of the kappa, mu, you can upper bound the sandwich profit
- How do we talk aboutut MEV for aggregations of sandwich attacks
    - Routing? how much worse does my route get if a sandwicher gets in there somewhere
    - Link to the study of traffic congestion
        - Braess’ paradox

