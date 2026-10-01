# Instalação

## Início rápido

1. Instala e inicia o `oxmysql`.
2. Adiciona `zbrou_frasekill` ao servidor.
3. Revê as permissões e a configuração antes de abrir o servidor ao público.
4. Adiciona ao `server.cfg`:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

5. Reinicia o recurso ou o servidor.

O FraseKill cria e migra automaticamente as tabelas quando `Config.Storage.AutoCreate = true`, que é o valor predefinido. Para uma instalação manual da base de dados, também podes executar `sql/install.sql`.

## Primeiro administrador

Executa:

```text
/frasekilladmin
```

Se ainda não tiveres permissão, o menu mostra a linha ACE exata para copiar para o `server.cfg`. Também podes adicioná-la manualmente:

```cfg
add_ace identifier.license:TUA_LICENSE zbrou.frasekill.admin allow
```

Reinicia o recurso depois de alterar permissões ACE.

## Verificação

- `/frasekill` abre o editor quando o jogador tem acesso.
- `/frasekilladmin` abre o painel de administração.
- `/frasekillstatus` mostra o diagnóstico aos administradores.

`/frasekilltest` é apenas para desenvolvimento e vem desativado na versão pública.
