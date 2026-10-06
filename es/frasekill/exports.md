# Exports

{% hint style="info" %}
Esta página es para integraciones avanzadas. Para una instalación normal puedes ignorarla.
{% endhint %}

## Servidor

```lua
exports['zbrou_frasekill']:HasAccess(source)
exports['zbrou_frasekill']:GetStorageIdentifier(source)
exports['zbrou_frasekill']:ShowFraseKill(victimSource, killerSource, options)
exports['zbrou_frasekill']:ExportPreset(source, slotIndex)
exports['zbrou_frasekill']:ImportPreset(source, slotIndex, presetJson)
exports['zbrou_frasekill']:HasFraseKillAccess(source)
exports['zbrou_frasekill']:HasFraseKillAdmin(source)
```

`ShowFraseKill` mantiene las comprobaciones normales de seguridad.

Para una integración server-side que realmente necesite saltarse alguna comprobación existe `ShowFraseKillTrusted`. El recurso que lo llame debe estar añadido explícitamente a `Config.Security.TrustedExportResources`.

## Cliente

```lua
exports['zbrou_frasekill']:SetExternalDeathState(trueOrFalse)
exports['zbrou_frasekill']:ShowFraseKill(payload)
exports['zbrou_frasekill']:HideFraseKill()
exports['zbrou_frasekill']:GetDetectedAdapter()
```

Un estado de muerte enviado por el cliente no sustituye la validación server-side.
