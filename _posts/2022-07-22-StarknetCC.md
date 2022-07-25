---
toc: true
layout: post
description: "Paris 2022"
categories: [notes, talks]
title: "StarknetCC 2022"
---
> 20220722

## Opening ceremony - Only Dust
- a lot of the big brains in the discord
- we want everyone to build together
- tokenomics have been revealed, - reward people who are building for the ecosystem
- Notion of gating - not all contributions are the same
    - some open to everyone and some require prerequisites
- Have more than 100 contribution hours
- want to be the number go to platform for contribution in the starknet ecosystem and then others ecosystems

## Uri Kolodny - Starknet: scaling Ethereum by devs, for devs
- the rate of change of where we started to where we are today is very interesting
- Starks hit mainnet June 202, July 2022 Foundation and token proposal. Stark was a mathematical paper in 2018
    - Starknet announced on Jan 2021
- Phases:
    - 1 - feature completeness e.g. cairo 1.0
    - 2 - scale, recursion.
    - 3 - decentralisation e.g. token
- Disproportionate number of people in the starknet ecosystem who love hearing that can’t be done then then proving people wrong
- Newsletters, swag and northstar
- L2 beat
- 1000 devs building in cairo
- 400 GitHub repos, 20 companies DAOs raised over 100M, 200 grants
    - 5 hackathons
- Giza on the blockchain
- Skyro, transpiler: functional languages to cairo
- Auditing services: ABDK, consensus, crypto experts, nether mind, Openzep, peck shield, trail of bits
- The last time we had a fresh start was with Ethereum, let’s build some new and exciting stuff. Let’s learn and build better.
- Braavos, fiat onramp, int with layer swap, metamask is coming before the end of the year
- Oracle networks: Empiric, Stork
- Sustainable development of public goods is key, we want to make sure this is done well and in a decentralised fashion
- L3: hyper scale control: for developers, exploring features data solutions, and verifiable VMs
    - permissionless?
    - You need social consensus before moving lower level stuff e.g. EIP 1559
    - On L3 you can test these experiments and then come to the community with the results of your experiment.
    - Remember Cairo can be used to build other bits fo verifiable virtual machines

## Eli Ben Sasson - Starks ecosystem: StarkNet next steps
- Starks prove integrity
- > do the right thing even though no one is watching - CS Lewis
- Scalable proofs of integrity
    - privacy 
    - scalability
        - the size of the proof and running time is exponentially smaller than running the computation itself
        - 150 NFTs in a block —> 2M NFTs in a block (we do this day in and day out)

### 30 years of math
- the margin of error only depends on the size of the sample, not the size of the population
    - the same holds for verifying the integrity of the computation
    - a single reliable pc can monitor the operation of a herd of supercomputers working with possible extremely powerful but reliable software and untested software
        - this assumes execution trace written in a nice format
- Starting from state of accounts whose hash is x, I processed 10,000 Ethereum patients using program P, and the hash of the new system state is y
    - PCP
    - This builds a sudoku like contrarians system
        - The prover is supposed to fill in a solution, and submit this to a verifier
        - The verifier opens up a few contrasts randomly and checks them
        - If the all the sampled constrains are satisfied the verifier is happy
        - In a STARK there is an interactive back and forth between the verifier and the prover
            - Many 3D sudokus done by the prover and the verifier samples from one of them
        - The verifier doesn’t need to open up all the sudokus and open up all the contrasts
    - Magic Theorem
        - verifier doesn’t specify all constraints
        - verifier samples constraint succinctly
        - Proof of true statement satisfied all constraints
        - Any proof of false statements must make 99% of constraints unsatisfied - this is why you only need to sample a few
- STARKS use math to enforce the driver of the bus to operate with integrity
    - ETH everybody takes their own car
    - Centralised: one bus, have to trust the driver is good
- Problems: 
    - stark ware can’t steal funds
    - stark ware can censor tx
    - stark ware may freeze system
    - stark ware may stop maintaining/upgrading
    - stark ware small - 100 employees

### Next steps
- public good, this is done via StarkNet
- The reason for the token is not a fund raise
    - starknet needs the token for decentralisation
    - Have raised $260M since 2018
    - started with $6M
    - Build tech, get token
- Centralized today:
    - operator: sequencer and prover
    - software: cairo Vm, OS
- Foundation has mission to maintain starknet as a public good
- Token allocation: smart contract developers will get a portion of fees that are paid. 
- Core developers: will need human discretions and a mechanism tbd
- Developers will receive tokens first before community rebates


## WARP Transpiler: Write solidity code, deploy to starknet
- install from source
- transpile example contract
- then hack
- emr

https://github.com/NethermindEth/warp/issues/622

- they have there own version of the solidity compiler, nether-solc, need to maintain it. main thing is to deal with the addresses
- names of functions and variables are mangled to remove potential clashes
- Should be able to deploy code with contract factories by wednesday
- delegate call transpilation in a month 

