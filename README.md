# GeneModeling

## Goals
- Model gene regulatory networks using ODEs

## Central Dogma of Biology
DNA → mRNA → Protein

### 1. Transcription
- DNA is transcribed into mRNA.
- mRNA degrades at rate \(\gamma_m\).
- While present, mRNA is a template for protein synthesis.

### 2. Translation
- Ribosomes translate mRNA into protein.
- Protein degrades at rate \(\gamma_p\).

### 3. Mathematical Model

\[
\frac{dm}{dt} = k_m - \gamma_m\,m
\]
\[
\frac{dp}{dt} = k_p\,m - \gamma_p\,p
\]

| Symbol        | Definition                        | Units                  |
|---------------|-----------------------------------|------------------------|
| \(m\)         | mRNA concentration                | molecules (or nM)      |
| \(p\)         | Protein concentration             | molecules (or nM)      |
| \(k_m\)       | mRNA production rate              | molecules·time⁻¹       |
| \(\gamma_m\)  | mRNA degradation rate             | time⁻¹                 |
| \(k_p\)       | Protein production rate per mRNA  | molecules·time⁻¹·(mRNA)⁻¹ |
| \(\gamma_p\)  | Protein degradation rate          | time⁻¹                 |

**Initial conditions:**  
\[
m(0) = m_0,\quad p(0) = p_0
\]
