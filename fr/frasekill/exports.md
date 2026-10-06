# Exports

{% hint style="info" %}
Cette page est destinée aux utilisateurs avancés qui veulent connecter FraseKill à un autre script. Tu peux l'ignorer pour une installation normale.
{% endhint %}

## Serveur

```lua
exports['zbrou_frasekill']:HasAccess(source)
exports['zbrou_frasekill']:GetStorageIdentifier(source)
exports['zbrou_frasekill']:ShowFraseKill(victimSource, killerSource, options)
exports['zbrou_frasekill']:ExportPreset(source, slotIndex)
exports['zbrou_frasekill']:ImportPreset(source, slotIndex, presetJson)
exports['zbrou_frasekill']:HasFraseKillAccess(source)
exports['zbrou_frasekill']:HasFraseKillAdmin(source)
```

## Client

```lua
exports['zbrou_frasekill']:SetExternalDeathState(trueOrFalse)
exports['zbrou_frasekill']:ShowFraseKill(payload)
exports['zbrou_frasekill']:HideFraseKill()
exports['zbrou_frasekill']:GetDetectedAdapter()
```
