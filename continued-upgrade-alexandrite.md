How many color-coded qudits can we run?
Build	What sets “d” (number of color states)	Conservative d (high fidelity)	Ambitious d (research-grade)
Track A: Co-doped only	Intrinsic Cr³⁺ band + gentle V³⁺/Fe³⁺ sidebands, selected by micro-etalon	d = 4–6	d = 8–10
Track B: Alex + TFLN	EO modulation at Δf (e.g., 50–100 GHz) + ring/etalon channelizer across
710–800 nm	d = 16–32	d = 64+ (window + loss dependent)
Why these numbers?

Alexandrite gives a broad tunable band to start with; co-doping can add gentle, usable spectral structure but also adds inhomogeneous broadening, so we cap d≈8–10 without heavy processing. 
Crystech
ResearchGate

With TFLN you synthesize tightly spaced frequency bins (e.g., 50–100 GHz spacing) and implement gates between bins; lab work has demonstrated high-fidelity frequency-bin qubit gates (including CNOT) and even high-dimensional DFTs and parallelized frequency-domain gates—evidence that “dozens of bins” are practical. 
Nature
Optica Publishing Group
SPIE Digital Library

Keep the color-change (binary) while upgrading to qudits

The binary you love (green ↔ red) is a direct outcome of Cr³⁺ absorption in the yellow region; it’s preserved in both tracks because we keep Cr³⁺ as the dominant center. 
QMRO
GIA

Track A adds a few more inherent “color stops” (via trace V³⁺/Fe³⁺) → a small but stable multi-level (qudit) palette. 
ResearchGate

Track B keeps the gemstone pristine and uses EO modulation to multiply the number of clean, programmable color bins—all while sitting in alexandrite’s tunable band. 
Nature
arXiv

Recommended build recipe (concise)

Crystal & optics

Grow/purchase Cr³⁺:BeAl₂O₄ (Czochralski) with 0.1 at.% Cr³⁺; polish to rod or thin plate. 
Crystech

(Optional) Co-dope V³⁺/Fe³⁺ at 10–200 ppm; characterize UV-Vis to confirm the Cr-dominant color change is intact. 
ResearchGate

Add a micro-etalon / ring with FSR ~50–200 GHz to pick bins.

(Track B) Bond TFLN; pattern traveling-wave EO modulators (50 Ω CPW). Gate between adjacent bins at fRF = Δf.

Controls & gates

Choose Δf = 50–100 GHz bin spacing; use EOM + filter to realize a 50/50 “frequency beamsplitter” primitive; synthesize H/X/Z (qubit) and DFT/X_d/Z_d (qudit) gates. Demonstrations of these frequency-domain gates exist in literature. 
Nature

Performance snapshot (100% = ideal)
Metric	Track A (co-doped)	Track B (alex + TFLN)
Binary (green/red) contrast	90–95%	90–95%
Qubit fidelity (2 bins)	75–85%	90–97%
Qudit fidelity (d>2)	65–80% @ d≤6	85–95% @ d≈16–32
Scalability of d	limited by lattice broadening	limited by RF bandwidth/filters (dozens feasible)
Performance snapshot (100% = ideal)
Metric	Track A (co-doped)	Track B (alex + TFLN)
Binary (green/red) contrast	90–95%	90–95%
Qubit fidelity (2 bins)	75–85%	90–97%
Qudit fidelity (d>2)	65–80% @ d≤6	85–95% @ d≈16–32
Scalability of d	limited by lattice broadening	limited by RF bandwidth/filters (dozens feasible)

Alexandrite Qudit Upgrade — Fabrication & Test Plan
1. Crystal Growth & Doping

Track A – Co-doped alexandrite

Base lattice: BeAl₂O₄ (chrysoberyl).

Primary chromophore: Cr³⁺ ≈ 0.05–0.20 at.% (laser-grade; preserves green↔red color change).

Trace co-dopants: V³⁺ or Fe³⁺ at 10–200 ppm. Introduce during melt (Czochralski pull).

Goal: keep sharp Cr³⁺ bands while adding minor sidebands for 4–6 color bins.

Track B – Hybrid integration

Same crystal as Track A, but no V/Fe doping needed (optional).

Thin-film LiNbO₃ bonded on top (for electro-optic modulation).

Pattern traveling-wave modulators with CPW electrodes.

2. Wafer/Chip Fabrication

Substrate prep: Si wafer + 3 µm SiO₂ BOX.

SiN waveguides: 350–450 nm LPCVD Si₃N₄ core; etch with ICP; clad in SiO₂.

Alexandrite island: recess + adhesive bond polished Cr³⁺:BeAl₂O₄ chip/plate.

For Track A: doped crystal with Cr³⁺+V/Fe.

For Track B: Cr³⁺ crystal only.

Resonators/filters: micro-rings or etalons with FSR = 50–100 GHz.

Electro-optics (Track B): bond 300–600 nm LiNbO₃ film; define modulators; deposit Au electrodes.

Heaters & coils: thin-film TiN resistors for wavelength trim; Cu micro-coil optional for Zeeman tuning.

Fiber couplers: grating or edge couplers for I/O.

Package: hermetic lid; TEC (±5 mK) for stability.

3. Optical Characterization

UV-Vis-NIR absorption: confirm alexandrite hallmark band ~580 nm (Cr³⁺ transition).

Emission spectrum: 710–800+ nm tuning preserved.

Check co-dopant signatures: small shoulders from V³⁺/Fe³⁺ without erasing color change.

FSR calibration: ring/etalon spacing 50–100 GHz.

4. Qudit Binning & Gates

Track A

Expect d = 4–6 bins.

Select bins with micro-etalon.

Primitive gate: filter + thermal phase shifters.

Qudit Fourier transform limited by filter sharpness.

Track B

Expect d = 16–32 bins (conservative); up to 64 with careful filtering & low loss.

Primitive gate: EO frequency beamsplitter (EOM @ Δf).

Build H, X, Z for qubits; extend to Fourier F_d for qudits.

RF drive: Δf = 50–100 GHz; Vπ ≈ 2–4 V.

5. Test Protocol

Binary check: measure color-change green↔red in broadband light → confirm preserved.

Single-bin prep: tune filter to λ₀; record emission.

Two-bin (qubit) test: apply EO coupling; measure superposition interference fringe → visibility > 0.9.

Multi-bin (qudit) test:

Track A: measure counts across {λ₀…λ₅}.

Track B: measure counts across {λ₀…λ₃₂}.

Run discrete Fourier transform gate (F_d); verify crosstalk < −15 dB.

Tomography: reconstruct density matrix (qubit/qudit); target fidelity ≥ 0.95 (qubit), ≥ 0.85 (qudit).

6. Expected Outcome

Track A (all gemstone): Stable 4–6 color-coded states with preserved green↔red binary.

Track B (hybrid): Programmable 16–32 states with high-fidelity frequency-bin gates.
