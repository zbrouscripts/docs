# Uprawnienia i administracja

Panel otwiera komenda `/frasekilladmin`. Zalecana ochrona to ACE:

```cfg
add_ace identifier.license:TWOJA_LICENSE zbrou.frasekill.admin allow
```

Bez uprawnienia FraseKill pokaże gotową linię ACE do skopiowania. W **Dostępach** można zarządzać stałymi i czasowymi uprawnieniami graczy oraz Jobami/grupami włączonymi w `Config.GroupAccess`. W **Frazach** można wyszukiwać graczy, otwierać szczegóły, edytować presety, resetować/usuwać konfiguracje, nadawać/odbierać dostęp, zapisywać notatki wewnętrzne i wysyłać wiadomości graczom online. Ważne akcje są ponownie weryfikowane po stronie serwera.
