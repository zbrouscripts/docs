# Konfiguracja

FraseKill można skonfigurować na dwa sposoby:

- **Panel administracyjny** — najprostsza opcja.
- **Pliki konfiguracyjne** — jeśli wolisz edytować Lua.

Tryb wybierasz w **FraseKill Admin → Ustawienia skryptu**.

Panel pozwala zmienić język, kolory, domyślne wartości, wykrywanie śmierci, dostęp, Tebex, zasady i powiadomienia. Każda opcja ma `?` z prostym opisem.

## Wypróbuj panel przed konfiguracją

Otwórz **interaktywne demo Ustawień skryptu** w tym samym stylu co prawdziwy panel. Możesz sprawdzić Classic/Liquid Glass, kolory, przełączniki, listy, blokadę plików i reset.

Demo odwzorowuje prawdziwą strukturę panelu: jeden przewijany ekran, sekcje w tej samej kolejności i stały pasek akcji na dole.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=pl" %}

[**Otwórz demo na pełnym ekranie →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=pl)

{% hint style="info" %}
To tylko demo dokumentacji: nie łączy się z FiveM, SQL ani Tebex.
{% endhint %}

- `config.lua` — wygląd, język, komendy, wartości domyślne i animacje.
- `config_server.lua` — dostęp, administracja, Tebex, bezpieczeństwo i opcje serwera.
- `server/webhooks.lua` — webhooki Discord.
