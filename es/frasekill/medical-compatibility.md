# Compatibilidad médica

En la mayoría de servidores puedes dejar **Auto** y FraseKill detectará el ambulance compatible que esté iniciado.

## Compatibles

- Wasabi Ambulance V1 y V2
- Brutal Ambulance Job
- ARS Ambulance Job
- TK Ambulance Job
- Qbox Medical / Qbox Ambulance
- QB Ambulance
- **ESX Ambulance Job clásico, versiones antiguas/1.2 y Legacy actual**
- AS Ambulance
- Sky Ambulance Job
- AK47 Ambulance Job
- P Ambulance
- Standalone

### ESX Ambulance Job

FraseKill incluye compatibilidad con las rutas usadas durante años por `esx_ambulancejob`: estados numéricos y booleanos, `esx:onPlayerDeath`, spawn/revive y las versiones Legacy más recientes.

En versiones antiguas de ESX que usan un único estado de inconsciente/muerto, deja **Detección de muerte → Incapacitado** para obtener la mayor compatibilidad.

La comprobación final sigue haciéndose en el servidor. FraseKill no convierte un simple estado enviado por el cliente en una muerte válida.

Si utilizas un fork privado que cambia completamente su sistema de muerte, puedes conectarlo mediante la comprobación personalizada server-side.
