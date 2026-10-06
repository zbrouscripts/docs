# Compatibilité médicale

Dans la plupart des serveurs, laisse **Auto**. FraseKill détecte la ressource ambulance compatible en cours d'exécution.

Compatibilité incluse avec Wasabi V1/V2, Brutal, ARS, TK, Qbox, QB, AS, Sky, AK47, P Ambulance, standalone et **ESX Ambulance Job classique, anciennes versions/1.2 et Legacy actuel**.

## ESX Ambulance Job

FraseKill prend en charge les chemins utilisés au fil des versions : état numérique/booléen, `esx:onPlayerDeath`, spawn/revive et l'état Legacy actuel.

Pour les anciennes versions avec un seul état inconscient/mort, utilise **Détection de mort → Incapacitated**.

La validation finale reste côté serveur. Un état client seul n'est pas accepté comme preuve de mort. Les forks privés peuvent utiliser la vérification serveur personnalisée.
