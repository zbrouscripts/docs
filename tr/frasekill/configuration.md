# Yapılandırma

FraseKill, **görsel Script ayarları panelinden** veya doğrudan `config.lua` ve `config_server.lua` dosyalarından yapılandırılabilir.

## Görsel yapılandırma paneli

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=tr" %}

[**Yapılandırma panelini tam ekran aç →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=tr)

Panel çoğu normal ayarı kod düzenlemeden değiştirmeni sağlar. Özel ayarlar kaynak dosyalarında kalır.

## Yapılandırma dosyaları

- `config.lua` — dil, görünüm, komutlar ve varsayılan değerler.
- `config_server.lua` — erişim, yönetim, Tebex, güvenlik ve sunucu ayarları.
- `server/webhooks.lua` — Discord webhookları.

## Yetkiler ve yönetim

Ana owner'ı `server.cfg` içine ekle:

```cfg
add_ace identifier.license:LICENSE zbrou.frasekill.admin allow
```

License değerini bilmiyorsan `/frasekilladmin` kullan.

Diğer adminler panelden ayrı yetkilerle oluşturulur. Admin olmak oyuncu olarak FraseKill erişimi vermez.
