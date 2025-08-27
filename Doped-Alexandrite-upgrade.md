the upgrade” in two flavors and say exactly how many color-coded qudit states (d) you can expect to run cleanly.

The hardware we’ll build (two tracks)

Track A — Co-doped alexandrite (keep the color-change physics)

Crystal: Cr³⁺:BeAl₂O₄ grown by Czochralski or flux; this is the standard alexandrite laser crystal. Practical tuning band ≈ 710–800+ nm (often quoted ~701–858 nm). 
Crystech
Castech

Dopants (targets):

Chromium (the workhorse chromophore): 0.05–0.20 at.% Cr³⁺ (laser-grade range).

Vanadium / Iron (trace co-dopants): 10–200 ppm each (optional) to gently reshape sidebands while preserving the hallmark color change (green ↔ red). These ions are well-documented in natural/synthetic chrysoberyl alongside Cr³⁺. 
ResearchGate
+1

Filtering: add a micro-etalon or ring filter to carve discrete color bins from the alexandrite spectrum.

Track B — Hybrid alexandrite + thin-film LiNbO₃ (TFLN) modulators (for scale)

Keep Track A’s crystal unchanged (don’t risk the color center), and bond a TFLN layer on the photonic stack for electro-optic (Pockels) control. State-of-the-art TFLN modulators reach huge bandwidths at visible–NIR with low drive voltages, ideal for carving many frequency (color) bins and doing fast gates. 
Nature
arXiv
Harvard Nano-Optics

How many color-coded qudits can we run?
Build	What sets “d” (number of color states)	Conservative d (high fidelity)	Ambitious d (research-grade)
Track A: Co-doped only	Intrinsic Cr³⁺ band + gentle V³⁺/Fe³⁺ sidebands, selected by micro-etalon	d = 4–6	d = 8–10
Track B: Alex + TFLN	EO modulation at Δf (e.g., 50–100 GHz) + ring/etalon channelizer across 710–800 nm	d = 16–32	d = 64+ (window + loss dependent)
