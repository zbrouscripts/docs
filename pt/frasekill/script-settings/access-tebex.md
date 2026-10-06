# Acesso e Tebex

## Modos de acesso

- **Acesso gerido** — acessos dados pelo FraseKill Admin a jogadores, jobs ou grupos.
- **Acesso gerido + Tebex** — inclui também compras Tebex ativas.
- **Verificação personalizada** — para servidores com o seu próprio sistema de permissões.

Os acessos podem ser permanentes ou temporários.

## Tebex

Tebex é opcional. Podes criar planos como 1 semana, 1 mês, 1 ano ou permanente.

Entrega:

```text
frasekill_tebex {id} month {transaction}
```

Reembolso/chargeback:

```text
frasekill_tebex_revoke {id} {transaction}
```

Os acessos temporários expiram automaticamente e as renovações acrescentam mais tempo.
