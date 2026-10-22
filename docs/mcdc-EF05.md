# MC/DC — EF-05 : fault_detect

Décision : D = A ∨ B ∨ C

- A : centi < -4000
- B : centi > 12500
- C : frozen_count ≥ 5

| Test | A | B | C | D | Condition étudiée |
|------|---|---|---|---|-------------------|
| T1   | F | F | F | F | Référence |
| T2   | V | F | F | V | Influence de A (T1/T2) |
| T3   | F | V | F | V | Influence de B (T1/T3) |
| T4   | F | F | V | V | Influence de C (T1/T4) |

A et B ne peuvent pas être vraies simultanément pour une même valeur de centi.

Vecteurs de test :
- T2 : ADC = 124, soit centi = -4001
- T3 : ADC = 2173, soit centi = 12507
- T4 : ADC = 931, répété cinq fois
