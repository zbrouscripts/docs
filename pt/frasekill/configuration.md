# Configuração

FraseKill pode ser configurado através do **painel visual das Definições do script** ou diretamente em `config.lua` e `config_server.lua`.

## Painel visual de configuração

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=pt" %}

[**Ver painel de configuração em ecrã inteiro →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=pt)

O painel permite alterar a maioria das opções habituais sem editar código. As opções privadas ficam nos ficheiros do recurso.

## Ficheiros de configuração

- `config.lua` — idioma, aparência, comandos e valores predefinidos.
- `config_server.lua` — acessos, administração, Tebex, segurança e opções do servidor.
- `server/webhooks.lua` — webhooks do Discord.

## Permissões e administração

Adiciona o owner principal em `server.cfg`:

```cfg
add_ace identifier.license:TUA_LICENSE zbrou.frasekill.admin allow
```

Se não souberes a tua license, usa `/frasekilladmin`.

Os restantes administradores são criados no painel com permissões separadas. Ser administrador não dá automaticamente acesso de jogador ao FraseKill.
