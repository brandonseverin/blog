---
toc: true
layout: post
description: School of Physics, The University of New South Wales Sydney, Australia
categories: [notes, talks]
title: "Gordon Godfrey Workshop on Spins, Topology and Strong Electron Correlations"
---

# Gordon Godfrey Workshop on Spins, Topology and Strong Electron Correlations

> School of Physics, The University of New South Wales, Sydney, Australia

> [Program: https://newt.phys.unsw.edu.au/Godfrey/2022/program_oral/](https://newt.phys.unsw.edu.au/Godfrey/2022/program_oral/)


## Mark Friesen | Wiggle Well: engineering valley and spin-orbit properties of silicon 

- wiggle well solves two problems related to scale up
    - reliably large valley splitting 
    - large intrinsic spin-orbit coupling without micromagnets
- Valley splitting variations are very large
    - 
- Valley vs spin qubits
    - quantum dot qubits are formed at the very bottom of the conduction band in silicon, 
    - Note conduction band minimum doesn't fall within the center of the brillouin zone
    - two valleys form - the valley states compete with the spin as a possible qubit. 2x2-fold energy level degeneracy in a quantum well
    -if the valley splitting is very small, relative to the zeeman splitting then the valley will be the qubit rather than the spin
    - Want sharp interfaces and narrow quantum wells to increase the valley splitting but there is still large variability. 0.33nm sharp interface
- Shape of the dot changes but not the location
- Valley splitting behaviour is fully explained by alloy disorder of random Si-Ge alloying
- Variability occurs because the dot samples fluctuations differently at different locations
- Concentration fluctuations have a small component of short-period wiggle well

### Best schemes for valley splitting
- deterministic scheme: find a way to grow the short-period wiggle well
- randomly dominated scheme: add uniform Ge to the quantum well and find a way to reposition the dot

### Scale-up problem (2): weak spin-orbit coupling in Si
- Electrically Driven spin resonance with a micromagnet
    - fab a micromagnet on top of the dot, drive it electrically
- EDSR via spin-orbit coupling (Rashba 1960s)
- Experimental suggestion of spin orbit coupling in wiggle well because g-factor is not equal to 2.
-sp3d5s theory predicts large enhancements of dresselhaus spin-orbit coupling

### Conclusions
- wiggle wells exist
- enhancing valley splitting
    - deterministic strategy short-period WWW
    - Randomly dominated strategy: Ge in the quantum well; reposition dot
- Enhancing spin-orbit coupling
    - deterministic strategy: long-period wiggle well

## Kristiaan De Greve (imec) | Si spin qubits fabricated in advanced, industry-standard CMOS facilities: state of the art and outlook

- novel integration 
- Si MOS
    - best for valley splitting , worst for charge noise due to oxide interface and defects
- Si/SiGe
    - worst for valley splitting, best for charge noise
- Interface characterisation via Hall 
    - can be done at relatively higher T
    - fast measurements
    - process optimization

## Amanda Seedhouse | Wavelet-based methods for noise analysis in

- Climate forecasting
    - sea surface index and a function of years - el nino and la nina
    - increase in data - better predictions

- quantum information forecasting
    - nuclear and electron spin paris with hyperfine coupling
    - we know there is fluctuation per hour
    - humans can forecast a stable point in the data
    - useful to have a theoretical framework to forecast
- Increase in data 
    - 1+ GB data/hour with engineering efforts (low latency FPGA)
    - temporally and spatially correlated signals
        - spatially as we are looking at the differences between qubit one and qubit two
    - better predictions
    Environemntal modelling and software
        - lots of literature out there on wavelets so taking inspiration from climate science
- Wavelet is a wavepacket localised in time and frequency
- A wider wavelet means that the amplitude of the wavelet will be smaller
Why wavelets - edge detection
    - edge detection for sharp features e.g. readout events or two-level fluctuators robust against 1/f noise

- quantum computing
    - Variance transformation - correlations
    in the larmor frequency we see long scale drift which is removed after the variance transformation
    - 
- Use in quantum computing
    - why wavelets - useful for edge detection - we really want to understand the noise in our devices so if we can break down the noise into its frequency components then we can understand the sources of noise. 
        - this can also lead to better controled pulses
        - less feedback
        - efficient quantum error correction

## Rajib Rahman | Vacancies in 2d mateirals: imaging spin, valley and orbital states

- as you cool down the devices you see these Coulomb peaks where are beleived to be coming from the vacancy centres 
- 

## Guido Burkhart - fingerprints of qubit noise in cavity qed
- qubit noise is often limiting quantum gate fidleieties and qubit coherence. Charge noise is the issue across the board, even for superconducting qubits
- dephasing/longitudinal noise often most dangerous
- characterize noise - many methods and results
- efficient characterisation needed also in qubit arrays
- 
- characterising noise qubit noise - quantum dot ransport flank method, do it by sitting on the flank of a Coulomb noise, 
    - This doesn't actually measure the qubit noise though
- dynamical decoupling (need high-fidelity issues)
- here: cavity QED with general qubit

- how to do circuit QED
    - Really just need some qubit with energy splitting coupled to a cavity mode
    - magnetic field gradient, put a single electron in a double dot
    - 

## Maja Cassidy | Experimental progress in hybrid super semi-devices

- Majorana recipe 
    - one=dimensional quantum wire
    - spin-orbit interaction superconductivity, tune chemical potential and apply magentic field
    - induce p wave superconductor with majorana zero modes
- How do we measure Majoranas?
- Burden of proof:
    - why is the gap so soft
    - why is the zero bias peak so small?
- Soft gap linekd to discorder - majorana signatures mimicked by disorder
    - became a materials science problem

- Got better materials but didn't have a better way of measuring
    - Non-local conductance measurements - measure the full conductance matrix of the device
    - Would give information about the induced gap
- Topological gap protocol
    - stage 1
        - tune to N=1 subband
        - local conductance shows regions of parameter space with stable ZBPs at each end, do this across many gate voltages
    - stage 2
        - non local conductance shows bulk phase transition - gap closing and reopening

- Prospects for realiszing majorana machines:
    - topological gap 20-30ueV
    - need to keep all experiemntal parameters below this
        - temperature
        - readout frequency
    - disorder dominates
    - Going to be hard to build these devices and scenarios

- What can we do?
    - Better dielectrics:
    - Dit ~0.5e12 (InAs)
    Dit ~0.1e11 Si/SiGe
    - new superconductors Pb, Sn
        - challenging to process due to phase changes
    - New semiconductors: Ge/SiGe? PbTe
    - More robust measurements

## Rainer Blatt | Quantum Simulations with trapped-ion spin chains
> The Innsbruck quantum processor - characteristics

- 100 ions in a chain
- Ca+ qubit s1/2  and D5/2
- You can measure the state of the qubit by shingin in 397 nm light
- try and remove the degree of phonos in the system
- AQT - made in Tirol
