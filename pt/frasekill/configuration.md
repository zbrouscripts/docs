# Configuração

FraseKill pode ser configurado de duas formas: através do **painel visual das Definições do script**, que permite alterar a maioria das opções de `config.lua` e `config_server.lua` sem editar código, ou diretamente nesses ficheiros.

Algumas opções privadas, como webhooks e definições sensíveis, ficam apenas nos ficheiros do recurso.

## Painel visual de configuração

Este é o mesmo tipo de painel disponível dentro do FraseKill Admin. Podes experimentá-lo aqui antes de alterar o teu servidor.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=pt" %}

[**Ver painel de configuração em ecrã inteiro →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=pt)

{% hint style="info" %}
A demo não se liga a FiveM, SQL ou Tebex e não guarda alterações no servidor.
{% endhint %}

## Configurar através dos ficheiros

- `config.lua` — idioma, aparência, comandos, valores predefinidos, animações e comportamento visual.
- `config_server.lua` — acessos, administração, Tebex, segurança e opções do servidor.
- `server/webhooks.lua` — webhooks do Discord.

{% hint style="info" %}
Se não tens muita experiência, usa o **painel visual** para os ajustes normais e edita os ficheiros apenas quando necessário.
{% endhint %}
