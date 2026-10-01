# İzinler ve yönetim

Paneli `/frasekilladmin` ile açın. Önerilen koruma ACE’dir:

```cfg
add_ace identifier.license:SENIN_LICENSE zbrou.frasekill.admin allow
```

İzniniz yoksa FraseKill kopyalamanız gereken ACE satırını otomatik gösterir. **Erişim** bölümünde kalıcı/süreli oyuncu erişimleri ve `Config.GroupAccess` ile açık olan Job/gruplar yönetilir. **FraseKill** bölümünde oyuncu arama, detay açma, preset düzenleme, sıfırlama/silme, erişim verme/kaldırma, iç not ve online mesaj işlemleri yapılabilir. Önemli tüm işlemler sunucuda tekrar doğrulanır.
