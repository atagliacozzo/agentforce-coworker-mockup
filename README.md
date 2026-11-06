# Mockup Agentforce Coworker

Mockup interattivo, in italiano, di un'app mobile di assistente digitale (Coworker). Serve per simulare in una demo come una persona fa una domanda, come l'agente cerca le informazioni (Salesforce, Slack, altri agenti) e come risponde.

È un **unico file HTML**: nessuna installazione, nessuna dipendenza, nessuna connessione. Domande, passi di ricerca, tempi, risposte, fonti e immagini si configurano da un pannello nascosto.

> Mockup dimostrativo. Tutti i nomi, i luoghi e i numeri sono fittizi. I nomi di prodotto e i marchi citati appartengono ai rispettivi proprietari.

## Avvio rapido

1. Apri `agentforce-coworker-mockup.html` in un browser (doppio clic).
2. Premi `→` per far digitare la prima domanda, poi `Invio` per inviarla.
3. Doppio clic nell'angolo in alto a destra della pagina per aprire la configurazione.

Con GitHub Pages attivo, il mockup è raggiungibile dall'indirizzo del sito (la pagina `index.html` rimanda al mockup).

## Cosa fa

- Telefono simulato con home, chat, menu laterale, domande suggerite o nascoste.
- Digitazione simulata con pause ed errori di battitura corretti; invio sempre con `Invio`.
- Fase di ricerca configurabile: passi Salesforce, Slack, altro agente, Web, con attese casuali tra minimo e massimo.
- Messaggi dell'agente formattabili (grassetto, elenchi) e mostrati una riga alla volta.
- Risposte con tabelle, citazioni numerate, fonti, immagini e domande di follow-up.
- Tornare indietro di un passo, ripartire da capo, schermo intero.
- Configurazione salvata nel browser, esportabile e importabile come file JSON.

## Scorciatoie

| Tasto | Azione |
|---|---|
| `→` | digita la prossima domanda nascosta (o riprende dopo `←`) |
| `Invio` | invia la domanda digitata |
| `←` | torna al passo precedente |
| `↓` | salta l'attesa in corso; scorre la chat quando non c'è attesa |
| `↑` | scorre la chat |
| `F` | schermo intero |
| `R` | riparte da capo |
| doppio clic in alto a destra | mostra o nasconde la configurazione |

Il [manuale](docs/manuale-agentforce-coworker-mockup.html) descrive ogni funzione e il formato del file di configurazione.

## Configurazione

Il mockup si apre con la configurazione incorporata, la stessa del file `agentforce-coworker-configurazione.json`. Dal pannello si può esportare, importare un file e ripristinare l'esempio.

La configurazione di esempio è inventata e contiene tre categorie, sei domande e una domanda nascosta (si avvia con `→`). Le immagini si indicano con il solo nome del file, nella stessa cartella dell'HTML: in `immagini-esempio/` c'è un grafico di prova.

## Struttura

```
agentforce-coworker-mockup.html          il mockup (file unico)
agentforce-coworker-configurazione.json  configurazione di esempio, importabile
index.html                               rimanda al mockup (utile con GitHub Pages)
docs/                                    manuale d'uso
immagini-esempio/                        immagine di prova
```

## Pubblicare su GitHub Pages

Impostazioni del repository, sezione Pages, sorgente "Deploy from a branch", ramo `main`, cartella `/ (root)`.
