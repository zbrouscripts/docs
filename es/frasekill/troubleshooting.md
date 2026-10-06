# Solución de problemas

## `/frasekill` no abre

- Confirma que el jugador tiene acceso efectivo.
- Revisa `Config.Access.Mode`.
- Ejecuta `/frasekillstatus` como admin.
- Revisa F8 y consola del servidor.

## El panel admin no abre

Comprueba el ACE del owner y reinicia después de cambiarlo:

```cfg
add_ace identifier.license:TU_LICENSE zbrou.frasekill.admin allow
```

Los admins delegados se gestionan desde el panel y no necesitan un ACE de uso de jugador.

## Ajustes del script aparece en gris/bloqueado

Es normal si está seleccionado **Archivos de configuración**. El owner debe cambiar a **Panel de administración** para editar desde la UI.

## Detecta mal el ambulance

Ejecuta `/frasekillstatus`, revisa `Config.Death.Preferred` y confirma el nombre real del recurso. Puedes forzar `Config.Death.Adapter` o usar el check server-side personalizado.

## Faltan tablas

Inicia `oxmysql` primero. Si AutoCreate está desactivado, aplica los SQL correspondientes de `sql/`.

## Tebex no da acceso

Comprueba `Config.Tebex.Enabled`, usa `managed_tebex`, revisa la clave del plan y asegúrate de que el comando lo ejecuta Tebex/consola.

## Los colores se ven mal

Usa los selectores separados de detalles/fondo/base. Cada color tiene reset individual y el owner puede usar **Restablecer predeterminado** para borrar todos los overrides de Ajustes del script.
