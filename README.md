# From Euclid II.5 to the Smith Chart
## A Shared Partition Ratio

**Author:** Carolina Johnson (CJ)
**Date:** October 2026
**License:** CC BY 4.0, Attribution required
**DOI:** [https://doi.org/10.5281/zenodo.23645952](https://doi.org/10.5281/zenodo.23645952)
**ORCID:** [https://orcid.org/0009-0002-8819-3347](https://orcid.org/0009-0002-8819-3347)

---

## What This Does

Shows that the two extents of Euclid's Elements, Book II, Proposition 5, are the sum and the difference of the incident and reflected amplitudes on a lossless transmission line. The Smith chart transformation sends their ratio to the reflection coefficient exactly, and the proposition itself is the power balance of the line.

---

## The Construction

Let AB be a segment with midpoint C, so that AC = CB = a. Let D lie on AB at signed distance b from C, with −a < b < a. The extents and their ratio are:

`AD = a + b`  and  `DB = a − b`

`u = AD / DB = (a + b) / (a − b)`

Euclid II.5 in algebraic form:

`(a + b)(a − b) + b² = a²`

---

## The Dictionary

Read a as the incident amplitude and b as the reflected amplitude at a plane of a lossless line.

| Euclid II.5 | Transmission line |
|-------------|-------------------|
| AC = CB = a | incident amplitude |
| CD = b | reflected amplitude |
| AD = a + b | V_max = Z₀ I_max |
| DB = a − b | V_min = Z₀ I_min |
| AD / DB | normalized impedance at the voltage maximum, equal to the standing wave ratio S |
| b / a | reflection coefficient Γ |
| AC², CD², AD · DB | 2Z₀ times incident, reflected, and net power |

---

## The Exact Reduction

The Smith chart transformation applied to the partition ratio:

`Γ = (u − 1) / (u + 1)`

The numerator is `2b / (a − b)` and the denominator is `2a / (a − b)`, so the factor a − b cancels and

`Γ = b / a`

The result is exact for every a > 0 and −a < b < a. No approximation enters.

---

## Boundary Behavior

| Cut | u | Γ | Line termination |
|-----|---|---|------------------|
| b = 0 | 1 | 0 | Matched |
| b → a | → ∞ | → 1 | Open circuit |
| b → −a | → 0 | → −1 | Short circuit |

The cut of II.5 covers the whole positive real axis of the chart and the whole open real diameter of the reflection-coefficient disk.

---

## II.5 as the Power Balance

Multiplying `(a + b)(a − b) + b² = a²` by 1/(2Z₀) gives

`P_net + P_ref = P_inc`

Euclid's rectangle is the delivered power, the square on CD is the reflected power, and the square on the half is the incident power. The delivered fraction is 1 − Γ².

With complex amplitudes, Γ = b/a and z = (a + b)/(a − b) hold unchanged, and the difference of squares becomes |a|² − |b|², which is the net power and the numerator of Re z.

---

## Worked Check

Smith's 1939 article works an example with load impedance 2.7 − j0.9. Taking a = 1:

| Quantity | Computed | Smith |
|----------|----------|-------|
| ρ = DB / AD | 0.3288 | circle marked 0.333 |
| z at 0.08 wavelength toward the generator | 0.792 − j1.021 | chart reading 0.8 − j1.0 |

---

## The Vocabulary

The pair a + b and a − b is named differently in Greek geometry, Arabic algebra, symbolic algebra, and transmission-line engineering. Smith's own parameter ρ is DB / AD, and Smith's 1939 article does not cite Euclid II.5. The claim is structural continuity under nomenclature displacement. It does not assert that Euclid, al-Khwārizmī, or Smith transmitted the relationship to one another.

---

## Repository Contents

| File | Description |
|------|-------------|
| `README.md` | This file |
| `Euclid II5 to the Smith Chart.pdf` | Full paper with all derivations and references |

---

## Citation
```
Johnson, C. (2026). From Euclid II.5 to the Smith Chart:
A Shared Partition Ratio. DOI: 10.5281/zenodo.23645952
```


## License

© 2026 Carolina Johnson (CJ)
Licensed under Creative Commons Attribution 4.0 International (CC BY 4.0)
Attribution required. [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)
