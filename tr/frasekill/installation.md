# Kurulum

## Gerekenler

- FiveM sunucusu.
- Sunucuda `oxmysql` kaynağı.
- ESX, QBCore ve Qbox isteğe bağlıdır. FraseKill frameworksüz de çalışır.
- `zbrou_utils` gerekli değildir.

## Sunucuya ekleme

1. Klasörü resources içine koy ve adını `zbrou_frasekill` olarak bırak.
2. `server.cfg` içinde `oxmysql` FraseKill'den önce olmalı:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

3. Gerekli SQL ilk çalıştırmada otomatik hazırlanır. Manuel kurulum isteyenler için `sql/install.sql` dosyası da bulunur.
4. Kaynağı veya sunucuyu yeniden başlat.

## Owner erişimi

```cfg
add_ace identifier.license:LICENSE zbrou.frasekill.admin allow
```

Yetkin yoksa `/frasekilladmin` kopyalaman gereken satırı gösterebilir.

## Test aracı

`/frasekilltest` varsayılan olarak kapalıdır. `config.lua` içindeki `Config.Developer` bölümünde `Enabled = true` yap. `RequireAdmin = true` kalsın; işin bitince tekrar `Enabled = false` yap.
