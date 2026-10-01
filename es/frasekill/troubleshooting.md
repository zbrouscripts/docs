# Solución de problemas

## `/frasekill` no abre

- Comprueba que el jugador tenga acceso efectivo.
- Revisa `/frasekillstatus` como administrador.
- Mira F8 y la consola del servidor por errores.

## La base de datos no crea tablas

- Verifica que `oxmysql` esté iniciado antes de `zbrou_frasekill`.
- Comprueba las credenciales de tu base de datos.
- Si no quieres creación automática, ejecuta `sql/install.sql` manualmente.

## El panel admin no abre

Añade el ACE correcto en `server.cfg` y reinicia el recurso:

```cfg
add_ace identifier.license:TU_LICENSE zbrou.frasekill.admin allow
```

## La frase aparece detrás de otra NUI

Aumenta `Config.NuiZIndex` solo si otro recurso fullscreen se está dibujando por encima.

## La FraseKill no desaparece al revivir

- Revisa `Config.Display.Mode`.
- Comprueba qué adapter detecta `/frasekillstatus`.
- `FailsafeSeconds` actúa como límite de seguridad en `death_state`.

## Tebex no concede acceso

- Comprueba `Config.Tebex.Enabled`.
- El comando debe ejecutarse desde consola/Tebex, no desde un jugador.
- Verifica que el nombre del plan coincida exactamente con la clave configurada.

## Necesito ayuda

Consulta **Soporte** para entrar al Discord oficial.
