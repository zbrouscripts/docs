# Tebex and expirations

FraseKill can automatically deliver access through Tebex game-server commands.

## Enable Tebex

In `config_server.lua`:

```lua
Config.Tebex.Enabled = true
```

Create any plans you need:

```lua
Plans = {
    week = { Label = '1 week', Days = 7 },
    month = { Label = '1 month', Days = 30 },
    permanent = { Label = 'Permanent', Permanent = true }
}
```

Minutes, hours, weeks, months and years are also supported.

## Purchase or renewal command

Use in the Tebex package:

```text
frasekill_tebex {id} month {transaction}
```

`month` must match your plan key. Renewals are added to the remaining time and each transaction is tracked separately.

## Refund or chargeback

```text
frasekill_tebex_revoke {id} {transaction}
```

This revokes only that transaction without removing other valid purchases from the same player.

## Normal expiration

Timed plans expire automatically. You do not need to run `revoke` when the paid period simply ends.

## Warnings

`Config.ExpiryNotifications` controls pre-expiration warnings. If another source such as a job or ACE still grants access, FraseKill avoids telling the player they are losing all access.
