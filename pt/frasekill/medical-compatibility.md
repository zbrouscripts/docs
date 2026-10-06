# Compatibilidade médica

Na maioria dos servidores podes deixar **Auto**. FraseKill deteta o ambulance compatível que estiver iniciado.

Compatibilidade incluída com Wasabi V1/V2, Brutal, ARS, TK, Qbox, QB, AS, Sky, AK47, P Ambulance, standalone e **ESX Ambulance Job clássico, versões antigas/1.2 e Legacy atual**.

## ESX Ambulance Job

São suportadas as rotas usadas ao longo das versões: estado numérico/booleano, `esx:onPlayerDeath`, spawn/revive e o estado das versões Legacy atuais.

Em versões antigas com um único estado inconsciente/morto, usa **Deteção de morte → Incapacitado**.

A validação final continua no servidor; um estado enviado pelo cliente sozinho não é aceite como prova de morte. Forks privados podem usar a verificação server-side personalizada.
