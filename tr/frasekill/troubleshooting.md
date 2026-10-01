# Sorun giderme

## `/frasekill` açılmıyor

Oyuncunun etkin erişimini kontrol edin, admin olarak `/frasekillstatus` çalıştırın ve F8 ile sunucu konsolunu inceleyin.

## Veritabanı tabloları oluşmuyor

`oxmysql` kaynağının `zbrou_frasekill` öncesinde başladığını kontrol edin. Otomatik oluşturma kapalıysa `sql/install.sql` çalıştırın.

## Admin paneli açılmıyor

Doğru ACE iznini `server.cfg` içine ekleyin ve kaynağı yeniden başlatın.

## Revive sonrası FraseKill kaybolmuyor

`Config.Display.Mode`, `/frasekillstatus` tarafından gösterilen adapter ve `FailsafeSeconds` değerini kontrol edin.

## Tebex erişim vermiyor

`Config.Tebex.Enabled`, komutun konsol/Tebex üzerinden çalıştığı ve plan anahtarının birebir doğru olduğu kontrol edilmelidir.

## Yardım

Resmi Discord için **Destek** sayfasını açın.
