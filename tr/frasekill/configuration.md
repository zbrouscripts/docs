# Yapılandırma

FraseKill iki şekilde yapılandırılabilir: **görsel Script ayarları panelinden**, yani `config.lua` ve `config_server.lua` içindeki çoğu ayarı kod düzenlemeden değiştirebilirsin, ya da bu dosyaları doğrudan düzenleyebilirsin.

Webhooklar ve bazı hassas seçenekler gibi özel ayarlar yalnızca kaynak dosyalarında kalır.

## Görsel yapılandırma paneli

Bu, FraseKill Admin içinde göreceğin panelin aynı yapısını kullanır. Sunucunda değişiklik yapmadan önce burada deneyebilirsin.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=tr" %}

[**Yapılandırma panelini tam ekran aç →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=tr)

{% hint style="info" %}
Demo FiveM, SQL veya Tebex'e bağlanmaz ve sunucuda hiçbir değişiklik yapmaz.
{% endhint %}

## Dosyalardan yapılandırma

- `config.lua` — dil, görünüm, komutlar, varsayılanlar, animasyonlar ve görsel davranış.
- `config_server.lua` — erişim, yönetim, Tebex, güvenlik ve sunucu seçenekleri.
- `server/webhooks.lua` — Discord webhookları.

{% hint style="info" %}
Çok tecrübeli değilsen normal ayarlar için **görsel paneli** kullanman en kolay seçenektir.
{% endhint %}
