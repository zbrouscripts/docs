# Accès et Tebex

Modes disponibles :

- **Accès géré**
- **Accès géré + Tebex**
- **Vérification personnalisée**

Les accès peuvent être permanents ou temporaires.

Tebex est optionnel. Commande de livraison :

```text
frasekill_tebex {id} month {transaction}
```

Pour un remboursement/chargeback :

```text
frasekill_tebex_revoke {id} {transaction}
```

Les accès temporaires expirent automatiquement et les renouvellements ajoutent du temps.
