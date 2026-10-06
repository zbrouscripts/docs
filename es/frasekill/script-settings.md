# Ajustes del script

Abre **FraseKill Admin → Ajustes del script** para cambiar las opciones comunes del recurso sin tener que editar Lua. El panel está pensado para owners de servidor: cada ajuste tiene un `?` con una explicación sencilla.

## Modo de configuración

En la parte superior eliges cómo quieres configurar FraseKill:

- **Archivos de configuración** — FraseKill usa `config.lua` y `config_server.lua`. El resto del panel queda bloqueado y oscurecido para dejar claro que no se puede editar desde ahí.
- **Panel de administración** — los ajustes compatibles se pueden cambiar y guardar directamente desde la interfaz.

Solo el owner principal puede cambiar este modo. Cambiar de modo no borra tus frases ni los accesos de los jugadores.

## Qué puedes cambiar desde el panel

### Interfaz

Idioma por defecto, tema Classic/Liquid Glass, comandos principales y los tres colores globales del menú.

- **Color de detalles** — botones activos, switches, slot seleccionado y resaltados.
- **Color del fondo** — fondo principal del menú.
- **Color base** — tarjetas, campos, slots inactivos y bloques interiores.

Los tres colores tienen un icono de reset individual para volver al valor definido en los archivos de configuración.

### FraseKill

Límite de caracteres y valores predeterminados que recibirán las nuevas configuraciones: modo de slot, frase, activación, colores, tamaño, brillo, animaciones y apariencia del nombre del killer.

**Fijo** mantiene el slot elegido. **Aleatorio** va cambiando entre tus slots válidos para que distintas kills puedan mostrar frases diferentes.

### Detección de muerte

Adaptador médico, momento en el que se considera válida la muerte, forma de mostrar la FraseKill y tiempo máximo en pantalla. Si usas un ambulance compatible, lo normal es dejar el adaptador en **Auto**.

### Acceso de jugadores

Modo de acceso, jobs/grupos y avisos de caducidad. Los modos disponibles son **Acceso gestionado**, **Acceso gestionado + Tebex** y **Comprobación personalizada**.

### Normas

Visibilidad de las normas y filtros básicos de moderación. Las normas y palabras bloqueadas se gestionan desde sus apartados del panel y se validan en el servidor.

### Notificaciones

Activa o desactiva los logs y cambia el nombre que aparecerá en los avisos de Discord. Las URLs de webhook siguen estando únicamente en los archivos privados del servidor.

## Restablecer predeterminado

El botón global **Restablecer predeterminado** está disponible solo para el owner. Pide confirmación y elimina todos los cambios guardados en **Ajustes del script**, devolviendo las opciones a los valores originales de `config.lua` y `config_server.lua`.

No borra:

- frases o presets de jugadores;
- accesos o caducidades;
- normas o palabras bloqueadas;
- administradores delegados.

También mantiene el modo de configuración actual. Los cambios que necesitan reiniciar el recurso quedan indicados como pendientes.

{% hint style="info" %}
Los secretos, URLs de webhook y callbacks Lua no se muestran en el panel web. Se configuran siempre en los archivos privados del servidor.
{% endhint %}
