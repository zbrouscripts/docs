# Actualización

Esta documentación corresponde a **zbrou_frasekill v1.0.0-glass-prototype.20**.

## Procedimiento seguro

1. Haz copia del recurso y la base de datos.
2. Sustituye el recurso `zbrou_frasekill` completo por la nueva build.
3. Usa los nuevos `config.lua` y `config_server.lua` y copia solo tus valores personalizados; no pises los archivos nuevos con configs antiguas.
4. Conserva tus valores privados de `server/webhooks.lua`.
5. Conserva `web/logo.png` si ya tienes tu logo.
6. Inicia `oxmysql`, reinicia FraseKill y vuelve a entrar.

Con `Config.Storage.AutoCreate = true` las tablas/migraciones necesarias se crean sin borrar perfiles, accesos, normas ni admins. Si desactivas el auto-SQL, revisa `sql/`.

Las versiones recientes añaden Ajustes del script, admins delegados, idiomas, colores de branding, más adapters de ambulance y Restablecer predeterminado. No copies un `web/` o configs antiguos encima de la build nueva.
