# privacy-informativa-mcp-info
privacy-informativa-mcp-info 
# privacy-informativa-mcp

Plugin MCP (Model Context Protocol) gratuito per Claude che aiuta chiunque
riceva un'informativa privacy a capirla davvero: quali dati vengono
trattati, per quali finalità, con quale base giuridica, per quanto tempo,
e a chi vengono comunicati — spiegato in linguaggio semplice, non in
legalese.

**Non è un tool per il titolare del trattamento**: è pensato dal punto
di vista di chi riceve un'informativa e vuole capirla.

> Il codice sorgente di questo progetto non è pubblico. Questa pagina
> descrive solo cosa fa il plugin e come collegarlo al proprio Claude.

## Cosa fa

Due funzionalità principali:

1. **Analizza un'informativa privacy** — capisci finalità, dati trattati,
   basi giuridiche, destinatari e tempi di conservazione, presentati in
   modo chiaro invece che come un muro di testo legale. Segnala anche il
   linguaggio vago/circolare tipico di molte informative ("trattiamo i
   tuoi dati con la massima cura e trasparenza" — frasi che suonano bene
   ma non dicono nulla di concreto).
2. **Verifica la coerenza tecnica** — controlla se quello che un sito
   dichiara nella sua informativa corrisponde a quello che fa davvero
   tecnicamente (tracker, pubblicità, analytics effettivamente presenti
   nella pagina), segnalando le mancanze.

Puoi fornire l'informativa in diversi modi: testo incollato, PDF o
screenshot caricato, link diretto, o semplicemente l'indirizzo del sito.

## Come usarlo

Nessuna installazione necessaria — basta collegare Claude al servizio già
online.

1. Su [claude.ai](https://claude.ai): **Impostazioni** → **Connettori**
   (in inglese "Customize" → "Connectors")
2. Clicca **"+"** → **Aggiungi connettore personalizzato**
   ("Add custom connector")
3. Incolla questo indirizzo:
   ```
   https://privacy-informativa-mcp.onrender.com/mcp
   ```
4. Nessuna autenticazione richiesta: lascia vuoto "Advanced settings"
5. Clicca **"Aggiungi"**, poi attivalo nella chat (pulsante **"+"** in
   basso a sinistra → **"Connettori"**)

Funziona su Claude.ai, Claude Desktop, Cowork e le app mobile.

**Nota sui tempi di risposta**: il servizio gira su un piano gratuito e
si "addormenta" dopo un periodo di inattività — la prima richiesta dopo
una pausa può richiedere 30-60 secondi. Le richieste successive sono
immediate.

Nota: gli utenti su piano gratuito di Claude possono aggiungere un solo
connettore personalizzato; Pro/Max/Team/Enterprise ne supportano più
di uno.

## Limiti, dichiarati apertamente

- La verifica di coerenza tecnica analizza il codice HTML statico della
  pagina: non vede tracker caricati dinamicamente via JavaScript dopo il
  caricamento (es. dopo il consenso cookie). I risultati sono un limite
  inferiore delle terze parti realmente presenti, non un elenco
  definitivo.
- Non è configurato per cercare l'informativa privacy di un organizzazione a partire dal solo nome:
  serve almeno il sito o il link diretto all'informativa.
- **Non fornisce consulenza legale.** Aiuta a leggere un documento e a
  raccogliere informazioni; qualunque azione formale (reclamo, diffida)
  va valutata con un professionista se la posta in gioco lo richiede.
- Progetto indipendente, **non affiliato** con il Garante per la
  protezione dei dati personali né con alcuna autorità di controllo.

## Domande o problemi?

Apri una issue su questo stesso repository, oppure contatta l'autore.

## Licenza d'uso

Il servizio è gratuito e liberamente utilizzabile da chiunque tramite
Claude. Il codice sorgente resta privato.
