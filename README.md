# GeneModeling

## Goals
- Modeling Gene regulatory networks

## Central Dogma of Biology
DNA → mRNA → Protein

### 1. Transcription
- DNA is transcribed into mRNA.
- mRNA degrades at rate γ<sub>m</sub>.
- While present, mRNA is a template for protein synthesis.

### 2. Translation
- Ribosomes translate mRNA into protein.
- Protein degrades at rate γ<sub>p</sub>.

### 3. Mathematical Model

<pre>
dm/dt = k<sub>m</sub> – γ<sub>m</sub>·m
dp/dt = k<sub>p</sub>·m – γ<sub>p</sub>·p
</pre>

| Symbol        | Definition                        | Units                    |
|---------------|-----------------------------------|--------------------------|
| m             | mRNA concentration                | molecules (or nM)        |
| p             | Protein concentration             | molecules (or nM)        |
| k<sub>m</sub> | mRNA production rate              | molecules·time⁻¹         |
| γ<sub>m</sub> | mRNA degradation rate             | time⁻¹                   |
| k<sub>p</sub> | Protein production rate per mRNA  | molecules·time⁻¹·(mRNA)⁻¹ |
| γ<sub>p</sub> | Protein degradation rate          | time⁻¹                   |

**Initial conditions:**  
<pre>
m(0) = m₀,   p(0) = p₀
</pre>
