# Instalación

## Requisitos

- Servidor FiveM.
- `oxmysql` iniciado antes que FraseKill.
- ESX, QBCore y Qbox son opcionales; también funciona standalone.
- `zbrou_utils` **no** es necesario.

## Instalar

1. Mete la carpeta en resources y mantén el nombre `zbrou_frasekill`.
2. Añade:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

3. Deja `Config.Storage.AutoCreate = true` para crear/migrar tablas automáticamente, o ejecuta `sql/install.sql` si prefieres gestionar SQL manualmente.
4. Reinicia el servidor/recurso y vuelve a entrar.

## Primer owner

El único ACE que utiliza FraseKill es el del owner/admin principal:

```cfg
add_ace identifier.license:TU_LICENSE zbrou.frasekill.admin allow
```

También puedes ejecutar `/frasekilladmin` sin permiso: FraseKill te mostrará la línea exacta para tu license. Reinicia después de cambiar los ACE.

## Comprobaciones

- `/frasekill` abre el editor si el jugador tiene acceso.
- `/frasekilladmin` abre el panel para owner o admins delegados.
- `/frasekillstatus` muestra diagnósticos a administradores.
- `/frasekilltest` viene desactivado y solo debe usarse en un servidor de pruebas.
