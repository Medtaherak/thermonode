
# Journal des défauts révélés — TP 3

| ID | Étape | Exigence | Test révélateur | Symptôme observé (message Unity/pytest) | Hypothèse de cause | Technique qui l'a révélé |
|---|---|---|---|---|---|---|
| DEF-01 | 1 | EF-05 | test_EF05_range_check_bounds | Expected TRUE Was FALSE (ligne 48) | Limite supérieure de range_check mal traitée | Valeurs limites (BVA) |
| DEF-02 | 2 | EF-03 | test_EF03_transient_partial_window ; test_EF03_invalid_sample_is_excluded | Expected 100 Was 2600 ; Expected 2500 Was 2650 ; AddressSanitizer : index 5 hors limites | Gestion incorrecte de la fenêtre et accès hors limites du tableau | Tests de séquences et analyse mémoire |
| DEF-03 | | | | | | |
| DEF-04 | | | | | | |
| DEF-05 | | | | | | |
| DEF-06 | | | | | | |
| DEF-07 | | | | | | |
| DEF-08 | | | | | | |
