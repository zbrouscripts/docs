# Fehlerbehebung

## `/frasekill` öffnet sich nicht

- Prüfe, ob der Spieler Zugriff hat.
- Als Admin: `/frasekillstatus` ausführen.
- F8 und Serverkonsole auf Fehler prüfen.

## FraseKill Admin öffnet sich nicht

Nutze `/frasekilladmin`. Wenn du noch kein Owner bist, zeigt das Script die nötige Zeile für `server.cfg`.

## Script-Einstellungen sind gesperrt

**Konfigurationsdateien** ist ausgewählt. Wähle **Adminpanel**, um im Panel zu bearbeiten.

## Falsches Ambulance-Script

Öffne **Script-Einstellungen → Todeserkennung**. Probiere zuerst **Auto** und wähle bei mehreren Medicals das richtige manuell.

## SQL-Problem

FraseKill bereitet seine Tabellen automatisch vor. Für eine manuelle Einrichtung ist `sql/install.sql` enthalten.

## Tebex gibt keinen Zugriff

Prüfe, ob **Verwalteter Zugriff + Tebex** gewählt ist und der Planname übereinstimmt.

## Alles zurücksetzen

Nutze **Standardwerte wiederherstellen**. Spielerphrasen, Zugriffe, Regeln und Admins bleiben erhalten.
