# Instalación

## Inicio rápido

1. Instala e inicia `oxmysql`.
2. Añade `zbrou_frasekill` a tu servidor.
3. Revisa los permisos y la configuración antes de abrir el servidor al público.
4. Añade al `server.cfg`:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

5. Reinicia el recurso o el servidor.

FraseKill crea y migra sus tablas automáticamente cuando `Config.Storage.AutoCreate = true`, que es el valor predeterminado. Si prefieres preparar la base de datos manualmente, también puedes ejecutar `sql/install.sql`.

## Primer administrador

Ejecuta:

```text
/frasekilladmin
```

Si todavía no tienes permisos, el propio menú mostrará la línea ACE que debes copiar en `server.cfg`. También puedes añadirla manualmente:

```cfg
add_ace identifier.license:TU_LICENSE zbrou.frasekill.admin allow
```

Reinicia el recurso después de cambiar permisos ACE.

## Comprobación

- `/frasekill` abre el editor cuando el jugador tiene acceso.
- `/frasekilladmin` abre el panel de administración.
- `/frasekillstatus` muestra diagnóstico para administradores.

La herramienta `/frasekilltest` existe solo para desarrollo y viene desactivada en la versión pública.
