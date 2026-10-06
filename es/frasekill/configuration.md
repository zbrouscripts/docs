# Configuración

FraseKill tiene dos archivos de configuración y un panel visual opcional de **Ajustes del script**.

## `config.lua`

Ajustes compartidos y no secretos: comandos, idioma por defecto, apariencia del menú, valores de FraseKill, fuentes, animaciones, visualización y detección médica. No pongas tokens ni webhooks aquí.

Valores importantes:

```lua
Config.Locale = 'en'
Config.UI.Theme = 'classic'
Config.UI.AccentColor = '#0e58d8'
Config.UI.BackgroundColor = '#15181e'
Config.UI.BaseColor = '#1a1e25'
Config.DefaultSlotMode = 'fixed'
Config.MaxCharacters = 70
Config.Death.Adapter = 'auto'
```

`fixed` mantiene el slot elegido. `random` va cambiando entre los slots válidos habilitados para que distintas kills puedan mostrar frases diferentes.

## `config_server.lua`

Ajustes privados/server-side: SQL, almacenamiento, jobs/grupos, acceso, ACE del owner, admins delegados, nombres, moderación, seguridad, Tebex, logs, diagnósticos y callbacks privados.

No muevas secretos a archivos visibles por el cliente. Las URLs de Discord van en `server/webhooks.lua`.

## Fuente de configuración

El owner puede elegir **Archivos de configuración** o **Panel de administración**.

- **Archivos de configuración**: mandan `config.lua` y `config_server.lua`; los controles del panel quedan bloqueados. Los valores del panel se conservan solo como borrador.
- **Panel de administración**: los ajustes seguros compatibles se aplican desde los overrides guardados del panel.

Callbacks, secretos, webhooks y otros ajustes avanzados siguen estando en archivos aunque uses el panel.
