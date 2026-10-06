# Permisos y administración

## Owner

FraseKill utiliza un único ACE:

```cfg
add_ace identifier.license:TU_LICENSE zbrou.frasekill.admin allow
```

Ese ACE da autoridad completa al owner principal. **No** concede automáticamente acceso de uso a FraseKill.

## Administradores delegados

Desde el panel, el owner puede crear admins y dar permisos individuales: ver perfiles, dar/quitar accesos, editar/restablecer frases, eliminar perfiles, enviar mensajes, editar normas, gestionar palabras bloqueadas y configurar el script.

Los permisos de admin se guardan en SQL y están separados del acceso normal de jugadores.

## Modos de acceso de jugadores

`Config.Access.Mode` solo admite:

- `managed` — accesos de jugadores/jobs/grupos gestionados por FraseKill.
- `managed_tebex` — lo anterior más entitlements activos de Tebex.
- `custom` — tu `Config.Access.CustomCheck` server-side.

No existe modo ACE para usar FraseKill.

## Acceso temporal

Los accesos gestionados pueden ser permanentes o temporales. La caducidad se valida server-side. Si otra fuente válida sigue dando acceso, FraseKill no avisa incorrectamente de que el jugador lo ha perdido por completo.
