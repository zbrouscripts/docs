# Tebex y caducidades

Tebex es opcional y se procesa server-side. Usa `Config.Access.Mode = 'managed_tebex'` si quieres los accesos gestionados normales **más** los entitlements activos de Tebex.

Actívalo en `config_server.lua`:

```lua
Config.Tebex.Enabled = true
```

```lua
Plans = {
    week = { Label = '1 week', Days = 7 },
    month = { Label = '1 month', Days = 30 },
    year = { Label = '1 year', Days = 365 },
    permanent = { Label = 'Permanent', Permanent = true }
}
```

## Compra / renovación

```text
frasekill_tebex {id} month {transaction}
```

Usa el mismo comando para renovar. Las renovaciones temporales amplían el tiempo restante y cada transacción queda registrada para evitar duplicados.

## Reembolso / chargeback

```text
frasekill_tebex_revoke {id} {transaction}
```

No uses revoke para una cancelación normal si el acceso debe seguir activo hasta terminar el periodo pagado. Los planes temporales caducan solos.

Los comandos de Tebex solo aceptan ejecución desde consola. FraseKill no guarda una API key de Tebex en la NUI.
