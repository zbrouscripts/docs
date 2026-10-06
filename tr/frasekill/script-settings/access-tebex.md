# Erişim ve Tebex

Erişim modları:

- **Yönetilen erişim**
- **Yönetilen erişim + Tebex**
- **Özel kontrol**

Erişim kalıcı veya süreli olabilir.

Tebex isteğe bağlıdır.

```text
frasekill_tebex {id} month {transaction}
```

İade/chargeback:

```text
frasekill_tebex_revoke {id} {transaction}
```

Süreli erişimler otomatik biter, yenilemeler mevcut süreye eklenir.
