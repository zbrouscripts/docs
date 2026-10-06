# Compatibilità medica

Nella maggior parte dei server puoi lasciare **Auto**. FraseKill rileva la risorsa ambulance compatibile in esecuzione.

Sono supportati Wasabi V1/V2, Brutal, ARS, TK, Qbox, QB, AS, Sky, AK47, P Ambulance, standalone e **ESX Ambulance Job classico, versioni vecchie/1.2 e Legacy attuale**.

## ESX Ambulance Job

FraseKill supporta i flussi usati nelle diverse generazioni: stato numerico/booleano, `esx:onPlayerDeath`, spawn/revive e lo stato Legacy moderno.

Con vecchie versioni ESX che usano un solo stato incosciente/morto, usa **Rilevamento morte → Incapacitated**.

La verifica finale resta server-side. Uno stato inviato dal client da solo non è considerato prova della morte. I fork privati possono usare il controllo server-side personalizzato.
