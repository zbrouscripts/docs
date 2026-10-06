# Updating

This documentation targets **zbrou_frasekill v1.0.0-glass-prototype.20**.

## Safe update procedure

1. Back up the resource and database.
2. Replace the complete `zbrou_frasekill` resource with the new build.
3. Start from the new `config.lua` and `config_server.lua`; copy only your custom values into them instead of overwriting new files with old configs.
4. Preserve your private `server/webhooks.lua` values.
5. Keep your custom `web/logo.png` if required.
6. Start `oxmysql` first, restart FraseKill and reconnect.

With `Config.Storage.AutoCreate = true`, required tables/migrations are created without deleting player profiles, access grants, rules or administrators. If automatic SQL changes are disabled, review the files in `sql/`.

## From older builds

Recent versions add Script settings, delegated admins, extra languages, branding colours, expanded ambulance adapters and a global Restore defaults button. Do not copy an old `web/` folder or old configuration files over the new build, or you will remove these features.
