# Fehlerbehebung

## `/frasekill` öffnet sich nicht

Prüfe den effektiven Zugriff des Spielers, führe `/frasekillstatus` als Admin aus und kontrolliere F8 sowie die Serverkonsole.

## Tabellen werden nicht erstellt

Stelle sicher, dass `oxmysql` vor `zbrou_frasekill` startet. Bei deaktivierter Auto-Erstellung kann `sql/install.sql` manuell ausgeführt werden.

## Admin-Panel öffnet sich nicht

Füge die korrekte ACE-Berechtigung in `server.cfg` ein und starte die Ressource neu.

## FraseKill bleibt nach dem Revive sichtbar

Prüfe `Config.Display.Mode`, den Adapter aus `/frasekillstatus` und `FailsafeSeconds`.

## Tebex gewährt keinen Zugriff

Prüfe `Config.Tebex.Enabled`, dass der Befehl über Konsole/Tebex läuft und dass der Plan-Key exakt stimmt.

## Hilfe

Öffne **Support**, um dem offiziellen Discord beizutreten.
