# Configuración

FraseKill se puede configurar de dos formas: desde el **panel visual de Ajustes del script**, que permite cambiar la mayoría de opciones de `config.lua` y `config_server.lua` sin tocar código, o editando directamente esos archivos.

Algunas opciones privadas, como los webhooks y ciertos ajustes sensibles, permanecen únicamente en los archivos del recurso.

## Panel visual de configuración

Este es el mismo tipo de panel que encontrarás dentro de FraseKill Admin. Puedes probarlo aquí antes de tocar nada en tu servidor.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=es" %}

[**Ver panel de configuración a pantalla completa →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=es)

{% hint style="info" %}
La demo no se conecta a FiveM, SQL ni Tebex y no guarda cambios en ningún servidor.
{% endhint %}

## Configurar desde archivos

### `config.lua`

Aquí están los ajustes generales: idioma, apariencia, comandos, valores predeterminados, animaciones y comportamiento visual.

### `config_server.lua`

Aquí están los ajustes del servidor: accesos, administración, Tebex, seguridad y otras opciones internas.

### `server/webhooks.lua`

Aquí puedes añadir los webhooks de Discord si quieres usar logs.

{% hint style="info" %}
Si no tienes mucha experiencia configurando scripts, lo más sencillo es usar el **panel visual** para los ajustes normales y tocar los archivos solo cuando sea necesario.
{% endhint %}
