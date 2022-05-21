---
toc: true
layout: post
description: Oxford University's Institute for Ethics in AI, Sheldonian Theatre
categories: [notes, talks]
title: Using AI to Accelerate Scientific Discovery - Demis Hassabis
---
> Demis Hassabis, *co-founder and CEO of DeepMind*

- Fresh trim Demis 😉

## Intro to DeepMind

- DeepMind’s initial aim was a programme to achieve Artificial General Intelligence (AGI)
  - Step 1: solve intelligence.
  - Step 2: solve everything else.
    - “To advance science and benefit humanity”
- Two approaches to build AI
  - Expert systems
    - Limited to what they have already seen
    - Relies on hardcoded knowledge
  - Learning systems
    - Can generalise and learn new tasks
    - Inspired by neuroscience
- Merge deep learning and reinforcement learning
  - Deep reinforcement learning systems can learn new knowledge through a process of trial and error
  - Feedback loop: Observations —> Agent —> Actions —> Environment —>

## AlphaGo

- The Game of Go

  - The search space is huge. Number of configurations of the board is more than the number of atoms in the universe
    - All the computers in the world working for 1 million years couldn’t calculate all the possible moves.
  - Impossible to write evaluation functions unlike in Chess
  - Go players rely on intuition rather than calculation “this felt right”

- How do we do it (Alpha Go Zero)? - V1 neural network (NN) plays against itself 100k times. It picks moves at random. This generates a dataset - V2 neural net is trained on V1 - V2 NN plays V1 NN 100 times - Best NN (55% win rate) then plays against itself another 100k times - Cycle repeats

  - Combine the neural network with Monte Carlo search for efficient move choice.

- Beat Lee Sedol (18 time world champion) 4-1.
- Changed the way human beings view the game of Go.

  - Move 37 will go down in history.

- Generalisation
  - AlphaZero generalised AlphaGo to 3 games: Chess, Go and Shogi
    - New style of chess: Mobility over Materiality
    - It will sacrifice pieces to get more mobility for it’s remaining ones; The Immortal Zugzwang Game
    - Human Chess Grandmaster searches 100 moves per decision, Stockfish: 100K, AlphaZero: 10K

## Scientific Discovery

- What makes for a suitable problem?

  - Massive combinatorial search space
  - Clear objective function
  - Lots of training data or an accurate simulator to generate data.

- Protein folding problem

  - Can you predict the 3D form of a protein based only on its Amino Acid sequence?
  - Proteins are essential to life. Their 3D structure determines their function
  - It takes one PhD student (4 years) per protein structure.
  - Levinthal’s paradox: 10^300 possible confirmations for an average protein. Yet nature solves this spontaneously.
  - It was a long road to getting fully into protein folding. 90s intro at Uni full start 2016.

- Alpha Fold 2

  - AlphaFold 2 achieved atomic accuracy for protein structure prediction in 2020 CASP.
  - Needed 32 component algorithms. 60 pages of suppl. info. Every part was a requirement for Alpha Fold 2 based on ablation studies
  - Made the system completely end to end, rather than relying on an intermediate step.
  - Architecture: attention based neural net.
  - Included biological and physical constraints that didn’t impact the learning.
  - Start with domain knowledge. Generality is secondary.
  - 2 weeks to train. Prediction now takes minutes.
  - Predicted 20K proteins encoded by the human genome.

- Roadmap

  - Prioritise neglected tropical disease for proteins structure prediction.
  - Plan to solve 100m proteins over the next year. All proteins currently known to humans
  - New era: digital biology
    - Can you derive the laws of motion of a cell? Can you learn them?
  - Demis has been shipping. Ticking off childhood dream projects.
  - Many products you use will probably have interacted with code from DeepMind.
    - Data centre and grid optimisation.
    - YouTube bit rates

- Ethics:
  - Has been central to their mission from the beginning.
  - We should not move fast and break things.
  - Use the scientific method: deliberation and foresight. Control tests. Update based on empirical data. Aim to get a better understanding.

