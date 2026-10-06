# Solución de problemas

## `/frasekill` no abre

1. Comprueba que el jugador tenga acceso.
2. Si eres admin, abre `/frasekillstatus` para ver el estado del script.
3. Revisa F8 y la consola del servidor por si aparece algún error.

## No puedo abrir FraseKill Admin

Ejecuta `/frasekilladmin`.

Si todavía no eres owner, el script te mostrará la línea que debes añadir a `server.cfg`.

## Ajustes del script aparece en gris

Tienes seleccionado **Archivos de configuración**.

Si quieres cambiar las opciones desde el panel, selecciona **Panel de administración**.

## No detecta bien mi ambulance job

Abre **Ajustes del script → Detección de muerte** y prueba primero con **Auto**.

Si tienes varios medical instalados, selecciona manualmente el que utilizas.

## Problema con la SQL

FraseKill prepara sus tablas automáticamente.

Si tu servidor utiliza una instalación manual de la base de datos, también tienes disponible:

```text
sql/install.sql
```

## Tebex no da acceso

Comprueba que hayas seleccionado **Acceso gestionado + Tebex** y que el nombre del plan coincida con el que has configurado.

## He cambiado muchos ajustes y quiero volver atrás

En **Ajustes del script** pulsa **Restablecer predeterminado**.

Esto no borra las frases de los jugadores, accesos, normas ni administradores.
