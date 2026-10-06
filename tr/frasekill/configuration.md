# Yapılandırma

FraseKill iki şekilde ayarlanabilir:

- **Yönetim paneli** — en kolay yöntem.
- **Yapılandırma dosyaları** — Lua dosyalarını düzenlemek isteyenler için.

Modu **FraseKill Admin → Script ayarları** bölümünden seç.

Panelden dil, renkler, varsayılanlar, ölüm algılama, erişim, Tebex, kurallar ve bildirimler değiştirilebilir. Her seçeneğin yanında basit açıklama gösteren bir `?` vardır.

## Yapılandırmadan önce paneli dene

Gerçek panelle aynı görsel stile sahip **etkileşimli Script ayarları demosunu** aç. Classic/Liquid Glass, renkler, switchler, menüler, dosya kilidi ve varsayılanlara dönüşü deneyebilirsin.

Demo gerçek panel yapısını takip eder: tek bir kaydırılabilir ekran, aynı sıradaki bloklar ve altta sabit işlem çubuğu.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=tr" %}

[**Tam ekran demoyu aç →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=tr)

{% hint style="info" %}
Bu yalnızca dokümantasyon demosudur; FiveM, SQL veya Tebex'e bağlanmaz.
{% endhint %}

- `config.lua` — görünüm, dil, komutlar, varsayılanlar ve animasyonlar.
- `config_server.lua` — erişim, yönetim, Tebex, güvenlik ve sunucu ayarları.
- `server/webhooks.lua` — Discord webhookları.
