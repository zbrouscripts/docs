# Access and Tebex

Choose who can use FraseKill.

## Access modes

### Managed access

Grant access from FraseKill Admin to players, jobs or groups.

Access can be permanent or temporary.

### Managed access + Tebex

Works like managed access and also accepts active Tebex purchases.

### Custom check

For servers that already have their own permission system and want to connect it to FraseKill.

## Tebex

Tebex is optional.

You can create plans such as:

- 1 week;
- 1 month;
- 1 year;
- permanent.

A Tebex package can use:

```text
frasekill_tebex {id} month {transaction}
```

For refunds or chargebacks:

```text
frasekill_tebex_revoke {id} {transaction}
```

Temporary purchases expire automatically. Renewals add more time to the player's existing access.
