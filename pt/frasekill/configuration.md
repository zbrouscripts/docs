# Configuração

FraseKill pode ser configurado de duas formas:

- **Painel de administração**, a opção mais simples se não quiseres editar ficheiros.
- **Ficheiros de configuração**, se preferires manter tudo em Lua.

Escolhe o modo em **FraseKill Admin → Definições do script**.

## Painel de administração

Permite alterar visualmente idioma, cores, valores predefinidos, deteção de morte, acesso, Tebex, regras e notificações.

Cada opção tem um `?` com uma explicação simples.

## Experimenta o painel antes de configurar

Abre uma **demo interativa das Definições do script** com o mesmo estilo visual do painel real. Podes testar Classic/Liquid Glass, cores, switches, listas, bloqueio por ficheiros e Restaurar predefinições.

A demo segue a estrutura real do painel: um único ecrã com scroll, blocos pela mesma ordem e a barra de ações fixa em baixo.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=pt" %}

[**Abrir demo em ecrã inteiro →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=pt)

{% hint style="info" %}
É apenas uma demo da documentação: não se liga a FiveM, SQL ou Tebex.
{% endhint %}

## Ficheiros

- `config.lua` — idioma, aparência, comandos, valores predefinidos, animações e comportamento visual.
- `config_server.lua` — acesso, administração, Tebex, segurança e opções internas.
- `server/webhooks.lua` — webhooks do Discord.

{% hint style="info" %}
Se não tens muita experiência, usa o **Painel de administração** para as opções normais.
{% endhint %}
