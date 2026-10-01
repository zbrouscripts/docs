# Rozwiązywanie problemów

## `/frasekill` nie otwiera się

Sprawdź efektywny dostęp gracza, uruchom `/frasekillstatus` jako admin oraz przejrzyj F8 i konsolę serwera.

## Tabele bazy danych nie są tworzone

Upewnij się, że `oxmysql` startuje przed `zbrou_frasekill`. Jeśli auto-tworzenie jest wyłączone, wykonaj `sql/install.sql`.

## Panel admina nie otwiera się

Dodaj poprawne uprawnienie ACE do `server.cfg` i zrestartuj zasób.

## FraseKill nie znika po revive

Sprawdź `Config.Display.Mode`, adapter pokazany przez `/frasekillstatus` oraz `FailsafeSeconds`.

## Tebex nie nadaje dostępu

Sprawdź `Config.Tebex.Enabled`, czy komenda jest wykonywana z konsoli/Tebex oraz czy klucz planu jest identyczny z konfiguracją.

## Pomoc

Otwórz stronę **Wsparcie**, aby dołączyć do oficjalnego Discorda.
