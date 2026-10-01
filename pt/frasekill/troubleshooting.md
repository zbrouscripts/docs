# Resolução de problemas

## `/frasekill` não abre

Confirma o acesso efetivo do jogador, executa `/frasekillstatus` como admin e verifica o F8 e a consola do servidor.

## As tabelas não são criadas

Garante que `oxmysql` inicia antes de `zbrou_frasekill`. Se a criação automática estiver desativada, executa `sql/install.sql`.

## O painel admin não abre

Adiciona a permissão ACE correta ao `server.cfg` e reinicia o recurso.

## FraseKill não desaparece após revive

Revê `Config.Display.Mode`, o adapter mostrado por `/frasekillstatus` e `FailsafeSeconds`.

## Tebex não concede acesso

Confirma `Config.Tebex.Enabled`, que o comando é executado por consola/Tebex e que a chave do plano está correta.

## Ajuda

Abre **Suporte** para entrar no Discord oficial.
