# Instalación

## Lo que necesitas

- Un servidor FiveM.
- Tener el recurso `oxmysql` en tu servidor.
- ESX, QBCore y Qbox son opcionales. FraseKill también funciona sin framework.
- `zbrou_utils` no es necesario.

## Añadir FraseKill al servidor

1. Coloca la carpeta en tus recursos y mantén el nombre:

```text
zbrou_frasekill
```

2. En tu `server.cfg`, comprueba que `oxmysql` aparece antes que FraseKill:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

3. La SQL necesaria se prepara automáticamente la primera vez que inicia FraseKill. También se incluye `sql/install.sql` por si prefieres prepararla manualmente.

4. Reinicia el recurso o el servidor.

## Dar acceso al owner

FraseKill usa un único ACE para el owner principal:

```cfg
add_ace identifier.license:TU_LICENSE zbrou.frasekill.admin allow
```

Si ejecutas `/frasekilladmin` sin tener permiso, el propio script te mostrará la línea exacta que debes copiar.

## Probar FraseKill mientras configuras el servidor

La herramienta `/frasekilltest` viene desactivada en la versión pública.

Si estás configurando el servidor tú solo y quieres usarla, abre `config.lua`, busca:

```lua
Config.Developer = {
    Enabled = false,
    Command = 'frasekilltest',
    RequireAdmin = true,
}
```

y cambia únicamente:

```lua
Enabled = true
```

Te recomendamos dejar `RequireAdmin = true` para que solo el owner/admin pueda ejecutar el test. Cuando termines de configurar el servidor, vuelve a dejar `Enabled = false`.
