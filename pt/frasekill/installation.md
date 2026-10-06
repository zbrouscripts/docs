# Instalação

## O que precisas

- Um servidor FiveM.
- O recurso `oxmysql` no servidor.
- ESX, QBCore e Qbox são opcionais. FraseKill também funciona sem framework.
- `zbrou_utils` não é necessário.

## Adicionar FraseKill ao servidor

1. Coloca a pasta nos recursos e mantém o nome `zbrou_frasekill`.
2. No `server.cfg`, confirma que `oxmysql` aparece antes de FraseKill:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

3. A SQL necessária é preparada automaticamente na primeira vez que FraseKill inicia. O ficheiro `sql/install.sql` também está incluído caso prefiras prepará-la manualmente.
4. Reinicia o recurso ou o servidor.

## Dar acesso ao owner

```cfg
add_ace identifier.license:TUA_LICENSE zbrou.frasekill.admin allow
```

Se executares `/frasekilladmin` sem permissão, o próprio script mostra a linha exata que deves copiar.

## Testar durante a configuração

`/frasekilltest` vem desativado na versão pública.

Em `config.lua`, procura `Config.Developer` e muda apenas:

```lua
Enabled = true
```

Mantém `RequireAdmin = true`. Quando terminares, volta a deixar `Enabled = false`.
