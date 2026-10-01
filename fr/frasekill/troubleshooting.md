# Dépannage

## `/frasekill` ne s’ouvre pas

Vérifiez l’accès effectif du joueur, lancez `/frasekillstatus` en administrateur et consultez F8 ainsi que la console serveur.

## Les tables ne sont pas créées

Vérifiez que `oxmysql` démarre avant `zbrou_frasekill`. Si la création automatique est désactivée, exécutez `sql/install.sql`.

## Le panneau admin ne s’ouvre pas

Ajoutez la permission ACE correcte dans `server.cfg`, puis redémarrez la ressource.

## FraseKill reste affiché après le revive

Vérifiez `Config.Display.Mode`, l’adapter indiqué par `/frasekillstatus` et la valeur `FailsafeSeconds`.

## Tebex ne donne pas l’accès

Vérifiez `Config.Tebex.Enabled`, l’exécution du command via console/Tebex et la clé exacte du plan.

## Besoin d’aide ?

Consultez **Support** pour rejoindre le Discord officiel.
