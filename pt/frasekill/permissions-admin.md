# Permissões e administração

Use `/frasekilladmin` para abrir o painel. A proteção recomendada é ACE:

```cfg
add_ace identifier.license:TUA_LICENSE zbrou.frasekill.admin allow
```

Sem permissão, o próprio menu mostra a linha ACE pronta para copiar. Em **Acessos** podes dar permissões permanentes ou temporárias por jogador e gerir Jobs/grupos ativados em `Config.GroupAccess`. Em **Frases** podes pesquisar jogadores, abrir detalhes, editar presets, restaurar/eliminar configurações, dar ou retirar acesso, guardar notas internas e enviar mensagens a jogadores online. Todas as ações importantes são validadas no servidor.
