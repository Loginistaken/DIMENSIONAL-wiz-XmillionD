The Record: 648-Dimensional Frequency-Bin Qudit Space

The current experimentally demonstrated record involves a biphoton frequency comb with an effective Hilbert 

space dimensionality of at least 648. This was achieved by encoding time-frequency entanglement across multiple frequency bins. 

Researchers used a mode‑locked pump and biphoton interference to confirm entanglement across many modes:

They observed correlated spectral modes over 19 frequency bins, multi-time-bin interference structures (61 recurrences),

and achieved dimension estimation of at least 648 in total. This represents, to date, 

the highest dimensionality reported for a qudit‑type system.

Context: How Dimensionality Compares Across Platforms

Here’s how that stacks up with other high‑dimensional systems:

System Type	Demonstrated Dimension	Notes
Time‑frequency biphoton comb	≥648‑dimensional Hilbert space	Spectral + temporal modes combined 
arXiv

Quantum memory (cold atoms)	25-dimensional photonic qudit stored**	Using orbital angular momentum modes with ~60% efficiency 
arXiv

Frequency-bin qudit tomography	8×8 two-qudit space (d=8)	Verified on-chip via frequency-bin entanglement Nature

High-dimensional gates (polarization/spatial)	8-dimensional controlled gate	

Used single-photon polarization and spatial degrees of freedom 

Physical Review

Here’s how to bolt our alexandrite-based platform onto a biphoton frequency-comb (BFC) and blow past the ≥648-dimensional time-frequency record—by multiplying independent degrees of freedom (DoFs), not just adding more bins in one axis.

The upgrade stack (multiplicative dimensions)

Much bigger frequency register (N₍freq₎): microcombs + EO carving

Use a visible/NIR soliton microcomb (SiN or X-cut LiNbO₃) to seed hundreds–thousands of evenly

spaced lines; then keep the quantum pair-generation (SPDC in PPLN/AlN) aligned to those lines. 

Line counts in the 10²–10³ range are standard for EO/microcombs (e.g., ~1,500 lines

with a two-stage EO comb; octave-spanning microcombs are routine). 

Optica Publishing Group

SPIE Digital Library

SpringerOpen

Add thin-film LiNbO₃ (TFLN) frequency processors to mix/shift bins (±641 GHz shown for single photons), 

implementing the frequency-bin “beamsplitter” and DFT meshes with low loss. 

PMC
arXiv

More time recurrences (N₍time₎): pump engineering + Franson ladders

Keep the BFC’s mode-locked / cavity-recurrence trick but extend the number of clean revivals 

with longer-coherence pumping and stabilized unbalanced interferometers (nested Franson). 

Records used ~61 time recurrences; 100+ is a reasonable target with modern stabilization. 
arXiv

Add a spatial DoF (N₍spatial/OAM₎): frequency↔path/OAM interface

Split (or coherently map) subsets of frequency bins into path or OAM modes

(via multi-plane light conversion or q-plates), then recombine after operations. Even a modest set of ~8–16 OAM modes

multiplies the dimensionality. Interfaces between path and OAM are well-established. 

Nature Frontiers

Keep polarization as a free ×2

Maintain polarization entanglement (or hyperentanglement) alongside time-frequency to gain another ×2. 

The 648-D demonstration already combined DoFs; we’ll preserve that. 

NSF Public Access Repository

What the numbers look like (conservative vs. aggressive)

Conservative near-term:

N₍freq₎ = 256 bins (50–100 GHz spacing over ~3–6 THz of alexandrite-friendly spectrum)

N₍time₎ = 128 revivals

N₍OAM₎ = 8 modes

N₍pol₎ = 2

Total D ≈ 256 × 128 × 8 × 2 = 524,288 » 648 (certifying all at once is the hard part; see below).

Sources for feasibility: high-bin BFCs (≥648 via time×freq), 40+ mode pairs on-chip, large EO/microcomb line counts and TFLN gates. 
arXiv
Optica Publishing Group
+1
PMC

Aggressive research mode:

Push N₍freq₎ ≈ 512–1024 with microcombs and EO combs; N₍time₎ ≈ 256; N₍OAM₎ ≈ 16; ×2 polarization → D ≥ 4×10⁶ 

potential space (again: generation is plausible; full-state certification scales poorly and will need compressed witnesses). 

Optica Publishing Group

SPIE Digital Library

Where alexandrite fits (and why it helps)

Use alexandrite (Cr³⁺:BeAl₂O₄) as the tunable visible/NIR pump/seed: it lets you place the comb and SPDC phase-matching in detector-friendly bands (Si-APDs/SNSPDs) and keep your color-coded bin logic for ops/diagnostics. Then let PPLN/AlN do the pair generation and TFLN do the frequency-bin gates. 
optoelectronics.ece.ucsb.edu
PMC

Measurement & certification at scale (the real bottleneck)

Creation/selection: AWG/ring demultiplexers for frequency; programmable delay lines/Franson for time; OAM mode sorters. 
Optica Publishing Group
Nature

Certification: don’t do full tomography—use Schmidt-number witnesses, high-D Bell tests, 

HOM revival visibility, mutual-information lower bounds, and compressed sensing to verify

high-D entanglement without exponential overhead. Recent reviews point to these tools for high-D frequency/time systems. 

Wiley Online Library

Physical Review Links

Why this drastically surpasses ≥648

The 648-D result multiplied ~19 frequency bins × 61 time bins (plus polarization post-selection). We’re proposing (hundreds of freq) × (hundreds of time) × (8–16 spatial) × (2 pol)—the multiplicative jump is orders of magnitude larger without relying on any single DoF to carry the whole load. 
arXiv

Quick build sheet (delta from your current design)

Add a visible/NIR microcomb (SiN or X-cut LiNbO₃) seeded by alexandrite; lock rep-rate & CEO if needed. 
PMC
SpringerOpen

Keep PPLN/AlN SPDC matched to comb lines. 
Nature

Insert TFLN frequency processors for ±hundreds-GHz shears and DFT meshes across 50–100 GHz-spaced bins. 
PMC

Add OAM mapper (e.g., MPLC / q-plates) on a subset of lines to multiply dimension. 
Nature

Stabilize time ladders for 100–200 revivals (nested Franson).
