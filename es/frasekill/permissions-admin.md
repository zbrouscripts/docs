# Permisos y administración

## Owner principal

El owner es la persona que tiene acceso completo al panel de FraseKill.

Añade una sola línea en tu `server.cfg`:

```cfg
add_ace identifier.license:TU_LICENSE zbrou.frasekill.admin allow
```

Si no sabes cuál es tu license, entra al servidor y ejecuta:

```text
/frasekilladmin
```

FraseKill te mostrará la línea exacta que debes copiar.

## Añadir más administradores

No hace falta añadir más líneas ACE.

El owner puede crear administradores directamente desde el panel y decidir qué puede hacer cada uno, por ejemplo:

- ver jugadores;
- dar o quitar acceso;
- editar o restablecer FraseKill;
- gestionar normas y palabras bloqueadas;
- cambiar los Ajustes del script.

Ser administrador **no da automáticamente acceso para usar FraseKill como jugador**.

## Acceso de jugadores

Los accesos se gestionan desde el panel y pueden ser:

- permanentes;
- por horas;
- por días;
- por semanas;
- por meses;
- por años.

También puedes dar acceso a jobs o grupos.

Si usas Tebex, consulta **Ajustes del script → Acceso y Tebex**.
