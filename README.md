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

| Symbol        | Definition                       |
|---------------|----------------------------------|
| m             | mRNA concentration               |
| p             | Protein concentration            |
| k<sub>m</sub> | mRNA production rate             |
| γ<sub>m</sub> | mRNA degradation rate            |
| k<sub>p</sub> | Protein production rate per mRNA |
| γ<sub>p</sub> | Protein degradation rate         |

### 4. How to find the Steady State
dm/dt = 0 -> m = k<sub>m/γ<sub>m

dp/dt = 0 -> p = k<sub>p * m/γ<sub>p --> p = k<sub>p * k<sub>m / γ<sub>p  * γ<sub>m


