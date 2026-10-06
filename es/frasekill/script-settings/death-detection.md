# Detección de muerte

Este apartado decide **cuándo y dónde puede aparecer FraseKill**.

En la mayoría de servidores puedes dejar el sistema médico en **Auto**. También puedes elegir si FraseKill aparece al quedar incapacitado o en la muerte final.

## Zonas de muerte

Las zonas no dan acceso a FraseKill. El killer sigue necesitando su acceso normal.

Puedes configurar círculos con centro y radio directamente desde el panel:

- **Fuera permitido + zona Bloquear** — FraseKill funciona normalmente excepto dentro de esas zonas.
- **Fuera bloqueado + zona Permitir** — FraseKill solo funciona dentro de las zonas permitidas.

Si una zona permitida y una bloqueada se solapan, **Bloquear tiene prioridad**.

El botón **Usar mi posición** toma la posición actual del administrador. **Previsualizar radio** oculta el panel unos segundos y dibuja el radio en el mundo: azul para permitir y rojo para bloquear.

La decisión real se hace server-side usando la posición donde muere la víctima. Estar dentro de una zona nunca sustituye el acceso del jugador.

Consulta **Compatibilidad médica** para ver la lista de scripts reconocidos.
