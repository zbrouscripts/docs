# Configuración

FraseKill se puede configurar de dos formas:

- **Desde el panel de administración**, que es la opción más cómoda si no quieres tocar archivos.
- **Desde los archivos de configuración**, si prefieres tener todo escrito en Lua.

Puedes elegir el modo desde **FraseKill Admin → Ajustes del script**.

## Panel de administración

El panel permite cambiar de forma visual la mayoría de ajustes habituales: idioma, colores, valores predeterminados de FraseKill, detección de muerte, accesos, Tebex, normas y notificaciones.

Cada opción tiene un símbolo `?` que explica qué hace sin necesidad de conocer programación.

Si eliges **Archivos de configuración**, las opciones del panel aparecen bloqueadas para dejar claro que los cambios deben hacerse en los archivos.

## Prueba el panel antes de configurarlo

Puedes abrir una **demo interactiva de Ajustes del script** con la misma estética del panel real. Puedes cambiar Classic/Liquid Glass, colores, switches, desplegables, bloquear el panel con Archivos de configuración y probar Restablecer predeterminado.

La demo sigue la misma estructura del panel real: una sola pantalla con scroll, los bloques en el mismo orden y la barra de acciones fija abajo.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=es" %}

[**Abrir la demo a pantalla completa →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=es)

{% hint style="info" %}
Es solo una demo de la documentación: no se conecta a FiveM, SQL ni Tebex y no guarda cambios en ningún servidor.
{% endhint %}

## Archivos de configuración

### `config.lua`

Aquí están los ajustes generales que no contienen información privada: idioma, apariencia, comandos, valores predeterminados, animaciones y comportamiento visual.

### `config_server.lua`

Aquí están los ajustes que solo debe leer el servidor: accesos, administración, Tebex, seguridad y otras opciones internas.

### `server/webhooks.lua`

Aquí puedes poner los webhooks de Discord si quieres usar logs.

{% hint style="info" %}
Si no tienes mucha experiencia configurando scripts, usa el **Panel de administración** para los ajustes normales y toca los archivos solo cuando la documentación te lo indique.
{% endhint %}
