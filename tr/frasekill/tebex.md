# Tebex ve süre sonları

`config_server.lua` içinde `Config.Tebex.Enabled = true` yapın ve dakika, saat, gün, hafta, ay, yıl veya kalıcı planlar oluşturun.

Satın alma/yenileme:
```text
frasekill_tebex {id} month {transaction}
```

Belirli işlem için iade/chargeback:
```text
frasekill_tebex_revoke {id} {transaction}
```

Yenilemeler kalan sürenin üzerine eklenir ve her işlem ayrı tutulur. Süreli planlar otomatik biter. `Config.ExpiryNotifications` bitiş uyarılarını yönetir.
