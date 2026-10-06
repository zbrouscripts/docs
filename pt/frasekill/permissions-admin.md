# Permissões e administração

## Owner principal

O owner tem acesso completo ao FraseKill Admin.

Adiciona uma única linha ao `server.cfg`:

```cfg
add_ace identifier.license:TUA_LICENSE zbrou.frasekill.admin allow
```

Se não souberes a tua license, entra no servidor e usa `/frasekilladmin`. O próprio script mostra a linha exata.

## Adicionar administradores

Não precisas de criar mais ACE.

O owner pode criar administradores no painel e escolher o que cada um pode fazer: ver jogadores, gerir acessos, editar/restaurar FraseKill, gerir regras e alterar as definições do script.

Ser administrador não dá automaticamente acesso para usar FraseKill como jogador.

## Acesso de jogadores

Pode ser permanente ou por horas, dias, semanas, meses ou anos. Também podes dar acesso a jobs ou grupos.

Para Tebex, consulta **Definições do script → Acesso e Tebex**.
