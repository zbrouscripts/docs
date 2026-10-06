# Tebex and expirations

Tebex access is optional and server-side. Use `Config.Access.Mode = 'managed_tebex'` when you want normal managed grants **plus** active Tebex entitlements.

Enable it in `config_server.lua`:

```lua
Config.Tebex.Enabled = true
```

Example plans:

```lua
Plans = {
    week = { Label = '1 week', Days = 7 },
    month = { Label = '1 month', Days = 30 },
    year = { Label = '1 year', Days = 365 },
    permanent = { Label = 'Permanent', Permanent = true }
}
```

## Purchase / renewal

Add a Tebex Game Server Command:

```text
frasekill_tebex {id} month {transaction}
```

Use the same command for renewal. Timed renewals extend the remaining entitlement and each transaction is tracked to prevent duplicates.

## Refund / chargeback

```text
frasekill_tebex_revoke {id} {transaction}
```

Do not use revoke for a normal cancellation when paid access should continue until its end date. Timed plans expire automatically.

Tebex commands accept console execution only. FraseKill does not store a Tebex API key in the NUI.
