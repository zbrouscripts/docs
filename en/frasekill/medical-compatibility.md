# Medical compatibility

`Config.Death.Adapter = 'auto'` is recommended. FraseKill checks the resources listed in `Config.Death.Preferred` and selects the first supported running system.

Built-in adapter names include:

- Wasabi Ambulance V2 — `wasabi_ambulance_v2`
- Wasabi Ambulance V1 — `wasabi_ambulance`
- Brutal Ambulance Job — `brutal_ambulancejob`
- ARS Ambulance Job — `ars_ambulancejob`
- TK Ambulance Job — `tk_ambulancejob`
- Qbox Medical — `qbx_medical`
- Qbox Ambulance — `qbx_ambulancejob`
- QB Ambulance — `qb-ambulancejob` / `qb_ambulancejob`
- ESX Ambulance — `esx_ambulancejob`
- AS Ambulance — `as-ambulance`
- Sky Ambulance — `sky_ambulancejob`
- AK47 Ambulance — `ak47_ambulancejob`
- P Ambulance — `p_ambulancejob`
- Standalone native death

`TriggerStage` can be `incapacitated` or `dead`. Some medical resources expose both stages while others expose one combined dead state.

For a private/unlisted medical resource, use `Config.DeathServer.CustomDeadCheck` with a **server-side cached state/export**. Do not trust a client boolean as proof of death.

Use `/frasekillstatus` to see detected medical resources and test the exact framework/medical combination before production.
