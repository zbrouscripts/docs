# Tebex y caducidades

FraseKill puede entregar acceso automáticamente mediante comandos de servidor de Tebex.

## Activar Tebex

En `config_server.lua`:

```lua
Config.Tebex.Enabled = true
```

Define los planes que quieras:

```lua
Plans = {
    week = { Label = '1 semana', Days = 7 },
    month = { Label = '1 mes', Days = 30 },
    permanent = { Label = 'Permanente', Permanent = true }
}
```

También puedes utilizar minutos, horas, semanas, meses o años.

## Comando de compra o renovación

En el paquete de Tebex:

```text
frasekill_tebex {id} month {transaction}
```

`month` debe coincidir con la clave del plan. Las renovaciones se acumulan sobre el tiempo restante y cada transacción queda registrada por separado.

## Reembolso o chargeback

```text
frasekill_tebex_revoke {id} {transaction}
```

Este comando revoca esa transacción concreta sin eliminar otras compras válidas del mismo jugador.

## Caducidad normal

Los planes temporales caducan automáticamente. No necesitas ejecutar `revoke` cuando simplemente termina el periodo pagado.

## Avisos

`Config.ExpiryNotifications` controla los avisos previos a la caducidad. Si el jugador mantiene acceso por otro origen, como job o ACE, FraseKill evita avisar como si fuera a perder totalmente el acceso.
