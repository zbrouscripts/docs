# Exports

## Server

```lua
exports['zbrou_frasekill']:HasAccess(source)
exports['zbrou_frasekill']:GetStorageIdentifier(source)
exports['zbrou_frasekill']:ShowFraseKill(victimSource, killerSource, options)
exports['zbrou_frasekill']:ExportPreset(source, slotIndex)
exports['zbrou_frasekill']:ImportPreset(source, slotIndex, presetJson)
```

- `HasAccess`: returns whether a player currently has effective access.
- `GetStorageIdentifier`: returns the identifier used to store that profile.
- `ShowFraseKill`: triggers the FraseKill flow for a specific victim/killer from another resource.
- `ExportPreset`: exports a slot as JSON.
- `ImportPreset`: imports preset JSON into a slot.

## Client

```lua
exports['zbrou_frasekill']:SetExternalDeathState(trueOrFalse)
exports['zbrou_frasekill']:ShowFraseKill(payload)
exports['zbrou_frasekill']:HideFraseKill()
exports['zbrou_frasekill']:GetDetectedAdapter()
```

`SetExternalDeathState` is useful when another resource owns a custom death state.
