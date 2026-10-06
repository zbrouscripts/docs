# Berechtigungen und Administration

## Haupt-Owner

Der Owner hat vollständigen Zugriff auf FraseKill Admin.

Füge nur eine Zeile in `server.cfg` ein:

```cfg
add_ace identifier.license:DEINE_LICENSE zbrou.frasekill.admin allow
```

Wenn du deine License nicht kennst, nutze `/frasekilladmin`. FraseKill zeigt dir die genaue Zeile zum Kopieren.

## Weitere Administratoren

Weitere ACE-Zeilen sind nicht nötig.

Der Owner erstellt Admins im Panel und entscheidet, was sie dürfen: Spieler ansehen, Zugriff verwalten, FraseKill bearbeiten/zurücksetzen, Regeln verwalten und Script-Einstellungen ändern.

Admin-Rechte geben nicht automatisch Spielerzugriff auf FraseKill.

## Spielerzugriff

Zugriff kann dauerhaft oder zeitlich begrenzt sein. Jobs und Gruppen können ebenfalls Zugriff erhalten.

Für Tebex siehe **Script-Einstellungen → Zugriff und Tebex**.
