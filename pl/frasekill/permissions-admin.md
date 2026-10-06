# Uprawnienia i administracja

## Główny owner

Owner ma pełny dostęp do FraseKill Admin.

Dodaj tylko jedną linię do `server.cfg`:

```cfg
add_ace identifier.license:TWOJA_LICENSE zbrou.frasekill.admin allow
```

Jeśli nie znasz swojej license, użyj `/frasekilladmin`. FraseKill pokaże dokładną linię do skopiowania.

## Dodawanie administratorów

Nie potrzebujesz kolejnych ACE.

Owner tworzy administratorów w panelu i wybiera ich uprawnienia: podgląd graczy, zarządzanie dostępem, edycja/reset FraseKill, zasady i ustawienia skryptu.

Bycie administratorem nie daje automatycznie dostępu do FraseKill jako gracz.

## Dostęp graczy

Może być stały lub czasowy. Dostęp można też przyznać jobom lub grupom.

Dla Tebex zobacz **Ustawienia skryptu → Dostęp i Tebex**.
