# Konfiguracja

FraseKill można skonfigurować na dwa sposoby: przez **wizualny panel Ustawień skryptu**, który pozwala zmienić większość opcji z `config.lua` i `config_server.lua` bez edycji kodu, albo bezpośrednio w tych plikach.

Niektóre prywatne opcje, takie jak webhooki i ustawienia wrażliwe, pozostają tylko w plikach zasobu.

## Wizualny panel konfiguracji

To ten sam typ panelu, który znajdziesz w FraseKill Admin. Możesz go wypróbować tutaj przed zmianą czegokolwiek na serwerze.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=pl" %}

[**Otwórz panel konfiguracji na pełnym ekranie →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=pl)

{% hint style="info" %}
Demo nie łączy się z FiveM, SQL ani Tebex i nie wprowadza zmian na serwerze.
{% endhint %}

## Konfiguracja przez pliki

- `config.lua` — język, wygląd, komendy, wartości domyślne, animacje i zachowanie interfejsu.
- `config_server.lua` — dostęp, administracja, Tebex, bezpieczeństwo i opcje serwera.
- `server/webhooks.lua` — webhooki Discord.

{% hint style="info" %}
Jeśli nie masz dużego doświadczenia, użyj **wizualnego panelu** do normalnych ustawień i edytuj pliki tylko wtedy, gdy jest to potrzebne.
{% endhint %}
