# Configuración

FraseKill puede configurarse desde el **panel visual de Ajustes del script** o directamente desde `config.lua` y `config_server.lua`.

## Panel visual de configuración

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=es" %}

[**Ver panel de configuración a pantalla completa →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=es)

El panel permite cambiar la mayoría de ajustes habituales sin editar código. Las opciones privadas siguen estando en los archivos del recurso.

## Archivos de configuración

- `config.lua` — idioma, apariencia, comandos y valores predeterminados.
- `config_server.lua` — accesos, administración, Tebex, seguridad y opciones del servidor.
- `server/webhooks.lua` — webhooks de Discord.

## Permisos y administración

El owner principal se añade en `server.cfg`:

```cfg
add_ace identifier.license:TU_LICENSE zbrou.frasekill.admin allow
```

Si no sabes tu license, ejecuta `/frasekilladmin` y FraseKill te mostrará la línea exacta.

Los demás administradores se crean desde el panel, con permisos separados. Ser administrador no da automáticamente acceso para usar FraseKill como jugador.
