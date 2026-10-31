# Protocollo di generazione e selezione

[← Torna al README](../README.md)

Come generare, valutare e ammettere le domande nell'archivio. Per la scrittura vedi [Linee guida di scrittura](linee-guida.md); per le dirette vedi [Live](live.md).

## Indice

- [Qualità prima, distribuzione dinamica dopo](#qualità-prima-distribuzione-dinamica-dopo)
- [Protocollo di generazione e controllo](#protocollo-di-generazione-e-controllo)
- [Motivazioni delle scelte editoriali](#motivazioni-delle-scelte-editoriali)

---

## Qualità prima, distribuzione dinamica dopo

**Regola fondamentale:** non fissare un numero obbligatorio di domande per categoria, macrotema o intensità. L'obiettivo è **massimizzare il numero di dilemmi memorabili**, non raggiungere quote prestabilite. È meglio pubblicare 30 domande eccellenti in `sports` che arrivare a 100 aggiungendo riempitivi; è accettabile avere più domande `social` o `love` se sono originali e affrontano conflitti diversi.

La strategia si articola in quattro passaggi:

1. **Generazione creativa:** proporre scenari attraverso macrotemi, meccanismi, ambientazioni e toni differenti. Le categorie sottorappresentate sono spunti di esplorazione, non obblighi quantitativi.
2. **Selezione qualitativa:** verificare prima i vincoli tecnici e i requisiti editoriali indispensabili, poi valutare i candidati con la griglia descritta nel protocollo. Le domande deboli si riscrivono o si scartano; non entrano solo per completare una quota.
3. **Analisi della varietà:** controllare la distribuzione per **tema**, **meccanismo** e **reazione emotiva**, oltre che per categoria e intensità. Identificare le famiglie semantiche abusate (es. ex, chat divulgate, genitori che scoprono segreti).
4. **Espansione mirata:** cercare *nuove idee* negli ambiti poco rappresentati e sottoporle agli stessi criteri; se non superano la selezione, restano fuori.

**Nessuna quota fissa nemmeno per `light` e `tough`:** esiste però un **obiettivo di copertura temporale per ogni live**, indipendente dalla distribuzione delle categorie. Serve una selezione utilizzabile in diretta, con ritmo adattabile. Una categoria non è carente solo perché ha meno righe: è carente quando manca un tipo di esperienza o quando le domande diventano ripetitive.

**Tre dimensioni della varietà:**

| Dimensione | Domanda di controllo | Esempio di saturazione da evitare |
| --- | --- | --- |
| Tematica | *Di cosa parla?* | Quasi tutte le domande `love` parlano di ex |
| Meccanica | *Perché è difficile scegliere?* | Quasi tutte contrappongono due figuracce pubbliche |
| Emotiva | *Che reazione provoca?* | Solo imbarazzo, mai comicità, sorpresa o riflessione |

**Importante:** qualità e varietà sono obiettivi complementari. La varietà non giustifica domande mediocri; la qualità isolata non giustifica un archivio monotono. Se una famiglia di dilemmi è satura, cercare un *nuovo conflitto*, non soltanto sinonimi o protagonisti diversi.

---

## Protocollo di generazione e controllo

Questa sezione traduce le linee guida in passaggi ripetibili quando si generano centinaia di domande.

### Preparazione e varietà

**Pianificazione delle sessioni:** costruire un pool di almeno 200 domande approvate (160 principali e 40 di riserva) come riferimento iniziale per due ore, dopo aver stimato il ritmo. Non confondere il target di copertura con quote per categoria o con l’obbligo di approvare domande deboli.

1. Partire da **idee e conflitti**, distribuendo *macrotemi*, *meccanismi*, *caratteri* e ambientazioni. Assegnare la categoria tecnica in base al contenuto; non generare un numero prestabilito di righe per ciascuna categoria. Se un tema è povero, cercare nuove prospettive, non riempitivi.
2. Generare due alternative **autonome e bilanciate**. Ogni opzione deve contenere soggetto, azione e conseguenza sufficienti a comprenderla senza l'altra; non ripetere parole inutili.
3. Fare un **test di simmetria**: invertendo A e B, il dilemma deve funzionare lo stesso. Se una delle due vince quasi sempre, rivedere costo, probabilità, durata o posta in gioco.
4. Verificare l'**assenza di scappatoie**: domande a scelta fittiziamente obbligata, ma facoltà reale del pubblico di passare. Esplicitare condizioni rilevanti anziché lasciar intendere scorciatoie.
5. Controllare la **diversità semantica**: confrontare il nuovo dilemma con quelli già presenti, anche con ordine invertito e sinonimi. Non contare come nuova idea la stessa figuraccia spostata da WhatsApp a Instagram.

### Metadati editoriali (non esportati)

Archivio di lavoro consigliato: `macrotema`, `meccanismo_principale`, `meccanismi_secondari`, `carattere`, `reazione_attesa`, `fascia_tough` (`ordinario` / `forte` / `insopportabile`), `adatta_live`, `sensibilita`, `famiglia_semantica`, `revisione`, `punteggio_editoriale` e `stato` (`bozza` / `da_rivedere` / `approvata` / `scartata`). Per analizzare la distribuzione, aggiungere `categoria_csv_proposta` e `motivo_classificazione`. Questi valori **non** diventano nuove colonne nel CSV Livecade.

### Verifica automatica e umana

- **Schema:** sette colonne esatte, `language=it`, categorie nell'elenco ammesso, intensità esclusivamente `light` o `tough`, `ref` non vuoto e univoco.
- **Testo:** `optionA` e `optionB` non vuote e ciascuna lunga al massimo 90 caratteri, comprese spazi e punteggiatura; evitare ritorni a capo e testi identici o equivalenti.
- **Contenuti:** controllo umano di autonomia, comprensibilità, bilanciamento, originalità, intensità e adeguatezza per la live.
- **Importazione:** rileggere il CSV con un parser CSV e controllare che il numero di record resti uguale, senza colonne spezzate da virgole o virgolette. Controllare inoltre che i separatori non introducano spazi fuori dai campi (`social,tough`, non `social, tough`); i testi quotati possono contenere virgole e spazi legittimi.

### Valutazione editoriale e criteri di ammissione

**Controlli obbligatori:** rispettare schema e valori CSV, massimo 90 caratteri per opzione, chiarezza e autonomia delle alternative, assenza di duplicati sostanziali, pertinenza della categoria e limiti di contenuto. Un punteggio alto **non compensa** il fallimento di questi controlli.

**Griglia di qualità proposta (1–5 per criterio):**

| Criterio | Peso | Domanda guida |
| --- | ---: | --- |
| Difficoltà ed equilibrio della scelta | **30%** | Entrambe le alternative hanno motivi credibili a favore e contro? |
| Originalità | **25%** | Introduce un conflitto realmente nuovo rispetto all'archivio? |
| Reazione emotiva | **20%** | Suscita risata, imbarazzo, disgusto, sorpresa o riflessione? |
| Potenziale di discussione | **15%** | Porta a spiegare e difendere la scelta? |
| Chiarezza e logica | **10%** | Si comprende subito ed è coerente anche se assurda? |

**Formula:** `punteggio = 0,30×difficoltà + 0,25×originalità + 0,20×reazione + 0,15×discussione + 0,10×chiarezza` (scala 1–5).

**Soglia editoriale iniziale:** ammettere i candidati con **punteggio ≥ 4,0/5**, purché superino tutti i controlli obbligatori. Tra **3,5 e 3,99**: riscrivere e rivalutare; sotto **3,5**: scartare o riprogettare. Questa è una **regola di lavoro proposta**, non una garanzia oggettiva né un requisito di Livecade; ricalibrare pesi e soglia attraverso test reali. Se il punteggio complessivo è alto ma un criterio essenziale è chiaramente insufficiente, chiedere comunque una revisione umana.

**Come interpretare l'equilibrio:** non significa ottenere sempre risposte 50/50. Una domanda con voti molto sbilanciati può essere brillante, ma se quasi tutti scelgono la stessa opzione *senza esitazione*, va rivista. Registrare percentuale di voto, commenti spontanei e `pass` come **segnali**, non come verdetti isolati; non chiedere confessioni o informazioni personali per misurarne l'efficacia.

**Regola di ammissione:** una domanda entra nel database perché è **buona e diversa**, non perché serve a completare `food`, `sports`, `light` o un numero prefissato. In caso di dubbio, privilegiare la revisione o l'esclusione.

### Controllo periodico della distribuzione

- Analizzare la composizione per categoria, macrotema, meccanismo principale, reazione attesa e intensità **senza pretendere quote identiche**.
- Identificare le famiglie ricorrenti a livello di significato (es. leggere chat, pubblicare chat, mostrare messaggi privati) anche se i testi differiscono o A/B sono invertite.
- In una categoria sottorappresentata, **proporre** candidati più vari e passarli alla stessa selezione. Se nessuno merita l'ammissione, non aggiungere nulla.
- Valutare l'esperienza di gioco complessiva: pochi temi dominanti, ripetizioni e lunghe sequenze con la stessa emozione possono rendere monotono anche un archivio di domande individualmente forti.

---

## Motivazioni delle scelte editoriali

Le regole seguenti sono **decisioni di progettazione del gioco**, non vincoli tecnici dichiarati da Livecade.

| Scelta | Motivazione | Conseguenza pratica |
| --- | --- | --- |
| **Niente quote fisse** per categoria o intensità | Una quota può premiare domande deboli solo perché manca un numero da raggiungere | Si ammettono 30 domande eccellenti invece di 100 mediocri; i totali possono essere diversi |
| **Qualità verificata prima della distribuzione** | Equilibrio, novità e chiarezza sono ciò che rende interessante una scelta | Tutti i candidati, anche nelle categorie rare, passano gli stessi controlli |
| **Varietà tematica, meccanica ed emotiva** | La categoria da sola non distingue gli scenari: molte domande `love` possono ripetere lo stesso conflitto | Si cercano differenti contesti, meccanismi e reazioni, non semplici sinonimi |
| **Categorie scelte per pertinenza** | Etichette forzate confondono filtri e statistiche del gioco | Una domanda su fama resta `fame`, anche se `sports` ha poche righe |
| **Soglia 4/5 come punto di partenza** | Un filtro esplicito è più ripetibile del giudizio vago "è carina" | La soglia è ricalibrabile, con revisione umana e senza rigidità cieca |
| **Copertura minima per sessione (inizialmente 200 approvate)** | Un archivio eccellente ma troppo piccolo non sostiene una diretta di due ore a ritmo rapido | Si preparano 160 principali e 40 di riserva, rivalutando il fabbisogno con i tempi reali |
| **La live determina il ritmo** | Archivio e singola sessione hanno esigenze diverse | Si alternano contenuti durante la diretta senza forzare la composizione del CSV |
| **Feedback reale, non solo voti** | Un 50/50 non misura da solo divertimento o coinvolgimento | Si osservano discussioni, risate, domande saltate e saturazione |

**Esempio pratico:** se `social` contiene già molte figuracce legate a chat divulgate, non si generano altre dieci varianti cambiando l'app o il destinatario. Si esplorano reputazione, amicizia, lealtà, competizione, status o verità scomode. Se `sports` ha meno domande ma quelle esistenti sono forti, non va riempita artificialmente: si possono progettare nuovi conflitti di rivalità, rischio fisico immaginario, ego e vittoria, mantenendo solo quelli migliori.

**Principio conclusivo:** *il database cresce con nuove scelte memorabili; la scaletta della live deve inoltre disporre di una scorta sufficiente per la durata programmata. La copertura si ottiene producendo più domande valide, mai accettando riempitivi.*
