# Yetkiler ve yönetim

## Ana owner

Owner, FraseKill Admin üzerinde tam yetkiye sahiptir.

`server.cfg` içine tek satır ekle:

```cfg
add_ace identifier.license:LICENSE zbrou.frasekill.admin allow
```

License değerini bilmiyorsan sunucuda `/frasekilladmin` kullan. FraseKill kopyalaman gereken satırı gösterir.

## Başka adminler eklemek

Başka ACE satırları gerekmez.

Owner panelden admin oluşturur ve her birinin yetkilerini seçer: oyuncuları görmek, erişim vermek/kaldırmak, FraseKill düzenlemek/sıfırlamak, kuralları yönetmek ve Script ayarlarını değiştirmek.

Admin olmak oyuncu olarak FraseKill kullanma erişimi vermez.

## Oyuncu erişimi

Erişim kalıcı veya süreli olabilir. Job ve gruplara da erişim verilebilir.

Tebex için **Script ayarları → Erişim ve Tebex** bölümüne bak.
