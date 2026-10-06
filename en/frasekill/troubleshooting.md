# Troubleshooting

## `/frasekill` does not open

1. Check that the player has access.
2. If you are an admin, run `/frasekillstatus`.
3. Check F8 and the server console for an error.

## FraseKill Admin does not open

Run `/frasekilladmin`.

If you are not the owner yet, FraseKill will show the line you need to add to `server.cfg`.

## Script settings is grey/locked

**Configuration files** is selected.

Choose **Administration panel** if you want to edit settings from the UI.

## Wrong ambulance job detected

Open **Script settings → Death detection** and try **Auto** first.

If you have several medical resources installed, select the one you actually use.

## SQL problem

FraseKill prepares its tables automatically.

For servers that use a manual database setup, the resource also includes:

```text
sql/install.sql
```

## Tebex does not grant access

Make sure **Managed access + Tebex** is selected and the plan name matches your configuration.

## I changed too many settings and want to start again

Use **Restore defaults** in Script settings.

Player phrases, access grants, rules and administrators are not deleted.
