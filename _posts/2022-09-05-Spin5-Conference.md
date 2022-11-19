---
toc: true
layout: post
description: Semiconductor spin physics and quantum computing conference in Pontresina, Switzerland
categories: [notes, talks]
title: "Spin5 Conference"
---

> 20220905, Pontresina
Speakers: https://spinqubit5.nccr-spin.ch/speakers/program?

## Vandersypen - Spin qubits and simulators - more, better, easier

- 25 years ago was the proposition 
- why are spin qubits great?

### Vision of a semiconductor qubit processor
- local registers
- quantum links 
- integrated circuits
    - overcome the wiring bottleneck
- Linear six qubit array 

- visibility of 96%,  one qubit control at a time, decreases with simultaneous measurement
- spin resonance frequency shifts with microwave driving and with temperature, non-monotonous temperature dependence, \ 
    - should we operate at 200mK
        - no RF heating effects, and T2 barely reduced. 
- Cross talk during simultaneous driving of two qubits b EDSR
    - after you reach a certain rabi frequency you see a plateau - this is expected, as the maximum distance that an electron can move inside a dot is capped.
    - If you do two at the same time, the distance is also capped
- 2x2 Si/SiGe quantum dot array
    - multi-layer design
        - one electron regime reached
        - independent control tunnel coupling achieved

### Quantum links

#### Electron shuttling
- take an electron and move it across the chip in hope that the spin state will be preserved
    - Charge shuttling in a 4-dot array, arXiv 2209.000920
    - reliable charge transfer control pulses
        - estimated spin-flip probability per hop below 0.01% :shock:
    - Vande thinks that electron shuttling will be a very attractive approach
        - Boter PRA 2022

#### Superconducting resonators
- coupling distance spins through a superconducting resonator
    - try a dispersive regime.
        - spins are resonant with each other but detuned from the resonator
        - Upper branch isn't visible but expected as it is in a dark state
            Harvey Collard PRX 2022
- quantum simulation of Fermi Hubbard physics
- can get exciton physics in 4x ladder
    - exciton formation from long-range Coulomb interaction

> "Not only the pieces are coming together, but also the prospects of large-scale integration of qubits and electronics"


## Silvano De Franceschi - Long life to holes

- 100MHz you can drive holes
    - electrically addressable, but exposed to charge noise defects
    - However there are sweet spots = "a single hole spin with enhanced coherence in silicon"
- N.B. xxx see similar Coulomb peak breaks that one sees in phosphorous donors in the holes regime
- gyromagnetic factor characterisation
- Hahn echo coherence time - charge noise limited

### take-home message
- fast single-shot readout of single-hole spin in SiMOS
- sweet spots where hole spin is immune to  noise
- Echo coherence spin in...

- strong coupling between a photon and a hole spin in silicon (see Copenhagen conference a week ago)
    - take out the wafer before they get metal bond layers, cut it out and die
    - cover each dye with NiN (superconductor), the pattern the material with e-beam lithography
    - Resonator is probed by microwave transition line
    - create coupling with electric field in the device and electric field in the cavity 

- most structures can couple to spins in microwave cavity
- unprecedented spin-photon coupling
- Prospects: high fidelity, two-qubit gates mediate
- To improve:
    - interface oxides as usual

## Dominik Zumbuhl - Hot Hole spin qubits in Ge/Si nanowires
> Holes could have a great future
- Will show you a bit about FiFETs as well
- Switzerland has a quantum computing programme, remember: NCCR Spin - to develop fast, compact and scalable electron and hole spin qubits

- Angular momentum L = 1, get heavy holes and light holes
- Spin-orbit interaction: Hso L, fast all electrical qubits, price charge noise coupling
- no contact hyperfine interaction -> longer coherence times

- Holes in 1D -> direct Rashba spin-orbit interaction // strong transverse confinement, heavy hole light hole mixing, happens strongly in quasi dimensional 1D geometry
- Strong spin-orbit interaction -> very fast qubits
- g-factor can be modulated strongly with gate voltages
- direct Rashba is also highly non-monotonic

### finfets
- tip is just a few nanometers is curvature
- the aspect ratio is relatively small to get good control of the electric field
- rely on self-aligned gates to fill the gap - filling the gaps between the lead gates and the centre gate. Industry technique. 
- Produced via IBM
- Rabi oscillations : 100MHz, Q factor of 100
- operable of 5K, readout actually ends up being the limiting factor via Pauli spin blockade (limited by temperature)
    - at higher T reservoir exchange can destroy readout
- Anisotropy of G-factor is strong
- First CROT for hole spins in silicon, see Kuhlman's talk tomorrow and posters from Geyer and Eggli

### sensing
- trying to use strontium titanate varactors for readout
    - don't freeze out at low T
    - Don't have a B-field dependence


### nanowires
- due to the band alignment there is a hole gas that populated the environment for free. Just like si FinFETs, there is no doping
- spin mixing transitions in spin blockade
- strong spin-orbit coupling ISO ~65nm
- all electrical spin manipulation
    - EDSRR, 
    - spin-orbit coupling is so strong that when you pulse into Coulomb blockade you completely go off-resonance and then you won't see Rabi oscillations
        - Rabi oscillations can be made extremely fast, 1ns for spin flips
- Can convert Rabi frequencies to the spin-orbit coupling length
    - on the order of 4nm, in InGaAs, they are an order of magnitude longer
        - spin-orbit length can also be tuned up to 24nm
    - the size of the dot/wavefunction is larger than the spin or bit length, 
- Unfortunately, T2 star time is really short, 10ns
    - there is a factor of charge noise, which should be able to echo away
- G-factor can change by 1.5x and Rabi frequency can change by a factor of 7x. due to gate voltage control
- can create a spin-orbit switch
- tunable g-factor is useful for coupling to a resonator, you can couple a hole spin to a microwave photon in the same way we do EDSR
- why is T2 star so slow?
    - oxide annealing improves capacitance robustness
    - But when they made a qubit with them the T2 star didn't change unfortunately even though bias triangles and pinch-off curves look cleaner after annealing
- The issue could be the oxide on the shell of the wires, remember this oxide layer is only 2nm away from the wavefunction of the Germanium in the shell of the wires. 
- my work was on the last slide, look mom I'm famous :fire:

## David Awschalom - Silicon carbide
> My students do all the work, not me. They use me as an ATM at this point. :rofl:

- really similar to NV centres in diamond
- vastly common electronics material, typically used in telecommunications and 5G applications
- Di-vacancies missing both silicon and carbon can be in four different orientations
- how could you have such long coherence times in a very dirty material that hasn't been engineered very cleanly

- explore lattice symmetries for quantum dynamics
    - excited state orbitals exhibit stronger coupling to phonic and electric fields
- Landau Zener Stuckelberg interference is strong without a cavity present
- With this kind of tuning you have 40,000 linewidths of single photon tuning to chuck down a communications channel.
- Creating a decoherence-protected space with microwave dressing.
- strongly coupled 29Si single nuclear Rabi oscillation, rely on nuclear spin as long-lived quantum registers
- Map the spin onto the charge, charge lifetime is on the order of 10s. (Elena glen Science Advances eabm5912 2022)
    - Only one state will be bright and one state will be dark.
    - look at the photon emission of a state from its charge dynamics\
    - end to end fidelity is low (80%) but the physics works well
- Using isotopically purified materials and specific pulsing we can put the lifetime up to 5s
    - T1 is a minute and a half, N-doped sample so can be cleaner. DFT says that these can go up to 10 minutes
- emerging magnetic quantum states and memories (telecom)
    - dope with vanadium, they emit light but they obey telecom optical fibre networks
    - luminesce line shape can be deconvolved to pick out all the isotopes of silicon. 20Ghx shifts per neutron in the curve

#### questions
- charge defects in silicon carbide are incredibly stable   
    - could be a surface stoichiometry thing
- NV centre non-radiative decay in phonon band
    -phonon relaxation processes are faster than diamond but slower than diamond
    - readout times are on the order of 1ms, can speed up, mainly a financial issue
- Use the starkshift as wavelength transduction 
    - yes we can make all of this electronic
- How does entanglement work?
    - the process works both ways
    - want to entangle to 100km for sensing applications

## Ferdinanc Kuemmeth - Spin rotations via real-time estimation of qubits parameters in GaAS
- work on GaAs, GeSi, SiGe, SiMOS, superconducting, plus auto-tuning

- measure simultaneously current through all 24 channels o create a leakage matrix
- characterisation of device quality (noise)
- Characterisation of device quality (homogeneity)
- sparse acquisition by time-stamping hardware triggers
    - adaptive line searches by active-learning algorithms
        - timestamps also find corners of the shape, this is so they don't miss out minature boundaries where corners might meet each other the
- estimation of the Overhauser gradient
    - FPGA - Bayesian estimation of uncontrolled Overhauser gradient
        - Fabrizio Berritta, and Fabio Ansaloni
        - Shulman, Harvey Nicol, Suppressing qubit dephasig using real-time Hamiltonia estiamtion 2014, nature comms. 
    - B using the overhauser gradient you ran use to do control spin rotations,
    - while the overhauser gradient evolves
    - can also do Ramsey based on Bayesian estimation

### questions
- Tunnel couplings and tuning
- feedback based on estimation, have you optimised the times at which you probe
    - we are not intentionally nuclear spins unlike the paper in 2014
    - we are letting them evolve in an uncontrolled fashion, and let's learn it and use it
    - Equidistant probes, more or less the same algorithm in Jacobi's group 
- Autotuning: regimes where you have...
    - you want to execute these ramps very quickly, if your tunnel rate is low you may not record a timestamps
    - If there is Pauli blockade, you run into the issue that your relaxation time is longer than your ramp speed 
    - although once it's tuned up there is/isn't a lot of fine-tuning to be done depending on your needs

## Peter Stano - A hole spin qubit
- we describe spin qubits using simplified models, expanding its kinetic energy in powers of crystal momentum
- good way to simplify: many-body
- the lowest non-trivial order in zinc-blende gives Rashba and Dresselhaus spin-orbit fields in the conduction band
- why are these terms large is the perturbation theory wrong?
- do you claim that all previous results are wrong?
    - No the difference ranges from small to large depending on parameters
        - there positions where the change is small and the previous models/results are not wrong

Full github directory of spin qubit data errors, tractable history for the database, the instructions for altering me on errors, you are welcome to give suggestions for improvements
You can access the database through an interactive interface in mathematica
 can be exported to latex
https://github.com/PeterStano/ReviewOfSpinQubits

## Vitaly Golovach - 
- what makes a good qubit
    - a combination for a very quantum system 2Ls with several very classical systems (gate, readout)
    - Our goal is: Coexistance of a very quantum system and a very classical system on the **same scale**

## Andreas Fuhrer - Towards scalable quantum computing with holes in silicon

- resource estimate of Shor's algorithm 0.1% error per gate 10^8
- wouldn't it be nice to have a chip that fits on a chip 
- hole qubits are 10,000 smaller than transmons
    - ideal two-level systems, no frequency crowding
    - dense lattices
    - harder to fab, will try and leverage CMOS technology
    - holes have no valley degeneracy
    - can be controlled fast and electrically using SOI

## Lukasz Cywinski - theory of spin qubit shuttling: si vs GaAs and chain of tunnel coupled dots vs a travelling dot
> Can one make an electron in Si travel 10um with small coherence loss?


## Michelle Simmons
> There's plenty of room at the bottom

- Imaging a single phosphorus dopant in silicon at low temperature
    - The ability to measure the wave function directly
    - Exact pinpointing of phosphorus atom lattice position with atomic precision

- Ultra-low noise quantum circuitry of tiny wires in silicon    
    - can make the wire down to 4nm wide,
    - As you make the wire more narrow you force the transport to hop on off of the donor islands
    - wider and it follows typical current 
    - why is it when you take mono-doped wires are is the noise so low
        - epitaxial structure is providing the low-noise environment

- impact of charge noise on exchange interactions - simmons
    - consider the distribution of charge noise as Gaussian
        - The exchange becomes skewed in frequency, in these systems we have to take into account the distribution 

- The quantum nature of 7 atom circuits
    - High fidelity single-shot spin readout classic elzermanA

- Advances: high fidelity readout
    - 99.6%, tunnel rate impacts the fidelity we gate,
        - adjust the donor number, electron number to tune the tunnel rate and thus the fidelity
    - Have spent a considerable amount of time to tune the SET to have high on/off ratio
    - single donor based sensors can readout 15 qubits
    - D Keith, New journal of physics 21, 063011 (2021)
    - Review of Elzerman style readout:
        - want to minimise spin-down tunnel rates
        - high mag field or low electron temperatures on the SETs
            - want a readout energy to where the Seeman energy is on the order of the thermal broadening
    - Have moved to a ramped readout rate
        - want to readout at different points in detuning to pick up the spin at more points
        - also picking up how the tunnel rates change over the course of readout
        - More time is spent in the lower rate regime rather than the high rate regime
        - can easily get above 99% fidelity
            - can go to half the magnetic field value and a different temperature

- analogue quantum simulator 
    - can put phosphorous atoms very close together, go back to Feynman
    - quantum sim of polyacetylene
    - precision engineering at aub nm scale
    - only needed six gates to do this

Comments: Absolute fire Michelle :fire:

## Menno Veldhorst - Quantum computation and simulation with holes in Germanium
- low effective mass, simplifies the fabrication
- absence of valley degeneracy states
- nuclear spin-free isotopes

- natural germanium can get amazing single-qubit readout
- transversal hyperfine interaction
- Sweet spots do they exist? - they shift to impractical fields when including multiple excited states
    - g-factor strongly anisotropic, change with inplane and out-of-plane electric field, no sweet spot but the slope is opposite, so there may exist an angle where they cancel each other out to fix the g-factor

- Phase-flip code: several one and two qubits gates
- Toffoli gate to correct
- can we electrically control quantum dot uniformity
    - minimal dot-to-dot variations are critical for true scalability 
    - charge hysteresis is often seen as a bug, but it is very reproducible and stable in time, oppopportunity to exploit
- Tuning a 4x4 array in prep
    - shared control, more parameters to tune than activate lines, hard but scalable -> rents rule
    - how do you identify 16 quantum dots and tune the array, even though you can make a quantum dot array
    - control tunnel coupling?
        - tunnel coupling only when both gates are on, 
        - reasonable agreement in the array 

## Maud Vinet - Increasing maturing of silicon spin qubits leveraging industrial methods
- The competition are moving ahead, and we have to catchup 
- what do we need to make millions of qubits and quickly as the competition isn't waiting for us
- incubation time
    - strained silicon 1992 -> 2003
    - HKMG 1996 - 2007
    - Raised S/D 1993 - 2009
    - the incubation time is typically 12 - 15 years
- Technology
    - off the shelf and slightly modify it, why because there are so many choices
        - what material in the gate channel, holes or electrons... how clean does it need to be, the layout, dot to dot distance.
    - Little deviation from FDSOI
        - added a module called a Qtrench,
        - TiN gate stack
    - FDSOI back gate to move the quantum dots away from the interface

- Statistical test and characterisation
- Probe dot shape and position

- there isn't a fab to create this het. layer on a large scale
- two: you can incorporate a back gate in your native silicon to pull the dot away from the interface and then you also have extra electrical control in one

## Andreas Kuhlman - FinFET quantum dot devices
- built their own custom cryogenic probe station, can fit inside a VTI
    - adding a magnetic field
    - adding RF probes as well. 

## Natalia Ares - real time tuning and characterisation of quantum devices using machine learning
- from quantum chip to qubit, rely on automation to do this

## Audrey Cottet - Quantum information with hybrid nanocircuits
> wit Kontos

- spin qubits with ferromagnetic elements
- hybrid light atter networks of Majorana nodes

### Coupling one individual spin to cavity photons
- synthetic spin-orbit interaction generated by non-collinear ferromagnets
- spin valve behaviour in a qdot with ferromagnetic contacts
- reaching the strong spin/photon coupling with carbon nanotubes
    - Potential limit due to C13 contamination leading to charge noise
    - 

#### conclusions
- theory suggests strong Zeeman fields
- dependent on the dot size (more theory to be done)

### Majorana based topological quantum computation
- You need a physical network in which you can move the Majorana modes - difficult to achieve experimentally
    - Is it possible to get rid of physical networks
    - can we get Majorana modes inside a microwave cavity?
- Direct coupling between Majorana modes and cavity potential?
    - cavity field equivalent to a cavity photonic potential

- universal set of gates for quantum computation (also T gate)
- Compatible with many experimental platforms
- Relatively insensitive to system details
- Controlled back action of the Cavity

## Andrew Dzurak 

- advantage of CMOS manufacturing isn't coherence but is the reproducibility to get qubits at scale

### SiMOS qubits key demonstrations
- multi-electron high-fidelity qubit operation
    - when we operate in single valence states we get standard spin one-half qubits 
    - can get extra screening from those extra electrons
        - less prone to local disorder than in the single electron regime
        - having more electrons smooths the local potential

### All electrical control of electron spin qubits
- On-demand electric control of spin qubits
    - shows that you can do reasonable electrical control of electrons similar to holes
    - by deforming the potential you can bring down orbit states allowing you to access electrical control where you wouldn't previously
        - therefore micromagnets aren't required
- Pulsed electron spin orbit spectroscopy: arXiv 2201.06679

### Charge Noise & 2-qubit fidelities
- Charge noise in Pd/ALD Gate stacks & return to Al
    - have struggled to find magic recipe so have moved back to Al gates
- Two qubit fidelities used to saturate around 97%
    - major change has been to employ fast feedback mechanisms using Quantum machines box
        - for each single shot you are checking that you have correct initialisation state as well as make sure that the SET is still reasonably tuned.

### Managing qubit variability
- SMART global control protocol - sinusoidally modulated always rotating 
    - how can you cope with all the different g-factors in your device
    - Used TEM imaging and tight-binding model to map out the spreads in g-factor. Seems to be that the surface roughness is the main source of g-factor variability.

Comment: Andrew shills his students hard. Much respect to supporting the mandem. buidl with the community


## Mark Erikson

- nice slide on the comparison between the different semiconductor stacks

- you really want large valley splitting
- would be nice if you could tune the nice valley splitting
- tensile strain at the interface lifts 4 of the valley states 
- what can be done to the heterostructure to increase the valley splitting?

- change the interface - add more Ge
    - the disorder isn't affected by the amount of Ge
    - can increase it by applying an electric field but not increasing the barrier
- add Ge inside the well
    - get two interfaces
        - get valley splitting contribution from each of the interfaces
        - two interfaces -> twice the valley splitting
- Wiggle Well
    - couple the two valleys together by some perturbation
    - wavelength for the oscillating Ge concentration is 0.32nm
    - couple to a valley in the neighbouring Brillouin zone, rather than the 1st one (turn around)
        - need 1.7nm of oscillating Ge structure in the well
            - have been able to grow this
- valley splitting and orbital splitting can be extracted from pulsed-gate spectroscopy: both can be tuned in situ by moving the dot around
    - changing the size of the dot doesn't really have much of an affect, unless you actually change the center of mass of the dot

- illumination of quantum dot devices allow you to reset the threshold voltages. Paper coming soon.
    - the dependent is very linear. 
- Wisconsin Quantum Institute, QNEXT, NSF, funded by the Army research office. :eyes:

## David DiVincenzo - superconducting qubits
- transmon platform for quantum computing challenged by chaotic fluctuations
    - not such a good method for quantum computing, problems for scaling due to their many-body physics
- Many body localisation phase is a good substrate for quantum computing

## Dimitrie Culcer

### Hole spin qubits
- great cafe called the sweet spot
- Optimal operation poitns for ultrafast highly coherent Ge hole spin-orbit qubits
- Compare our effective Hamiltonian with numerical diagonalisaiton
    - different out of place confinement and different in plane confinement
- qubit lives in the heavy hole subspace
- 

### question
- do you have a way to extract the heavy hole light hole mixing?
    - it is the effective spin orbit that you get in the 2d, maybe you can look at the zeeman splitting
    - you will have to look on a case by case basis     

- is there a chance that spin orbit plays a role on alongside the EDSR/hyperfine driving
    - spin orbit would be naturally included
    - what we have done does match well with the numerics
    - hand wavy

## Klaus Ensslin - Quantum devices in graphene
- GaAs is the best, Si is the workhorse, graphene is the future
- Graphene has no bandgap, linear dispersion unlike Si and GaAs. Can't just switch it off.
    - carbon based
        - 99% spin free without doing anything
        - lightest group 4 element,
            - very weak spin-orbit interaction
        - doesn't work with single-layer graphene
            - need a gap

    - by making a bilayer graphene you make a parabolic dispersion, no gap. apply an electric field and you get a mexican hat dispersion -> gap

### sample design
- lab tech
- piece of graphite, hBn, bilayer of graphene, hBn, then insulator and gates (Cr/Au)
- can achieve resistances beyond giga Ohms
-  can push to split gates
- channel conductance levels split by factor 4e^2/h. 2x from valley degen, 2x from spin degen

### quantum dot
- confined by pn junctions. p type leads, n type dot. Can be reversed as well.
- dirac cones aren't round, they are often warped at higher energies, which are brought down and are accesible when you apply an electric field
- tunnel barriers aren't opaque enough in graphene, so you need the magnetic field
    - need to tune the tunnel barriers alongside tuning the magnetic field -> nightmare to do manually.
- Pauli spin blockade
    - life is a little complicated
        - the ground state is always a spin triplet
        - the total wave function is anti symmetric. 
        - 3-particle state 
    - you can have spin blockade, you can have valley blockade

## Graphene dreams
- josephson junctions, quantum dots, topology built in, valleys are built in and you might as well use them
- spin-orbit interaction which you can bring in by adding in a transition metal to be able to tune the spin-orbit interaction


## Leo Kouwenhoven - quantum dots coupled to superconductors
- use cQED as just a very fast way to measure the super-current
- o

## Seigo Tarucha

- Useful QEC may need 1000 qubits 
-

### noise correlation between two qubits
- assume two qubits are both subject to nuclear spins and charge noise to two-level fluctuations
- freq of qubit L depends on state of qubit R and vice versa
- the qubits are strongly correlated and increases at higher frequencies.
- will be important in multi-qubit entanglement and quantum error correction performance

## Giorgos Katsaros - Importance of g-factor differences for hole spin qubits in planar Ge devices

### Holes
- spin is locked with the direction of motion, Holes in Germanium
- HH and LH splitting depends on how confined your splitting is
- HH spin qubit is a Kramers doublet, the wavefunction is a superposition of the spin-up an dspin-down states entangled with the orbital degrees of freedom
    - will need to place your magnetic in plane to make a qubit

### Germanium
- HH means the Jz = 3/2 HH doesn't refer to the mass. 
- large g-factors which are electrically tunable
- 1M hole mobility achieved 
- Rabi has exceeded 400 MHz
- decent spin manipulation times
- fab is difficult especially in 1D structures, need to move to planar germanium
- Giorgos uses depletion mode qubits
    - quantum well buried 20nm below the surface
- coherent rotations already at 300uT, g-factor difference of 4

### granular aluminium
- Superconductivity in granular al 1967, high critical magnetic fields and very high normal resistivity

### Outlook
- use JPA from superconducting circuits. create a JPA on al indium arsenide. Achieve a gain of 20dB and tunability of 2GHz
- deposit cold 
- make germanium great again

## Tristan Meunier - Coherent electron spin displacement
- long-range coupling

## Susan Coppersmith - Si/SiGe heterostructure

## Alex Hamilton - semiconductor holes - more spin for your buck
- no nuclear spin problems, fast all electrical control, sweet spots for fast spin control and reduced decoherence. Challenges: materials issues.
- holes aren't just positively charged electronsA
- uniaxial strain strongly affects LH-HH splitting. The splitting of LH and HH greatly affects qubit and quantum dot properties, comment: yay materials science 

### summary
- spin states of a single hole in a planar Si MOS quantum dot
- 3D g-tensor and strain effects
- CMOS hole qubit and electron charge sensor
- Future: measurement optimisation coherent control of single holes, Ge holes, charge noise

## Giordano Scappucci - materials and interfaces on and off the beaten path
- Development cycle for spin-qubit materials
    - quantum devices as statistical local probes of qubit environment

### optimising the Si/sige het
- reducing charge noise in Si: no caps and thin wells
    - no cap: Si-rich passivation instead of non-uniform epitaxial growth -> improve semi-dielectric interface
    - thinner quantum well
        - lattice-mismatched, misfit dislocations suppressed and hence background scattering reduced. 
- scattering in 2DEGs and charge noise in dots are related
- superconductivity in low-disorder Ge/SiGe
    - Ge-silicidation for superconducting PtGeSi
## Andrea Morello

Impurity spins hold record coherence times in each category where data for them exist

### Coupling mechanisms for donor spin qubits
- sub 10 nm --> share wave fucntion
- 20-20nm - exchange interaction
- 100nm electric dipole, 
- long-range: electron shuttling

- two qubit operations: aharonov-Anandan geometric phase: classical case, transport on a sphere, think hands
- two-qubit gate set tomography
- 3-qubit nuclear spin electron gate
    - pi on 2 pulse on one of the nuclei, 

#### Exchange interaction
- ESR spectrum in the presence of J
- actual fidelities are around 80%
    - the main difference is that we have entanglement
    - Bell state 92% Fidelity, two-qubit fidelities are in the 99% ball park, so why 80% so low in GST
    - Bell state coherence times, there is a beating. Two frequencies that the system hops between.
        - Si 29 or a charge trap, not sure what it is

#### Long range - electric dipole interaction
- encode quantum information in the nuclear spin and the electron spin flip-flop state
    - you can't do magnetic resonance between those states
    - Hyperfine interaction appears as a sigma-x term

- make on-chip ion detectors
    - 99.85% confidence of detecting a single atom
    - enables step and repeat donor arrays

#### scaling up inwards - high spin donors
- larger than one-half spin leads to electric quadrapole moment
    - get full magnetic control and full electrical control
    -
- electrical noise effect on nuclear dephasing (throwing the baby with the bath water?)
    - 1/2 projection is insensitive to electric field
        - also has a longer T2* by 30%
    - electrical noise is a weak effect
- lab temperature fluctuations in voltage sources
- error-co

### Question
- there is some sensitivity to the magnetic field to the crystal axis, will affect T1 a little bit.
- strain inhomogeneities, the splitting on the Sb NMR spectrum is due to the local strain, we basically have  local strain sensor in the device of a bandwidth of 2Hz


## Guido Burkard - Finger prints qubits noise in cavity qed

- two-qubit gates between spin qubits AC/DC
- DC control: CPHASE (CZ) gate
- high fidelity AC gates: synchronization
    - simultaneously control qubit on and off-resonant control off-rotation target

- Qubit noise
    - limiting gate fidelities and qubit coherence
    - dephasing longitudinal noise often most dangerous
    - needs characterisation
        - plus needs to be efficient and applicable in arrays
            - try circuit QED
- characterisation tech:
    - flank method:
        - run a current through the quantum dot, sit on the flank on the peak of Coulomb blockade and measure the shift
            - probes the voltage fluctuations in the circuit rather than the qubit fluctuation
- dynamical decoupling
- cavity QED, with general qubit, measure the cavity transmission
- Objective: qubit coupled to a cavity, longitudinal noise, coupled to our qubit via a parameter known as the noise sensitivity. Can assume Gaussian noise
    - can you correlate the noise to the cavity transmission
- describe the system using quantum Langevin equations
    - take into account cavity decay and qubit decay rates
- Transient Cavity transmission:
    - no variance in lowest order
    - averaged cavity transmission
    - long-time cavity transmission 
    - transient without the qubit
- this is only for the linear effect in the transient situation
- quadratic coupling in qubit and cavityA
- Semiconductor spin qubits arXiv 2112.08863

## Andreas Wallraff - repeated quantum error correction in surface code
- final fidelity of the final state of the google computer was 10-3, so way less than 1
    - gonna need error correction for sure
- Challenges in quantum error correction
    - bit flips and phase flips
    - measurements collapse your qubit state
        - store logical qubits in a system of many physical qubits
        - make use of symmetry properties (parity) of logical qubit states
            - revealing errors
            - but not the encoded quantum state
- why surface code
    - can realise it in a planar geometry, probably will be used in semiconductor qubits as well
    - has the largest error threshold, 1%
        - every individual operation has to have physical errors less than 1%
        - assuming that your physical error doesn't increase as you increase the size of your chip - Requirements
    - high-fidelity entangling gates between data and ancilla qubits
    - fast high-fid measurements of the ancilla qubits
    - Low readout cross-talk between ancilla and data qubits
    - Ability to do repeated gates and mid-cycle measurements

- what do we measure
    - Initialize, perform n wec cycles, read out all data qubits in z-basis, determine logical operator for each  run with up to n repeated cycles, apply correction conditioned on decoded syndromes for each run,
- Outcomes of logical z and logical x
    - exponential decay of logical expectation values
    - logical lifetime
    - logical coherence time 
- then you can calculate the logical error per cycle: seems to come out with a performance of 3% error rate
    - decent but not perfect,
    - for a real qc you want E-8 % error 
    - use simulations to project performance with physical error rates reduced by factor x
        - break-even within reach
        - we are within a factor of 2 away from the threshold

#### summary
- fast qec cycle of 1.1 us

### questions
- is it as simple as give us more money and it will work?
    - if you can modules that you are below the error threshold per module and that you can guarantee performance then you can say that you have done it 
    - it isn't just engineering now, there is still space for new ideas

## Pasquale Scarlino - superconducting and semi-conducting, hybrid quantum circuits
> In situ tuning of the electric dipole strength of a double dot  charge qubit: charge noise protection and ultra-strong coupling 

### background
- versatile platforms: quantum information, optics and simulation
- barely reached the strong coupling regime until fairly recently
- Strong coupling regime achieved later in 2017, same happened in the spin degree of freedom in 2018

- make use of high impedance technolgy
    - can use josephson junction array
        - high impedance circuit elements
        - lossless josephson inductance can be very high
    - NbN disordered thin films
        - play with the kinetic energy of cooper pairs to play with the resonance
- High impedance SQUID array resonator
    - 100x smaller than the current competition
    - 

- Frequency tunability of the squid array resonator


