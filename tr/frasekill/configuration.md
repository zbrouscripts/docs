# Yapılandırma

FraseKill ayarları istemciyle paylaşılan bir dosya ve yalnızca sunucuda çalışan bir dosya olarak ayırır.

## `config.lua`

Görsel ve ortak ayarları içerir. **Buraya secret, token veya webhook koymayın.**

- `Config.Debug`: canlı sunucuda `false` bırakın.
- `Config.Command` / `AdminCommand`: editör ve admin panel komutları.
- `Config.Locale`: varsayılan dil.
- `Config.MaxCharacters`: her cümle için maksimum karakter.
- `Config.DefaultSlotMode`: `fixed` seçili slotu kullanır; `random` rastgele moda izin verilen geçerli slotlar arasından seçim yapar.
- `Config.Death.Adapter = 'auto'`: mevcut entegrasyonu otomatik algılar. İsterseniz `esx_ambulancejob`, `qb-ambulancejob`, `qbx_medical` veya `standalone` zorlanabilir.

### `Config.Display.Mode`

```lua
Config.Display = {
    Mode = 'death_state', -- timed | death_state | smart
    Seconds = 10,
    MaxSeconds = 20,
    FailsafeSeconds = 120,
    MinVisibleMs = 850
}
```

- `timed`: oyuncu hâlâ ölü olsa bile `Seconds` sonunda gizler.
- `death_state`: oyuncu ölü olduğu sürece görünür ve revive olduğunda kaybolur. `FailsafeSeconds`, overlay’in ekranda takılı kalmasını önler.
- `smart`: ölüm durumunu takip eder ve ayrıca `MaxSeconds` üst sınırını uygular.

`MinVisibleMs`, metnin okunabilmesi için minimum görünme süresidir.

Aynı dosyada varsayılan görsel değerler, limitler, fontlar, animasyonlar, diller ve presetler bulunur. Canlı sunucuda `Config.Developer.Enabled = false` bırakın.

## `config_server.lua`

Bu dosya **yalnızca sunucuda** çalışır.

- `Config.Storage`: tablo, otomatik oluşturma ve kimlik türü (`license`, `character`, `custom`). `license` önerilir.
- `Config.GroupAccess`: Jobs, GuilleGangs V2, QB/Qbox gangleri ve custom gruplar. Aynı anda birden fazlası açılabilir.
- Gruplar `job:police`, `guille:ballas`, `frameworkgang:vagos` gibi namespace ile tutulur. Böylece aynı isimler karışmaz. Minimum grade için `job:police@2` kullanılabilir.
- `Config.Access.Mode`: `everyone`, `managed`, `ace` veya `custom`. VIP/ücretli erişim için `managed` önerilir.
- `Config.Admin`: admin paneli ACE ve owner ayarları.
- `Config.KillerName`: FiveM adı, karakter adı veya custom resolver.
- `Config.Moderation`: URL, yasaklı kelime ve sunucu tarafı custom doğrulama.
- `Config.Security`: kayıt/reset/admin cooldownları.
- `Config.ExpiryNotifications`: süre bitiş uyarıları.
- `Config.Logs`: logları açar; webhook URL’leri `server/webhooks.lua` içinde kalır.
- `Config.Tebex`: süreli veya kalıcı planlar.
- `Config.Diagnostics`: adminlere özel `/frasekillstatus`.
