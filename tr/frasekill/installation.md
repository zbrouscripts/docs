# Kurulum

## Hızlı başlangıç

1. `oxmysql` kurun ve başlatın.
2. `zbrou_frasekill` kaynağını sunucunuza ekleyin.
3. Sunucuyu oyunculara açmadan önce izinleri ve ayarları kontrol edin.
4. `server.cfg` dosyasına ekleyin:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

5. Kaynağı veya sunucuyu yeniden başlatın.

`Config.Storage.AutoCreate = true` varsayılan olarak açıktır ve FraseKill gerekli tabloları otomatik oluşturur/günceller. Manuel kurulum isterseniz `sql/install.sql` dosyasını da çalıştırabilirsiniz.

## İlk yönetici

Şunu çalıştırın:

```text
/frasekilladmin
```

Henüz izniniz yoksa menü, `server.cfg` içine kopyalamanız gereken ACE satırını gösterir. Manuel örnek:

```cfg
add_ace identifier.license:SENIN_LICENSE zbrou.frasekill.admin allow
```

ACE değişikliklerinden sonra kaynağı yeniden başlatın.

## Kontrol

- `/frasekill` erişimi olan oyuncuda editörü açar.
- `/frasekilladmin` yönetim panelini açar.
- `/frasekillstatus` yöneticilere tanılama bilgisi gösterir.

`/frasekilltest` yalnızca geliştirme içindir ve herkese açık sürümde kapalıdır.
