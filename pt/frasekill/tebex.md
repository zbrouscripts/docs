# Tebex e expirações

Ativa `Config.Tebex.Enabled = true` em `config_server.lua` e cria os planos que quiseres com minutos, horas, dias, semanas, meses, anos ou `Permanent = true`.

Compra/renovação:
```text
frasekill_tebex {id} month {transaction}
```

Reembolso/chargeback de uma transação concreta:
```text
frasekill_tebex_revoke {id} {transaction}
```

As renovações somam-se ao tempo restante e cada transação é registada separadamente. Planos temporários expiram automaticamente; não uses `revoke` apenas porque chegou a data normal de expiração. `Config.ExpiryNotifications` controla os avisos prévios.
