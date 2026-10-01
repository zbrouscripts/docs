# Configuración

FraseKill separa la configuración en dos archivos para que sea fácil saber qué puede ver el cliente y qué debe quedarse únicamente en el servidor.

## `config.lua`

Este archivo contiene opciones compartidas y visuales. **No pongas secretos, tokens ni webhooks aquí.**

### General

```lua
Config.Debug = false
Config.Command = 'frasekill'
Config.AdminCommand = 'frasekilladmin'
Config.Locale = 'es'
Config.MaxCharacters = 70
```

- `Debug`: déjalo en `false` en producción.
- `Command`: comando del editor.
- `AdminCommand`: comando del panel admin.
- `Locale`: idioma inicial.
- `MaxCharacters`: máximo de caracteres permitido en cada frase.

### Slots

```lua
Config.DefaultSlotMode = 'fixed' -- fixed | random
```

- `fixed`: usa el slot seleccionado.
- `random`: elige aleatoriamente entre los slots válidos habilitados para random.

### Detección de muerte

```lua
Config.Death.Adapter = 'auto'
```

`auto` intenta detectar automáticamente la integración disponible. También puedes forzar `esx_ambulancejob`, `qb-ambulancejob`, `qbx_medical` o `standalone`.

### `Config.Display.Mode`

```lua
Config.Display = {
    Mode = 'death_state', -- timed | death_state | smart
    Seconds = 10,
    MaxSeconds = 20,
    FailsafeSeconds = 120,
    MinVisibleMs = 850
}
```

- `timed`: FraseKill aparece y desaparece después de `Seconds`, aunque el jugador siga muerto.
- `death_state`: permanece visible mientras el jugador esté muerto y desaparece al revivir. `FailsafeSeconds` evita que se quede en pantalla indefinidamente si otro recurso no notifica correctamente el revive.
- `smart`: usa el estado de muerte, pero además aplica `MaxSeconds` como límite máximo. Es útil si quieres que normalmente desaparezca al revivir, pero nunca permanezca demasiado tiempo.

`MinVisibleMs` evita que la frase aparezca y desaparezca tan rápido que no llegue a verse.

### Personalización

En `config.lua` también puedes cambiar valores predeterminados, límites de tamaño/posición/velocidad, tipografías, animaciones, idiomas y presets iniciales.

### Herramienta de prueba

```lua
Config.Developer.Enabled = false
```

Déjala desactivada en producción. Si la activas para pruebas, mantén `RequireAce = true`.

---

## `config_server.lua`

Este archivo **solo se ejecuta en el servidor**. Aquí van permisos, acceso, jobs/grupos, Tebex y cualquier lógica que no debe enviarse al cliente.

### Base de datos y almacenamiento

```lua
Config.Storage.Identifier = 'license'
```

- `license`: una configuración por Rockstar license. Es la opción recomendada.
- `character`: una configuración por personaje cuando el framework lo permite.
- `custom`: usa `CustomIdentifier` para devolver tu propio identificador estable.

`AutoCreate = true` crea y migra las tablas automáticamente.

### Jobs, gangs y grupos

`Config.GroupAccess` permite activar varios sistemas a la vez: Jobs, GuilleGangs V2, gangs nativas de QB/Qbox o un resolver custom.

Los permisos se guardan internamente con namespace para que dos sistemas con el mismo nombre no se mezclen, por ejemplo:

```text
job:police
guille:ballas
frameworkgang:vagos
custom:vip
```

También puedes exigir un grado mínimo, por ejemplo `job:police@2`.

### Modo de acceso

```lua
Config.Access.Mode = 'managed'
```

- `everyone`: todos pueden usar FraseKill.
- `managed`: panel admin + grupos + ACE + Tebex. Recomendado si vas a vender acceso dentro de tu servidor.
- `ace`: solo el permiso ACE configurado.
- `custom`: decide el acceso con `CustomCheck`.

### Administración

`Config.Admin.AcePermission` define el ACE del panel. `Owners` permite añadir identificadores directamente, aunque lo recomendado es ACE.

### Nombre del killer

`Config.KillerName.Mode` puede ser:

- `game`: nombre de FiveM.
- `character`: nombre del personaje si el framework lo proporciona.
- `custom`: usa `CustomResolver`.

### Moderación

`Config.Moderation` permite bloquear URLs, palabras concretas y añadir un validador propio. Toda la validación se realiza en servidor.

### Seguridad

`Config.Security` controla los cooldowns de guardado, reset y acciones administrativas. No conviene ponerlos a `0` en un servidor público.

### Caducidades

`Config.ExpiryNotifications` define cada cuánto se comprueban los accesos temporales y con cuánta antelación se avisa al jugador.

### Logs

`Config.Logs.Enabled` activa los logs. Las URLs se configuran únicamente en `server/webhooks.lua`.

### Tebex

`Config.Tebex` permite definir planes de minutos, horas, días, semanas, meses, años o permanentes. Consulta la página **Tebex y caducidades** para configurarlo paso a paso.

### Diagnóstico

`Config.Diagnostics` controla `/frasekillstatus`, un comando para admins que ayuda a comprobar base de datos, detección e integraciones.
