# Exports

## Servidor

```lua
exports['zbrou_frasekill']:HasAccess(source)
exports['zbrou_frasekill']:GetStorageIdentifier(source)
exports['zbrou_frasekill']:ShowFraseKill(victimSource, killerSource, options)
exports['zbrou_frasekill']:ExportPreset(source, slotIndex)
exports['zbrou_frasekill']:ImportPreset(source, slotIndex, presetJson)
```

- `HasAccess`: devuelve si un jugador tiene acceso efectivo.
- `GetStorageIdentifier`: devuelve el identificador usado para almacenar su configuración.
- `ShowFraseKill`: muestra el flujo de FraseKill para una víctima/killer concretos desde otro recurso.
- `ExportPreset`: exporta un slot como JSON.
- `ImportPreset`: importa un preset JSON en un slot.

## Cliente

```lua
exports['zbrou_frasekill']:SetExternalDeathState(trueOrFalse)
exports['zbrou_frasekill']:ShowFraseKill(payload)
exports['zbrou_frasekill']:HideFraseKill()
exports['zbrou_frasekill']:GetDetectedAdapter()
```

`SetExternalDeathState` es útil cuando otro recurso controla un estado de muerte personalizado.
