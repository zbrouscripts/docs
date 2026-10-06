# Compatibilidad médica

Se recomienda `Config.Death.Adapter = 'auto'`. FraseKill revisa `Config.Death.Preferred` y usa el primer sistema compatible que esté iniciado.

Adaptadores incluidos:

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
- Muerte nativa standalone

`TriggerStage` puede ser `incapacitated` o `dead`. Algunos medical distinguen ambas fases y otros solo exponen un estado combinado.

Para un medical privado/no listado usa `Config.DeathServer.CustomDeadCheck` con estado/export **server-side** en caché. No uses un booleano del cliente como prueba de muerte.

`/frasekillstatus` muestra los recursos detectados. Prueba siempre la combinación exacta framework + ambulance antes de producción.
