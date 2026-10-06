# Exports

{% hint style="info" %}
This page is only for advanced users connecting FraseKill to another script. You can ignore it for a normal installation.
{% endhint %}

## Server

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
