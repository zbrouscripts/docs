# Configuração

O FraseKill separa as opções em dois ficheiros: um partilhado com o cliente e outro exclusivo do servidor.

## `config.lua`

Contém opções visuais e partilhadas. **Nunca coloques segredos, tokens ou webhooks aqui.**

- `Config.Debug`: mantém `false` em produção.
- `Config.Command` / `AdminCommand`: comandos do editor e do painel admin.
- `Config.Locale`: idioma inicial.
- `Config.MaxCharacters`: limite máximo de caracteres de cada frase.
- `Config.DefaultSlotMode`: `fixed` usa o slot selecionado; `random` escolhe entre slots válidos ativados para aleatório.
- `Config.Death.Adapter = 'auto'`: deteta automaticamente a integração disponível; também pode ser forçado para `esx_ambulancejob`, `qb-ambulancejob`, `qbx_medical` ou `standalone`.

### `Config.Display.Mode`

```lua
Config.Display = {
    Mode = 'death_state', -- timed | death_state | smart
    Seconds = 10,
    MaxSeconds = 20,
    FailsafeSeconds = 120,
    MinVisibleMs = 850
}
```

- `timed`: esconde após `Seconds`, mesmo que o jogador continue morto.
- `death_state`: mantém a FraseKill enquanto o jogador estiver morto e esconde ao reviver. `FailsafeSeconds` evita que fique presa no ecrã.
- `smart`: segue o estado de morte, mas também aplica `MaxSeconds` como limite máximo.

`MinVisibleMs` garante um tempo mínimo de leitura.

O mesmo ficheiro inclui valores visuais, limites, fontes, animações, idiomas e presets predefinidos. `Config.Developer.Enabled` deve ficar `false` em produção.

## `config_server.lua`

É executado **apenas no servidor** e contém tudo o que não deve ser enviado ao cliente.

- `Config.Storage`: tabela, criação automática e identificador (`license`, `character` ou `custom`). `license` é recomendado.
- `Config.GroupAccess`: Jobs, GuilleGangs V2, gangs QB/Qbox e grupos custom. Podem ser combinados.
- Os grupos usam namespaces como `job:police`, `guille:ballas` e `frameworkgang:vagos`, evitando colisões. Pode usar grau mínimo, por exemplo `job:police@2`.
- `Config.Access.Mode`: `everyone`, `managed`, `ace` ou `custom`. `managed` é recomendado para acesso VIP/pago.
- `Config.Admin`: ACE e owners do painel de administração.
- `Config.KillerName`: nome FiveM, nome do personagem ou resolver custom.
- `Config.Moderation`: bloqueio de URLs, palavras e validação custom server-side.
- `Config.Security`: cooldowns de gravação/reset/admin.
- `Config.ExpiryNotifications`: avisos antes da expiração.
- `Config.Logs`: ativa os logs; os webhooks ficam em `server/webhooks.lua`.
- `Config.Tebex`: planos temporários ou permanentes.
- `Config.Diagnostics`: comando `/frasekillstatus` para admins.
