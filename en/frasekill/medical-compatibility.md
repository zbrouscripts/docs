# Medical compatibility

On most servers you can leave detection on **Auto** and FraseKill will use the supported ambulance resource that is running.

## Supported

- Wasabi Ambulance V1 and V2
- Brutal Ambulance Job
- ARS Ambulance Job
- TK Ambulance Job
- Qbox Medical / Qbox Ambulance
- QB Ambulance
- **Classic/older/1.2-era ESX Ambulance Job and current ESX Legacy**
- AS Ambulance
- Sky Ambulance Job
- AK47 Ambulance Job
- P Ambulance
- Standalone

### ESX Ambulance Job

FraseKill supports the long-lived `esx_ambulancejob` paths used across classic and current generations: numeric/boolean death status, `esx:onPlayerDeath`, spawn/revive flows and current Legacy state.

For older ESX builds with one combined unconscious/dead state, use **Death detection → Incapacitated** for maximum compatibility.

The final check remains server-side. A client-provided state by itself is not accepted as proof of death.

Private forks that replace the normal death flow can use the custom server-side death check.
