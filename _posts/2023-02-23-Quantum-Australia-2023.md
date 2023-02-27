---
toc: true
layout: post
description: Sydney, Australia
categories: [notes, talks]
title: "Quantum Australia 2023"
---

> https://quantum-australia.com/quantum-australia

## Cathy Foley  - Quantum in Action
> Quantum has entered the lexicon of marvel movies
- you in industry need to be taking action now
- Will Australia lose out on this race due to lack of investments
    - Even Signapore invests more than Australia in to Quantum apparently?
- How do you see cooperation with the united states and the UK.

## State of the Nation - Panel discussion
- collaboration is a great way to find out where the market is heading
- international collaboration is just fun.
- Australia quantum alliance sitse under the australia tech council.


## Joel Wallman Keysight - bridging the gap between theory and experiment
- how to build a quantum computer
- Keysight is originally under HP
150 hubs - global support network

- acquired - signadyen, labber and quantum benchmark

- the quantum application
    - quantum algorithms researcher
        - developing quantum algorithms to solve real problems
- the quantum memory
    - quantum algorithms person needs to pass their algorithm to someone with expertise in fault-tolerance
    - quantum error correction researcher
        - developing ways of protecting quantum computer calculations/results from errors
        - error correction can be broken into multiple steps
            - encode logical qubit into a larger space
            - measure the error syndrome
            - apply a correction operator
            - decode teh logival qubits in post processing
- translating to physical control
    - quantum control researcher
    - developing ways of making quantum computers work properly
    - simple error correction protocol needs
        - measurments, x-gaes, hadamard gates, controlled-not gates
        - each needs to be translated into singals sent to hardware
- translating to fpga
    - fpga developer - enabling quantum computers to be operated efficiently with real-time decision making
        - output of AWGs specified by an array of voltages from the eaveform sampled at a finite rate
        - finit sampling causes aliasing, so need up/down converters
        - specify complex voltages and an LO frequency, difitally synthesize
        - want to send a small number of sampled waveforms to the FPGA
        - But if the w
        - upload one waveform and a starting phase for each waveform
            - integrate and classify 


## Warwick Bowen - The potential for quantum in biotechnology
- chief investigator australian quantum systems
- biochemical dynamics span a vast range of spatial and temporal scales
- technological bottleneck
    - imaging - harder to image stuff as they get smaller, and as they get smaller, they move faster
    - modelling on the scal of atoms is fine, but if you want to go beyond that then you need to start making approximations
- Theortical modlecular science laboratoty riken youtube - life is motion in some sense
- A quantum problem
- Quantum market cap 260M projected to reach 9B after 2030
- Mckinsey estimates the majority of the future quantum industry will be allocated to biotech (chemistry and pharma)
- Australian Research Council Centre of Excellence in Quantum Biotechnology
- single protein dynamics
    - partnership with IBM, employing teir quanutum computing technoloogies
        - optical nanocavities
        - Hartree-Fock on a superconducting qubit quantum computer - google AI quantum
            - a few atoms, ten to 20 qubits, far from chemical precision
    - noise-robust ground state energy estimates from deep quantum circuits - Vallury 2022
        - quantum induced moments approach: two orders of magnitude improved robustness
- Quantum optomechanics - Gerard Milburn, Wawrick P Bowen
- Enzyme catalysis - ammonia production
    - crucial for us, plants do it naturallyA
- useful tech coming out of the centre in 4 years 


## Panel - the role of governemnt in quantum ecosystem
- qctrol is australias first australia backed comany
    - partner with vendors and diraq
    - want to deliver utility from quantum systems
    - larged the largest series B in quantum
        - have had to sell ownership of the company to further comapany
        - european companies have been able to raise from government without having to sell the company
    - it is a market failure when world changing company is not supported by the private investors.
- starshots, think of moonshots but going further
- community needs to articulate how their tech can be used to government more effectively.


## Barry Sanders - Quantum Canada
- creative destruction labs - accelerator
- canada wants to create darpa like aganecy but doesn't want pure defense strategy
- CREATE program = trains talent and funds internships
- Quantum city - a world leading quantum innovation hub fostering research breadkthroughs and driving a thriving quantum technology economy in Alberta
    - Quantum alberta
- quantum computing diploma in graduate studies


## Jeremy O'Brien - PsiQuantum 
- Startup company
- HQ in California, team members in UK, 
- foudning thesis - utility means error correction, which means millions of qubits, 
- phtons 
    - cips can be manufactured using mature semiconductor fabs
    - cooling - photons do not feel heat and operate at less demandign cryogenic temperatures
    - connectivity - interconnect can be achieved using conventionaloptical fiber
    - thermal and EM insensitivity permits colocation of complex control electronics
    - Names: David Reilly, Microsoft, Andrew Dzurak and Michelle Simmons have looked at what is required.
    - solving the connectivity issue: approx 50x reduction in run-time for cimpiled fault-tolerant algorithms
    - GHz clock - crack RSA in 48 hours
- 5000 CPU hours to evaluate an architecure 
- Map of photonic quantum computer
    - Photonic chip, board-level assembly , cryogenic cabinet, facility
- what is needed for photonic quantum computing to work?
    - lots of engineering challenges
- testing - can characterise devices at room temperature with robits rapidly    
    - there are still cryogenic tests that they have to do.
- nanowire cotrol within nm across wavefers
- film thickness within angstron reliability
- single photon generation - spontaneous emission with four wave in silicon, 99.9% purity
- chip to fiber coupling eeficiency = 98% want to be better than 0.99
- Multiplexing - haven't seen thhosands of qubits because of the need of multiplexing
    - non-deterministic outcomes
    - biggest challenge
    - take a ton of non-deterministic operations and run them in parrallel and pick one out in the end
    - optcal phase shifting material needs to be really good. Typically use LiNib
    - BTO - 1000mp/V electro optic coefficient
    - Buit the biggest molecular beam epitaxy in San Jose
        - moten titanium at 1000 deg and liquid helium at few K
    - a year to go from 350pm/V to 1000pm/V in their wafers
- 120dB of filtering done off chip
- thermal heaters used a phase shifters
- path to higher temp operation. the detectors are teh only thing that need to be cold. manufacturable metal superconductor. Pushhing transition temeperature up to 30K
- 

- contious variable vs discrete variable quantum qomputing. 
    - some people say that you can do a hybrid approach
    - Hybridsing systems are really hard though.

- How are photonic qubits initialised - just a single photon intl a wave guide
- fibre coupling - do you want to join the company 
- 

## Hon Ed Husic MP - federal minister for inductry nad science - Delivering on australia's strengths in quanutm technologies

- Acknowledgement 
- Not announcing quantum strategy today 
- 19k jobs by 2045. conservative estimate. mostlikely 50k
- could add 9Bn to GDP
- 1B fund, loands, bills and equity. Similar fashion to clean energy corporation fund
- Vikram sharma - quantum random number generation
- QCtl - softtware to IBM and regetti. team from 80 to 120 people


## Panel: Cyber security in the quantum age Alexey Bocharnikov, APAC Quantum Technology Leader, EY

Lily Lidong Chen, Manager, Cryptographic Technology Group, Computer Security Division, National Institute of Standards and Technology, USA (V);
Julian Fay, Chief Technology Officer, Senetas;
Peter Rohde, Senior Lecturer, UTS;Gavin Brennen, Professor, Macquarie University (Panel Chair)    - you don't just a cryptographic system to be secure. You also want it to work.
- a quantum network will be more sparse than classical Mensing it may be possible to cut nodes of the network off due to reduced oath redundancy
- bear in mind QKD will be used to protect precisely the things that you don't want to cut off
- QKD doesn't meet the assurance requirements of most western governments at the moment. PQC is the future more than QKD. PQC can be used in a hybrid manner and QKD could be used to complement classical things
- want to be able to change the underlying encryption algorithm when you need to. This is hard.
- organising an full upgrade of any organisation will be very hard. It may take decades for many organisations and will be continual learning from their mistakes. Improvements will be gradual.
- how paranoid should we be with PQC? Is it as safe as we believe it to be.
- will need to consider the cost of an attack, may not be worth it.
- quantum internet and computing. Homomorphic encryption and blind computing. You don't want the person performing your computation to know what you're computing. Can be done with relatively little overhead if you have a quantum encryption network. Important as the things we'd be computing are likely to have high value implications.
- Decentralised quantum computing.
- should we trust nation states with the security of quantum cryptography in terms of back doors.
- looking for hashing collisions.
- Hashing algorithms are secure by doubling the key length## Michael Cuthbert, Director, National Quantum Computing Centre (NQCC) UK- see their role as not trying to do everything themselves. Want international collaboration and accelerate the roadmap for the wider ecosystem
- establishing a new national laboratory
- build consensus, don't assume that their is a clear or shared vision amongst key stake holders
- plan for life
- hire early , recruitment is tough. The more you can build the team up the faster you can go.
- stay focused. Have a clear plan, be ready to adapt but avoid snap responses.
- over communicate. Keep everybody updated. Don't assume an audience that has heard the plans that they were listening.##  Andrew Dzurak, CEO & Founder, Diraq- quantum counting private investment greater than $1B per annum
- fault tolerant market will eventually be a fraction of $1T dollars per annum.
- reading: Kearney 2021: Quantum Computing. Why should you care
- Reiher - Elucidating reaction mechanisms on quantum computers
- Only 10e5 qubits are needed if the error rates are 10e-9
- networking is a huge challenge for current quantum computing architectures. Diraq wants the opposite. Quantum computer on a chip - similar to current computers
- history of 1998 to 2023 of work on Silicon.
- $31M from Army research
- qubits made by advance semiconductor manufacturing - J Clarke
- get 9 logical qubits in 3 years
- start the move towards to fault tolerance in 6 years


## Panel: Australia’s strengths in quantum sensing> Andre Luiten, Managing Director, QuantX Pty Ltd;

Silvana Palacios, Lead Quantum Physicist, Nomad Atomics;
Jim Rabeau, Director, Quantum Technologies, CSIRO (Panel Chair)- we can cook quantum sensing croissants with 50% reliability. Next step is reliable mass production
- if you are able to speak the language that industry understands labs with find partners very easily
- why quantum sensors: what do we do if GPS goes down. We need a sovereign capability of telling time and location. $2B a day in Australia depends on knowing the time correctly. Sensitivity and accuracy.
- the issue is rejecting background noise rateher than finding the target. Quantum sensors give you an absolute result. It doesn't drift and doesn't need calibration


## Panel: Bridging the research to commercialisation gap> Clare Birch, Associate, Blackbird;
Lucas Hakewill, Accelerator Program Manager, UNSW Founders
Nat Puffer, Managing Director, IQT International;
Thomas Volz, Professor, Macquarie University and Strategic Partnerships Manager, Redback Systems;
Annie Parker, Executive Director, Tech Central, Greater Cities Commission (Panel Chair);
- Clair. Billion dlar fund. Blackbird ventures
- Founders 10x UNSW, Lucas hakewill
- what can the investment community do better.
