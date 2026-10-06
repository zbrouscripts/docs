# Kompatybilność medyczna

Na większości serwerów możesz zostawić **Auto**. FraseKill wykryje uruchomiony, obsługiwany ambulance.

Obsługiwane są Wasabi V1/V2, Brutal, ARS, TK, Qbox, QB, AS, Sky, AK47, P Ambulance, standalone oraz **klasyczny/starszy/1.2-era ESX Ambulance Job i aktualny ESX Legacy**.

## ESX Ambulance Job

FraseKill obsługuje wieloletnie ścieżki: numeryczny/boolean status śmierci, `esx:onPlayerDeath`, spawn/revive i aktualny stan Legacy.

W starszych wersjach ESX z jednym wspólnym stanem nieprzytomny/martwy użyj **Wykrywanie śmierci → Incapacitated**.

Końcowa walidacja pozostaje po stronie serwera. Sam stan wysłany przez klienta nie jest dowodem śmierci. Prywatne forki mogą użyć własnego sprawdzania server-side.
