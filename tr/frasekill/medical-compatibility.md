# Medical uyumluluğu

Çoğu sunucuda **Auto** bırakabilirsin. FraseKill çalışan uyumlu ambulance kaynağını algılar.

Wasabi V1/V2, Brutal, ARS, TK, Qbox, QB, AS, Sky, AK47, P Ambulance, standalone ve **klasik/eski/1.2 dönemi ESX Ambulance Job ile güncel ESX Legacy** desteklenir.

## ESX Ambulance Job

Sayısal/boolean ölüm durumu, `esx:onPlayerDeath`, spawn/revive akışları ve güncel Legacy state desteği bulunur.

Tek bir baygın/ölü durumu kullanan eski ESX sürümlerinde **Ölüm algılama → Incapacitated** kullan.

Son doğrulama sunucuda yapılır. Yalnızca client tarafından gelen bir durum ölüm kanıtı olarak kabul edilmez. Özel forklar server-side custom check kullanabilir.
