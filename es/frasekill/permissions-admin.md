# Permisos y administración

## Abrir el panel

```text
/frasekilladmin
```

El acceso recomendado al panel se controla con ACE:

```cfg
add_ace identifier.license:TU_LICENSE zbrou.frasekill.admin allow
```

Si intentas abrir el panel sin permiso, FraseKill muestra la línea ACE preparada con tu identificador para que puedas copiarla.

## Accesos de jugadores

Desde la pestaña **Accesos** puedes conceder acceso a jugadores online por ID o usando un identificador compatible. El permiso persistente se guarda con un identificador estable, no con el ID temporal de sesión.

Los accesos pueden ser permanentes o tener duración en minutos, horas, días, semanas, meses o años.

## Jobs y grupos

Los grupos disponibles dependen de `Config.GroupAccess` en `config_server.lua`. Puedes habilitar Jobs, GuilleGangs V2, gangs de QB/Qbox y resolvers custom. También se pueden exigir grados mínimos.

## Frases

La pestaña **Frases** permite buscar usuarios, abrir detalles, editar presets, resetear o eliminar configuraciones, conceder/quitar acceso manual, guardar notas internas y enviar un mensaje si el jugador está conectado.

## Seguridad

Todas las acciones importantes se validan de nuevo en servidor. No confíes en permisos de NUI o cliente como única protección.
