---
toc: true
layout: post
description: "intro to starkware"
categories: [notes, talks]
title: "zk-SPARK StarkNet Bootcamp"
---
## Fields

- Define a field just for two operations
- A field is a set of integers with two fields
- Division is tricky because if we divide two integers we get may get a float
- 

### zk Ecosystem

- stark system came out in 1976
- Halo BulletProof - multi person computation. Need to go through ceremony to set up system
- ZKSNARKS have small proofs but require an initial setup and are not quantum resistant

### Rollups
- transaction execution is done outside layer 1
- data or proof of transaction is on layer 1 (incl. state transitions)
- Verifier is a contract on layer 1 and can secure the latest state
- zero knowledge proofs can be done recursively
    - a proof to prove 100 proofs are valid
    - layer 3 and layer 4 -> can create specific applications on each layer which passes proofs to layer 2 which bundles them into a single proof for submission to layer 1.

### Questions from the first session
- How does the colorblind verifier know which had the different colored balls are in. This relies on some form of a trusted setup, is this setup similar to the initial ceremony used in setting up the starknet ecosystem



—
Break
—




Interesting projects on Starknet:
- Game of Life
- Giza - machine learning on starlet

- transaction process: the state of the system is able to be reconstructed by running though the transactions in the blocks
- Signatures are done differently on starkness compared to ethereum. You have account abstraction in starknet as your account is a contract
- Drawbacks form transpilers
    - is the code that you wrote in solidity idiomatic for solidity?
- cairo playground is a great tool
- run a local node for testing as the bundling of transactions on testate takes a while
    - protostars and nile allow you to do this
- Protostar is better than Nile which is better than starknet CLI
- Voyager is the main block explore

## The cairo language
- you may use some of the implicit arguments that are passed to your function
- Hints
    - when we are writing a program we are trying to prove the correctness of the computation, not try and calculate this value
    - We therefore may want to pass the value that we want to prove into the programme as a hint
    - You need to use python for this
- Output
    - serialise word: output the values for different variables
    - a nice way to log things out from your code
    - This output is seen by the validator
- Entrypoint
    - this is the main function
- Should an argument be implicit or normal
    - The implicit argument is more around the low level things that ae happening around your code
    - Normal arguments are for the business logic - similar to those that you’d have in solidity
- Error messages and scope attributes
    - strange syntax, attribute must be a string
- This afternoon we go through some cairo examples and go through the language
- 1 hour break
    - then we will look at writing contracts
    - 
—
Break
—


`range_check_ptr` is to make sure things haven’t overflow
The other two implicit variables are for storage slots


https://github.com/ExtropyIO/ZKSparkWorkshop

## 20220717 - Day 2

- No loops in cairo, use recursion
- Validium mode: data is stored off chain
- Volition mode is a hybrid, data is stored off chain and on chain
- You can’t prove if a transaction is going to revert/result in an error.
    - The reason is that for a transaction to fail, one needs to prove that the transaction resulted in an error
    - Potential for denial of service attacks
- L1 to L2 messaging mechanism
    - Sequencers could skip messages, it is worth checking that the message has been passed on by the starkness sequencer
    - Sequencers may eventually need to put up a stake and it is slashed if they skip messages to incentivise fair good practise

- Gaming on starknet
    - regard things as final once submitted to the sequencer
    - Checkout Starknet react
