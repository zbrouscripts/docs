# Acceso y Tebex

Aquí eliges quién puede usar FraseKill.

## Modos de acceso

### Acceso gestionado

Los accesos se dan desde FraseKill Admin a jugadores, jobs o grupos.

Pueden ser permanentes o tener una duración.

### Acceso gestionado + Tebex

Funciona igual que el acceso gestionado, pero también reconoce los accesos comprados mediante Tebex.

### Comprobación personalizada

Para servidores que ya tienen su propio sistema de permisos y quieren conectarlo con FraseKill.

## Tebex

Tebex es opcional.

Desde los archivos puedes definir los planes que quieras ofrecer, por ejemplo:

- 1 semana;
- 1 mes;
- 1 año;
- permanente.

En el paquete de Tebex se utiliza un comando de entrega como:

```text
frasekill_tebex {id} month {transaction}
```

Para retirar una compra por reembolso o chargeback:

```text
frasekill_tebex_revoke {id} {transaction}
```

Las compras temporales caducan automáticamente. Una renovación añade más tiempo al acceso que ya tenga el jugador.
