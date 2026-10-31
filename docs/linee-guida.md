# Linee guida di scrittura

[← Torna al README](../README.md)

Come costruire una domanda: struttura, intensità, meccanismi, temi, tono e limiti.

## Indice

- [Anatomia di una domanda](#anatomia-di-una-domanda)
- [Livelli di intensità](#livelli-di-intensità)
- [Meccanismi del dilemma](#meccanismi-del-dilemma)
- [Macrotemi e categorie](#macrotemi-e-categorie)
- [Regole Assurde e Divieti Impossibili](#regole-assurde-e-divieti-impossibili)
- [Aggettivi per il carattere](#aggettivi-per-il-carattere)
- [Espressioni di tono](#espressioni-di-tono)
- [Glossario per le live](#glossario-per-le-live)
- [Regole di qualità e limiti](#regole-di-qualità-e-limiti)
- [Ricerca Reddit e originalità](#ricerca-reddit-e-originalità)

---

## Anatomia di una domanda

Ogni domanda si costruisce su tre elementi.

1. **Tema**: di cosa parla (vedi [Macrotemi e categorie](#macrotemi-e-categorie)).
2. **Meccanismo**: perché scegliere è difficile (vedi [Meccanismi del dilemma](#meccanismi-del-dilemma)).
3. **Carattere**: come deve far sentire il giocatore (vedi [Aggettivi](#aggettivi-per-il-carattere) ed [Espressioni di tono](#espressioni-di-tono)).

Una domanda piccante, disgustosa o assurda non basta. Senza un meccanismo che renda le due opzioni equilibrate, la scelta è ovvia e la domanda non funziona.

**Tenere distinti:** il *tema* descrive il contenuto, il *meccanismo* crea il conflitto, il *carattere* determina il tono e l'*intensità* misura il disagio o l'impatto. Una domanda può essere `tough` senza essere volgare o estrema; una domanda `light` può essere assurda e molto divertente.

---

## Livelli di intensità

Nel CSV esistono solo `light` e `tough`, e questi valori **non sono modificabili** (vedi la [regola inamovibile](../README.md#formato-e-vincoli)). **"Preferirei morire"** è una *fascia interna* del `tough` (e può essere l’effetto cercato dal meccanismo **Il Dilemma Insopportabile**), mai un terzo valore CSV o un’opzione letterale di morte.

| Livello | Valore CSV | Effetto cercato | Opzione A | Opzione B |
| --- | --- | --- | --- | --- |
| Light | `light` | Far ridere o arrossire un po' | Mandare per sbaglio un vocale lunghissimo a vostro zio | Mandare per sbaglio un meme al gruppo di lavoro |
| Tough | `tough` | Mettere davvero a disagio | Il vostro capo legge una chat in cui vi lamentate di lui | Vostra madre legge la chat del vostro gruppo di amici |
| Preferirei morire | `tough` | Far rifiutare entrambe le opzioni | La vostra famiglia legge tutte le vostre chat dell'ultimo anno | Il vostro ex legge tutte le chat in cui avete parlato di lui |

**Fascia estrema senza quote obbligatorie:** il Dilemma Insopportabile va usato come picco narrativo, non come componente numerica da riempire. Per una live generalista si può **provare** una presenza contenuta (ad esempio 10–20% delle domande `tough` mostrate), per poi adattarla alle reazioni: è una scelta di programmazione della sessione, **non** una percentuale imposta al database.

### Criteri della fascia "preferirei morire"

- Ogni opzione, presa da sola, è un no secco: non solo scomoda, inaccettabile.
- Le due opzioni sono ugualmente terribili. Se una è chiaramente meno peggio, il dilemma sparisce.
- Concreta e specifica: persone precise (vostra madre, il vostro ex, il vostro capo) e contenuti precisi (cronologia, chat, foto).
- Conseguenze pubbliche, durature o intimamente intollerabili: non sempre serve una punizione permanente.
- Catastrofica ma da ridere: deve far urlare "no!" ridendo, non far calare il silenzio.
- "Preferirei morire" è una reazione iperbolica da evocare, mai un’opzione: la scelta resta obbligatoria nel gioco.
- Il disagio appartiene allo **scenario immaginario**, non a una persona reale costretta a confessare: si può sempre saltare una domanda che mette davvero a disagio.

### Esempi di fascia alta

| Categoria | Opzione A | Opzione B |
| --- | --- | --- |
| `love` | I vostri genitori vi sentono durante un momento intimo | Voi sentite i vostri genitori durante un momento intimo |
| `love` | Il vostro partner vede tutti i profili che avete spiato sui social | Il vostro ex legge in pubblico i messaggi che gli scrivevate |
| `social` | Sapere cosa pensa davvero di voi ogni persona che conoscete | Tutti sanno cosa pensate davvero di loro |
| `social` | I vostri pensieri vengono trasmessi in diretta per 24 ore | Le vostre ricerche online appaiono sopra la vostra testa per un mese |
| `gross` | Usare lo spazzolino di uno sconosciuto per un mese | Indossare le stesse mutande per un anno senza lavarle |
| `money` | Perdere tutti i vostri risparmi domani | Lavorare gratis per due anni per la persona che odiate di più |
| `survival` | Una settimana bloccati in ascensore con il vostro ex | Un mese su un'isola deserta con il collega più insopportabile |

---

## Meccanismi del dilemma

Il meccanismo è ciò che rende la scelta difficile: ogni domanda deve averne almeno uno riconoscibile.

| Meccanismo | Come funziona |
| --- | --- |
| Perdere-perdere (*Il Male Minore*) | Entrambe le conseguenze sono negative; si confrontano gravità, durata e reversibilità. Non è un macrotema né una categoria predefinita. |
| Desiderio contro vergogna | Ottieni qualcosa che vuoi, ma devi esporti pubblicamente |
| Vantaggio contro sacrificio | Guadagni qualcosa rinunciando a un valore importante |
| Segreto contro reputazione | Proteggi una verità oppure salvi la tua immagine |
| Piacere contro disgusto | Una ricompensa allettante comporta una conseguenza ripugnante |
| Assurdo contro plausibile | Una scelta surreale compete con una situazione realistica altrettanto terribile |
| Fedeltà contro interesse | Favorisci una persona importante oppure te stesso |
| Verità contro conseguenze | Confessi qualcosa oppure continui a nasconderlo |
| Controllo contro libertà | Ottieni sicurezza perdendo autonomia, oppure rischi tutto |
| Male immediato contro male futuro | Subisci una conseguenza subito o una peggiore più avanti |
| Rischio contro certezza | Prendi poco ma sicuro, oppure tanto con la possibilità di perdere tutto |
| Subire contro infliggere | Soffri tu una cosa, oppure la fai soffrire a qualcun altro |
| **Vantaggio assoluto contro invidia** | Ottieni molto ma un rivale ottiene di più, oppure accetti poco pur di non farlo vincere |
| **Colpa segreta contro condanna ingiusta** | Resti impunito dopo una colpa immaginaria, oppure sei innocente ma tutti ti ritengono colpevole |
| **Fastidio cronico contro shock unico** | Sopporti un piccolo disagio ripetuto per anni oppure una sola umiliazione molto intensa |
| **Il Dilemma Insopportabile (Nessuna Via d’Uscita)** | Entrambe le opzioni fanno reagire con un rifiuto istintivo: devi scegliere fra due conseguenze ugualmente inaccettabili, ma comprensibili e narrativamente efficaci |
| **Conoscenza contro serenità** | Scoprire qualcosa di affascinante o scomodo al prezzo della tranquillità, oppure mantenere un'ignoranza rassicurante |
| **Impatto contro felicità** | Lasciare un segno importante a caro prezzo emotivo, oppure vivere serenamente senza riconoscimenti straordinari |
| **Ragione contro istinto** | Preferire la scelta più sensata nei risultati oppure quella che risponde a intuizioni, affetti e valori personali |

### Tre meccanismi riflessivi: quando usarli

- **Conoscenza contro serenità:** definire che cosa si scopre e qual è il prezzo emotivo. Non rendere il sapere automaticamente vantaggioso o la serenità automaticamente ingenua. Può produrre `light` o `tough` a seconda delle conseguenze.
- **Impatto contro felicità:** confrontare riconoscimento, contributo al mondo, fatica e benessere. Una vita ordinaria non è per definizione inferiore, né una vita memorabile è automaticamente migliore.
- **Ragione contro istinto:** chiarire perché la scelta razionale è utile e quella intuitiva è umanamente convincente. Non ridurre l'istinto a irrazionalità o la ragione a freddezza caricaturale.

| Meccanismo | Opzione A | Opzione B | Categoria indicativa |
| --- | --- | --- | --- |
| Conoscenza contro serenità | Sapere sempre quando qualcuno vi mente, anche sui dettagli più dolorosi | Non scoprire mai una bugia che potrebbe rovinarvi una bella giornata | `dilemmas` |
| Impatto contro felicità | Creare un'invenzione famosa senza poter godere della vostra vita privata | Vivere felici nell'anonimato senza ottenere grandi riconoscimenti | `fame` |
| Ragione contro istinto | Scegliere sempre la soluzione più logica, anche quando vi rende impopolari | Seguire sempre il vostro intuito, anche se a volte vi porta fuori strada | `dilemmas` |

Questi sono **meccanismi editoriali**. Per ogni domanda controllare che il conflitto sia effettivo e che A e B restino autonome e sotto i 90 caratteri. Una risposta ragionata e pacata è un esito valido: non forzare sempre un costo scioccante.

### Il Dilemma Insopportabile: regole operative

È il **16° meccanismo** nell’elenco, non una categoria CSV e non un livello di intensità distinto. Si associa di norma a `tough` e può combinarsi con *Perdere-perdere*, *Subire contro infliggere*, *Segreto contro reputazione* e *Piacere contro disgusto*.

1. **Doppio rifiuto:** prese separatamente, entrambe le opzioni devono far dire "no".
2. **Equilibrio:** nessuna delle due deve essere una via di fuga evidente; considerare gravità, durata, probabilità, reversibilità e impatto sociale.
3. **Specificità:** usare persone, azioni e conseguenze concrete; evitare formule generiche tipo "una cosa terribile".
4. **Nessuna scappatoia narrativa:** niente soluzioni implicite (es. mentire, pagare per evitare, annullare il patto), pur lasciando al giocatore la libertà reale di non partecipare.
5. **Intrattenimento, non trauma:** puntare su vergogna, disgusto immaginario, perdita di reputazione, assurdità e dilemmi morali; evitare di trasformare sofferenze reali in una gag.
6. **Plausibilità emotiva:** anche un'ipotesi assurda deve avere conseguenze comprensibili e coerenti.
7. **Varietà:** non ripetere sempre chat divulgate, ex, genitori e figuracce; cambiare contesto, posta in gioco e meccanismo secondario.

**Esempi di meccanismo (opzioni sotto i 90 caratteri):**

| Categoria CSV | Opzione A | Opzione B |
| --- | --- | --- |
| `social` | Tutti vedono la vostra cronologia di ricerca degli ultimi cinque anni | Tutti ascoltano i vostri vocali più imbarazzanti degli ultimi cinque anni |
| `gross` | Avere l'odore di un bidone dell'umido ogni volta che sorridete | Sentire sapore di dentifricio scaduto ogni volta che bevete acqua |
| `money` | Perdere tutti i risparmi per cancellare la vostra figuraccia peggiore | Rivedere in TV ogni mese la figuraccia peggiore della vostra vita |
| `dilemmas` | Il vostro migliore amico scopre la bugia più grave che gli avete detto | Scoprire davanti a tutti la bugia più grave del vostro migliore amico |

**Nota sul confronto con Perdere-perdere:** tutte le domande insopportabili sono di tipo "perdere-perdere", ma non tutti i "perdere-perdere" sono insopportabili. La differenza è **l'intensità del rifiuto che provocano entrambe le scelte**, non la sola presenza di due conseguenze negative.

**Distinzione progettuale:** il Dilemma Insopportabile è anche un *meccanismo composito* (un amplificatore editoriale): indica il livello di rifiuto, ma non spiega da solo **perché** la scelta è difficile. Annotare sempre almeno un altro meccanismo concreto, come *Segreto contro reputazione*, *Subire contro infliggere* o *Controllo contro libertà*.

**Specificare bene rischio e danno:** in *Rischio contro certezza* indicare probabilità, premio e perdita quando servono a capire il confronto; in *Subire contro infliggere* chiarire chi subisce, quanto dura il danno e se la conseguenza è simmetrica, senza chiamare in causa atti reali contro persone del gruppo.

### Tre meccanismi aggiuntivi: indicazioni ed esempi

- **Vantaggio assoluto contro invidia:** tenere comparabili premio e prezzo emotivo. L'invidia è il costo della prima opzione, la rinuncia al premio è il costo della seconda. Non usare sempre il denaro: funzionano anche fama, talento, successo o riconoscimenti.
- **Colpa segreta contro condanna ingiusta:** distinguere *colpa reale* e *reputazione percepita*. Privilegiare colpe inventate e conseguenze ipotetiche, senza chiedere confessioni di reati veri.
- **Fastidio cronico contro shock unico:** precisare frequenza, durata e intensità; bilanciare il disagio ripetuto con un episodio breve ma memorabile. Evitare traumi reali usati come gag.

| Meccanismo | Opzione A | Opzione B | Categoria indicativa |
| --- | --- | --- | --- |
| Vantaggio contro invidia | Vincere 10.000 €, ma il vostro rivale ne riceve 20.000 | Vincere 100 €, ma il vostro rivale resta senza premio | `money` |
| Colpa contro condanna | Rompere di nascosto il trofeo del gruppo senza essere scoperti | Essere accusati da tutti di aver rotto il trofeo del gruppo, pur essendo innocenti | `social` |
| Fastidio contro shock | Starnutire rumorosamente a ogni riunione per il resto della vita | Cadere dal palco davanti a mille persone una sola volta | `school-work` |

Questi tre sono **meccanismi narrativi**, non nuove categorie o intensità CSV.

---

## Macrotemi e categorie

I **31 macrotemi principali** sono filoni di progettazione, **non** valori di `category`. La tabella comprende **33 righe** perché *Caos & Conseguenze Impreviste* ha tre sottogeneri. È la fusione delle integrazioni caricate e dei macrotemi già approvati o discussi, senza perdere *Regole Assurde & Divieti Impossibili*.

**Molte categorie per macrotema, una sola categoria per domanda:** la categoria *primaria* è il riferimento più naturale, non una destinazione obbligatoria. Le *secondarie* sono percorsi validi quando il contenuto della singola domanda cambia; non vanno usate per compensare squilibri numerici. Nel CSV `category` contiene **un solo valore** fra i 14 consentiti.

**Tipi di macrotema:** *Conflitto* descrive cosa mette in difficoltà (segreti, reputazione, invidia), mentre *Ambito* indica dove o su che cosa accade (casa, viaggio, lavoro). La generazione può **incrociare conflitto × ambito × meccanismo** per creare nuove situazioni, ma i tag editoriali restano separati dal CSV.

| Macrotema | Tipo | Territorio narrativo | Primaria | Secondarie ammesse se pertinenti |
| --- | --- | --- | --- | --- |
| Livello Cringe | Conflitto | Figuracce, messaggi sbagliati, situazioni sociali e sentimentali imbarazzanti | `social` | `school-work`, `love`, `fame`, `sports`, `food` |
| Scheletri nell'Armadio | Conflitto | Segreti, bugie, confessioni immaginarie, passato imbarazzante | `social` | `love`, `school-work`, `fame`, `dilemmas` |
| Il Prezzo dell'Anima | Conflitto | Corruzione, compromessi morali, denaro in cambio di principi | `money` | `dilemmas`, `school-work`, `fame`, `sports` |
| Unpopular Opinion | Conflitto | Convenzioni sociali, opinioni impopolari, doppi standard | `social` | `food`, `lifestyle`, `sports`, `dilemmas` |
| Ego, Potere & Reputazione | Conflitto | Viralità, successo pubblico, scandali, bisogno di visibilità | `fame` | `social`, `money`, `school-work`, `sports` |
| Verità Brutali | Conflitto | Prime impressioni, giudizi sinceri e dilemmi di sincerità | `dilemmas` | `social`, `love`, `school-work` |
| Red Flag & Relazioni Tossiche | Conflitto | Gelosie, tradimenti e dinamiche sentimentali problematiche (solo finzione) | `love` | `social`, `lifestyle`, `dilemmas` |
| Amicizia & Lealtà | Conflitto | Favori, fiducia, tradimenti tra amici, appartenenza al gruppo; rivalsa/karma come sottogenere | `social` | `dilemmas`, `love` |
| Soldi Facili & Debiti | Conflitto | Prestiti, debiti, fortuna economica, lusso selettivo, rischio e rinunce | `money` | `dilemmas`, `social`, `lifestyle` |
| Identità & Ricordi | Conflitto | Memoria personale, personalità, cancellazione dei rimpianti, identità segrete | `dilemmas` | `fantasy`, `social`, `time-travel` |
| Fortuna, Sfortuna & Destino | Conflitto | Premi fortuiti, sfortuna trasferibile, coincidenze e predestinazione immaginaria | `fantasy` | `money`, `dilemmas`, `silly` |
| Comunicazione & Malintesi | Conflitto | Parole fraintese, bugie impossibili, traduzione assurda, pensieri che sfuggono | `social` | `silly`, `dilemmas`, `school-work` |
| Scenari Assurdi & Sopravvivenza | Ambito | Catastrofi inventate, risorse limitate e decisioni per cavarsela | `survival` | `silly`, `fantasy`, `food` |
| Caos & Conseguenze Impreviste — assurdo | Ambito | Scambi di ruolo, assurdità e conseguenze quotidiane | `silly` | `lifestyle`, `school-work`, `love` |
| Caos & Conseguenze Impreviste — fantastico | Ambito | Superpoteri difettosi, maledizioni comiche e creature inventate | `fantasy` | `silly`, `survival`, `love` |
| Caos & Conseguenze Impreviste — temporale | Ambito | Bivi del destino, rimpianti, paradossi e viaggi nel tempo | `time-travel` | `dilemmas`, `fantasy`, `school-work` |
| Ufficio & Carriera | Ambito | Capi, colleghi, stipendi, colloqui, promozioni, videochiamate | `school-work` | `money`, `social`, `fame` |
| Cibo & Penitenze a Tavola | Ambito | Ristoranti, sfide culinarie, ingredienti insoliti, diete impossibili | `food` | `gross`, `money`, `lifestyle` |
| Vita Quotidiana & Rinunce | Ambito | Comodità, abitudini, consumi, vizi quotidiani, rinunce personali | `lifestyle` | `money`, `social`, `food` |
| Disgusto & Corpo | Ambito | Odori, igiene, abitudini sgradevoli e repulsione immaginaria | `gross` | `food`, `sports`, `lifestyle` |
| Sport & Rivalità | Ambito | Palestra, gare, competizione, risultati e tifo | `sports` | `fame`, `social`, `gross` |
| Famiglia & Parenti | Ambito | Suoceri, rivalità fra fratelli, festività domestiche, favoritismi, eredità | `social` | `love`, `food`, `dilemmas` |
| Casa & Convivenza | Ambito | Coinquilini, vicini, condominio, bollette, pulizie e privacy | `lifestyle` | `gross`, `social`, `money` |
| Viaggi & Vacanze | Ambito | Voli, hotel, compagni scomodi, vacanze rovinate e avventura | `lifestyle` | `survival`, `money`, `silly` |
| Feste & Matrimoni | Ambito | Ricevimenti, compleanni, discorsi, invitati e riti sociali | `social` | `food`, `money`, `love` |
| Animali & Convivenza Assurda | Ambito | Animali domestici, pet parlanti, convivenza e dilemmi buffi | `silly` | `fantasy`, `lifestyle`, `dilemmas` |
| Spicy & Sotto le Lenzuola | Ambito | Flirt, desideri e situazioni intime tra adulti consenzienti, allusive o esplicite, anche in live | `love` | `silly` |
| Regole Assurde & Divieti Impossibili | Ambito | Privilegi con clausole ridicole, divieti logici e umiliazioni sociali comiche | `silly` | `money`, `food`, `school-work`, `social`, `lifestyle` |
| Tecnologia & Dipendenze Digitali | Ambito | Smartphone, IA, privacy, notifiche, algoritmi, vita digitale distopica | `lifestyle` | `fame`, `social`, `silly` |
| Sonno & Sogni | Ambito | Sogni lucidi, incubi assurdi, notti bizzarre e tempo di riposo | `fantasy` | `silly`, `lifestyle`, `dilemmas` |
| Spoiler, Fandom & Cultura Pop | Ambito | Videogiochi, serie, fandom, spoiler, salvataggi, fenomeni pop | `lifestyle` | `silly`, `fame`, `social` |
| **Grandi Domande** | Conflitto | Identità, memoria, libertà, tempo, valori e scelte di vita; confronto tra prospettive | `dilemmas` | `time-travel`, `lifestyle`, `social`, `fame` |
| **Curiosità & Scoperte** | Ambito | Esperimenti mentali, talenti impossibili, scoperte, enigmi ed esplorazioni | `fantasy` | `dilemmas`, `lifestyle`, `time-travel`, `silly` |

*Conteggio aggiornato:* 29 macrotemi consolidati + 2 nuovi (*Grandi Domande* e *Curiosità & Scoperte*) = **31 macrotemi**, rappresentati in **33 righe** perché *Caos & Conseguenze Impreviste* conserva tre sottogeneri. Le 14 categorie tecniche restano tutte rappresentate come primarie.

### Curiosità e riflessione: cinque sottogeneri dei due nuovi macrotemi

Questi sottogeneri **non sono cinque macrotemi aggiuntivi**: sono aree narrative esplicite utilizzabili per produrre domande concrete, con tag interni `sottogenere` e una sola categoria finale per domanda.

| Sottogenere | Macrotema principale | Categorie possibili | Focus |
| --- | --- | --- | --- |
| **Verità Assolute & Ignoranza Felice** | Grandi Domande | `dilemmas`, `fantasy`, `social` | Misteri, verità difficili, lettura del pensiero, costo del sapere |
| **Bivi Esistenziali & Senso del Tempo** | Grandi Domande | `time-travel`, `lifestyle`, `dilemmas` | Rimpianti, stabilità, passato/futuro, valore del tempo vissuto |
| **Mente, Talento & Percezione** | Curiosità & Scoperte | `fantasy`, `lifestyle`, `dilemmas` | Talenti impossibili, modi diversi di pensare, sogni e ricordi |
| **Eredità & Impronta nel Mondo** | Grandi Domande | `fame`, `dilemmas`, `lifestyle` | Riconoscimento pubblico contro serenità e valore personale |
| **Natura Umana & Fiducia** | Grandi Domande | `social`, `dilemmas`, `love` | Empatia, sincerità, fiducia e appartenenza, senza confessioni forzate |

**Confini con i temi esistenti:** *Identità & Ricordi* tratta specificamente la memoria personale; *Caos — temporale* tratta il dispositivo fantastico del viaggio nel tempo; *Ego, Potere & Reputazione* privilegia visibilità e scandali; *Comunicazione & Malintesi* privilegia scambi e incomprensioni. *Grandi Domande* riguarda invece il conflitto di valori che emerge da questi scenari; *Curiosità & Scoperte* riguarda il piacere della scoperta e dell'esperimento mentale. Applicare il tag più informativo, evitando nuove domande equivalenti a scenari esistenti.

**Esempi (opzioni autonome, massimo 90 caratteri ciascuna):**

| Sottogenere | Opzione A | Opzione B |
| --- | --- | --- |
| Verità Assolute | Conoscere una verità importante che vi toglierebbe ogni tranquillità | Restare sereni senza conoscere una verità fondamentale sulla vostra vita |
| Bivi Esistenziali | Rivivere una giornata felice senza poter cambiare nulla | Usare un giorno nel futuro per scoprire una vostra scelta importante |
| Mente & Percezione | Imparare ogni lingua in una settimana senza poterla insegnare | Capire ogni emozione altrui senza trovare le parole per spiegarla |
| Eredità & Impronta | Essere ricordati per un'invenzione, ma vivere senza tempo libero | Vivere felici e anonimi, senza lasciare un nome famoso |
| Natura Umana | Capire sempre chi si fida di voi, senza sapere perché | Sapere sempre perché qualcuno non si fida di voi |

**Regola dell'intensità:** normalmente `light` per curiosità, talenti, desideri e paradossi; `tough` solo quando il contenuto comporta disagio reale, perdita significativa o un conflitto psicologico difficile. La profondità non è sinonimo di `tough`.

**Regola della qualità:** una domanda non deve essere per forza dolorosa o esilarante. È valida anche quando incuriosisce, sorprende, invita a confrontare argomenti o genera riflessioni **chiare e ragionevoli**. A e B devono comunque essere comparabili, autonome e non banali.

### Il Male Minore: recuperato come meccanismo trasversale

**Il Male Minore non viene cancellato.** Non indica un universo tematico, ma una configurazione di scelta in cui entrambe le conseguenze sono negative. Per questo è una **specializzazione del meccanismo *Perdere-perdere***; può essere annotato come `male_minore` nei metadati editoriali. Non va classificato automaticamente `dilemmas`: un male minore in famiglia può essere `social`, in cucina `food` o `gross`, in ufficio `school-work`, in viaggio `survival` o `lifestyle`.

Non coincide sempre con **Il Dilemma Insopportabile**: il Male Minore comprende anche difficoltà ordinarie e comiche; l'Insopportabile richiede il rifiuto istintivo di entrambe le opzioni e un meccanismo specifico aggiuntivo.

### Sottogeneri recuperati senza moltiplicare i macrotemi

| Sottogenere / proposta | Collocazione principale | Perché non diventa subito autonomo |
| --- | --- | --- |
| Parenti Serpenti & Cene di Famiglia | Famiglia & Parenti | Stesso universo, tono più ironico |
| Amicizia & Tradimento | Amicizia & Lealtà | Conflitto complementare alla fiducia |
| Coinquilini & Condominio da Incubo | Casa & Convivenza | Specifica un ambiente già autonomo |
| Vendette & Karma Istantaneo | Amicizia & Lealtà / Red Flag | Dinamica trasversale; evitare ripicche ripetitive |
| Black Mirror & Vita Digitale | Tecnologia & Dipendenze Digitali | Sottogenere distopico della tecnologia |
| Vacanze Rovinate & Viaggi Estremi | Viaggi & Vacanze | Scenario specializzato e facilmente riutilizzabile |
| Lusso Selettivo & Povertà Assurda | Soldi Facili & Debiti | Ricompensa materiale contro rinuncia quotidiana |
| Superpoteri Difettosi | Caos — fantastico | Potere desiderabile con clausola comica |
| Bivi del Destino & Rimpianti | Caos — temporale / Identità & Ricordi | Paradosso temporale o memoria secondo focus |
| Patto Biologico & Cinque Sensi | Sonno & Sogni / Caos — fantastico | Solo fantastico, senza malattie o traumi reali |
| Talenti Inutili & Maledizioni Sociali | Regole Assurde / Caos — fantastico | Effetto assurdo con costo coerente |
| Regole assurde in ambito scolastico | Regole Assurde / Ufficio & Carriera | `school-work` quando domina il contesto |
| Crimine & Giustizia | Scheletri nell'Armadio / Verità Brutali | Sottogenere definitivo su colpe, processi e giustizia immaginari; non chiedere confessioni vere |

**Promossi a definitivi:** Scuola & Università, Tifo & Passione Sportiva, Arte & Talento e Moda & Apparenza non sono più candidati di prova. Sono categorie editoriali definitive nel [README](../README.md#categorie-editoriali), con i nomi *Scuola, Esami & Università*, *Tifo & Fede Sportiva*, *Arte, Musica & Talento* ed *Estetica, Look & Apparenza*. **Politica, Religione, Morte & Aldilà restano in standby**, anche quando emergono in ricerche esterne. I sottogeneri sono tag creativi e non creano valori di categoria.

### Esempi di classificazione multi-categoria

| Incrocio editoriale | Categoria CSV | Perché |
| --- | --- | --- |
| Livello Cringe × Ufficio | `school-work` | La figuraccia avviene durante una riunione |
| Livello Cringe × Sport | `sports` | La figuraccia altera una gara o un allenamento |
| Famiglia × Cibo | `food` | Il dilemma riguarda piatti e rituali a tavola |
| Spicy × Caos assurdo | `silly` | L'effetto comico immaginario domina il flirt; toni adatti alla live |
| Tecnologia × Reputazione | `fame` | Un algoritmo rende pubblica una figuraccia a livello nazionale |
| Soldi Facili × Amicizia | `money` | Il prezzo del prestito è il centro della scelta |
| Il Male Minore × Casa | `lifestyle` | Si decide fra due fastidi di convivenza |
| Bivi del Destino × Caos temporale | `time-travel` | Cambiare il passato è il cuore del dilemma |
| Regole Assurde × Ristorante | `food` | Premio e clausola comica riguardano il pasto |
| Grandi Domande × Identità & Ricordi | `dilemmas` | Scelta tra memoria, identità e felicità |
| Curiosità & Scoperte × Caos fantastico | `fantasy` | Talento impossibile e prezzo dell'apprendimento |
| Grandi Domande × Ego & Reputazione | `fame` | Impronta nel mondo contro serenità personale |

**Regola di assegnazione:** classificare in base al conflitto e all'argomento *dominante della domanda finale*, non al macrotema usato per generarla. La distribuzione del database rimane dinamica: **nessuna quota obbligatoria per categoria o intensità**, ma nessuna domanda di riempimento.

---

## Regole Assurde e Divieti Impossibili

**Scopo:** trasformare situazioni quotidiane riconoscibili in scene comiche attraverso regole chiare. Una stranezza casuale (come salutare una porta senza alcuna conseguenza) **non** basta. Il dilemma deve unire **vantaggio o limite concreto → clausola coerente → conseguenza comica immaginabile**, con due scelte bilanciate.

Tre sottogeneri editoriali: **Privilegi con Clausole Ridicole**, **Divieti Quotidiani Impossibili**, **Regole Sociali Umilianti**. Non sono categorie CSV e non richiedono quote fisse. Esempi, controesempi, correzioni e verifiche nel documento [Regole Assurde & Divieti Impossibili](regole-assurde.md).

Cinque verifiche specifiche: **causa-effetto**, **comicità visualizzabile**, **costo concreto**, **equilibrio fra A e B**, **escalation sensata**. Se una scena è soltanto insolita ma non fa ridere, non imbarazza e non rende la scelta difficile, **scartare o riscrivere**. Non normalizzare comportamenti lesivi e mantenere i temi in standby esclusi.

---

## Aggettivi per il carattere

Di norma un aggettivo compare in un solo gruppo, quello dove descrive meglio l'effetto cercato. Può stare in più gruppi solo se in ciascuno ha un significato diverso: *intriganti* vuol dire attraenti in *Romantiche e sensuali* e stimolanti in *Curiose e stimolanti*; *ingegnose* indica una sorpresa ben costruita in *Sorprendenti e paradossali* e un ragionamento brillante in *Curiose e stimolanti*.

| Gruppo | Aggettivi |
| --- | --- |
| Provocatorie e audaci | provocatorie, audaci, sfacciate, sfrontate, irriverenti, impertinenti, insolenti, spudorate, temerarie, spregiudicate, ardite, azzardate, dissacranti, sovversive, pungenti, taglienti, graffianti, mordaci, caustiche, sfidanti, disinibite, ribelli, anticonformiste |
| Controverse e divisive | controverse, polemiche, divisive, polarizzanti, scottanti, spinose, scomode, discutibili, dibattute, incendiarie, esplosive, ambigue, moralmente ambigue, controcorrente, conflittuali, difficili da difendere, socialmente scomode |
| Imbarazzanti e personali | imbarazzanti, indiscrete, intime, personali, private, invadenti, inopportune, sconvenienti, scabrose, impudiche, umilianti, compromettenti, vergognose, difficili da confessare, emotivamente esposte |
| Romantiche e sensuali | romantiche, sensuali, seducenti, ammiccanti, flirtanti, allusive, maliziose, piccanti, osé, spinte, pruriginose, stuzzicanti, intriganti, tentatrici, provocanti, passionali, proibite, cariche di tensione |
| Divertenti e comiche | divertenti, spassose, esilaranti, comiche, buffe, spiritose, ironiche, sarcastiche, goliardiche, demenziali, assurde, bizzarre, stravaganti, strampalate, folli, ridicole, tragicomiche, improbabili, farsesche, nonsense, caricaturali, parodistiche |
| Sorprendenti e paradossali | inaspettate, sorprendenti, imprevedibili, spiazzanti, sconcertanti, destabilizzanti, paradossali, surreali, contraddittorie, controintuitive, assurde ma plausibili, ingegnose, beffarde, ironicamente crudeli, con conseguenze nascoste, dal finale inatteso |
| Profonde ed esistenziali | profonde, esistenziali, filosofiche, introspettive, morali, etiche, dilemmatiche, psicologiche, emotive, vulnerabili, identitarie, riflessive, sincere, enigmatiche, tormentate, laceranti |
| **Curiose e stimolanti** | curiose, intriganti, stimolanti, brillanti, ingegnose, perspicaci, argute, illuminanti, accattivanti, esplorative, conoscitive, intellettualmente vivaci, capaci di suscitare meraviglia e nuove domande |
| Difficili e spietate | difficili, impossibili, crudeli, sadiche, spietate, impietose, brutali, dirette, schiette, estreme, atroci, irreversibili, dolorose, disperate, senza compromessi, senza via d'uscita, a trabocchetto, a tranello, ingannevoli, moralmente costose, a perdere in entrambi i casi |
| Disgustose e disturbanti | disgustose, nauseanti, ripugnanti, rivoltanti, stomachevoli, repellenti, raccapriccianti, macabre, morbose, grottesche, viscerali, inquietanti, scioccanti, fisicamente sgradevoli, da voltastomaco |
| Esplosive per il gruppo | rivelatrici, accusatorie, competitive, indisponenti, spietatamente sincere, capaci di scatenare gelosie, rivalità, sospetti, confessioni e confronti |

Da evitare: **faziose**, che è un difetto e non una qualità; l'effetto giusto è "polarizzanti ma equilibrate".

---

## Espressioni di tono

Servono a descrivere l'effetto che un blocco di domande deve avere.

| Obiettivo | Espressioni |
| --- | --- |
| Provocare | senza filtri, senza peli sulla lingua, a bruciapelo, senza vergogna, dritte al punto, politicamente scorrette nel tono, da far arrossire, che nessuno vuole sentirsi fare, da far saltare la cena di Natale coi parenti |
| Divertire | da morire dal ridere, talmente assurde da sembrare vere, da vergognarsi anche solo a scegliere, da non raccontare ai genitori, degne di una commedia demenziale |
| Mettere in difficoltà | qualunque risposta ti incastra, non esiste una risposta pulita, scegli il tuo disastro, impossibili da giustificare, non c'è via di fuga, ogni scelta ha un prezzo, che mettono in crisi, preferirei morire |
| Coinvolgere il gruppo | da far discutere per mezz'ora, da dividere la chat, che fanno litigare, da scatenare sospetti, da mettere alla prova le amicizie, da far emergere segreti, da far cambiare idea sugli amici |
| **Incuriosire e far riflettere** | non ci avevo mai pensato, c'è più di una risposta sensata, cambia prospettiva, vale la pena pensarci, cosa conta davvero, una scelta da argomentare, fa venire altre domande |

---

## Glossario per le live

Quando una live richiede un registro più prudente, preferire formulazioni **allusive, non grafiche e comprensibili**, senza impoverire il dilemma. Gli eufemismi aiutano a moderare il registro; **non garantiscono l'approvazione o la monetizzazione** della piattaforma, che dipendono dal contesto e dalle regole aggiornate.

| Quando il tema riguarda… | Espressioni consigliate | Accorgimento |
| --- | --- | --- |
| Sessualità e rapporti | momento intimo, intimità, notte insieme | Preferire sottintesi a dettagli anatomici |
| Immagini riservate | foto privata, scatto personale, immagine confidenziale | Non sollecitare foto o materiali reali |
| Relazioni non definite | frequentazione, interesse romantico, storia non ufficiale | Rendere chiaro se la coppia è esclusiva o no |
| Attrazione e flirt | cotta, chimica, tensione romantica, sguardo provocante | Evitare descrizioni grafiche |
| Fantasie | fantasia segreta, desiderio inconfessabile | Non chiedere ai partecipanti di rivelarne di proprie |
| Tradimenti e gelosia | doppia vita sentimentale, messaggio compromettente | Presentare comportamenti tossici come dilemmi, non modelli da imitare |
| Figuracce e indiscrezioni | chat privata, ricerca imbarazzante, messaggio fuori posto | Solo ipotesi immaginarie, mai esposizione di dati reali |

**Checklist della diretta:** distinguere il contenuto *consentito* da quello *adatto al proprio pubblico*. Prevedere filtri editoriali e la possibilità di saltare una domanda; evitare di mostrare o richiedere dati personali autentici.

---

## Regole di qualità e limiti

### Qualità

- **Alternative autonome:** ogni opzione si capisce da sola; l'opzione B non deve mai dipendere dall'opzione A.
- **Equilibrio:** nessuna delle due opzioni è palesemente migliore **per il pubblico a cui si rivolge**, considerando probabilità, durata, reversibilità, benefici, danni e contesto; non serve che siano uguali in ogni dimensione.
- **Reazione:** ogni domanda suscita una risposta **forte oppure chiara e ragionevole**: risata, disgusto, imbarazzo, sorpresa, curiosità, meraviglia, interesse, riflessione o discussione. Non penalizzare un esperimento mentale perché non scandalizza.
- **Logica umana:** anche le domande assurde devono avere una logica comprensibile. Nel filone *Regole Assurde*, esigere un rapporto causa-effetto fra beneficio/divieto e prezzo comico; il semplice comportamento casuale non basta.
- **Varietà:** cambiare situazioni, protagonisti, conseguenze e meccanismi; niente ripetizioni **anche se le parole cambiano**. Controllare duplicati con opzioni invertite A/B.
- **Ritmo:** alternare toni, categorie, meccanismi e intensità secondo le reazioni reali; non applicare quote fisse. La fascia estrema resta un picco occasionale, non il tono dominante.

### Alternative autonome

Chi legge una sola delle due opzioni deve capire esattamente cosa sceglierebbe. L'opzione B non deve mai riprendere, completare o contraddire l'opzione A.

Campanelli d'allarme nell'opzione B: rimandi come "quella", "quello", "lo stesso", "la sua", "invece", "anche", oppure frasi che iniziano con "Tenere…", "Evitare…", "Rinunciare a…" **quando** si riferiscono a qualcosa nominato solo nella A. Queste parole non sono vietate in assoluto: conta che il referente sia presente e chiaro nella singola opzione.

**Esempio `money`**

| Versione | Opzione A | Opzione B |
| --- | --- | --- |
| Sbagliata | Perdere ogni risparmio per cancellare la figuraccia peggiore della vostra vita | Tenere i soldi, ma rivivere quella figuraccia in TV ogni mese |
| Corretta | Perdere tutti i risparmi per cancellare la vostra figuraccia peggiore | Rivedere in TV ogni mese la figuraccia peggiore della vostra vita |

Problema: "Tenere i soldi" e "quella figuraccia" hanno senso solo dopo aver letto l'opzione A.

**Esempio `dilemmas`**

| Versione | Opzione A | Opzione B |
| --- | --- | --- |
| Sbagliata | Far scoprire a un amico la vostra bugia più grave | Scoprire pubblicamente la sua bugia più grave |
| Corretta | Il vostro migliore amico scopre la bugia più grave che gli avete detto | Scoprire davanti a tutti la bugia più grave del vostro migliore amico |

Problema: "la sua" si riferisce all'amico nominato solo nell'opzione A.

### Limiti

- Il tough può essere molto piccante, cattivo o disturbante, ma gli abusi non vanno mai presentati come situazioni sessuali desiderabili.
- Niente tragedie vere (lutti, malattie): non fanno ridere, spengono la serata.
- **Riferimenti sessualmente espliciti:** sono ammessi, anche in live, perché il pubblico è composto solo da maggiorenni. Riguardano solo adulti consenzienti in scenari immaginari e si marcano nei metadati con `esplicito`, così si possono escludere quando serve.
- Mai riferimenti sessuali che coinvolgano minori, ambientazioni scolastiche, infanzia o adolescenza, né situazioni senza consenso presentate come desiderabili.
- Le regole della piattaforma di streaming valgono a prescindere dall'età del pubblico: prima di portare in live domande esplicite, verificare che la piattaforma usata le consenta.
- "Preferirei morire" è un’etichetta interna: non compare nel testo delle domande.
- Le situazioni di tradimento, manipolazione o violazione della privacy possono essere scenari di dilemma, ma non vanno normalizzate né proposte come azioni reali da compiere.
- In giochi di gruppo, consentire sempre di **passare** senza spiegazioni quando il contenuto tocca esperienze personali sensibili: la scelta è obbligatoria solo *all’interno della finzione*.
- **Non confondere personaggio e partecipante:** formulare scenari immaginari, senza chiedere di mostrare chat, cronologie, foto intime o altri dati reali. Se la domanda evoca confessioni personali, non pretenderle in diretta.
- **Seconda persona plurale:** le opzioni si rivolgono al pubblico con verbi, pronomi e possessivi al plurale (*voi*): "il vostro capo", "vi lamentate", "bloccati in ascensore". Il plurale parla a tutta la chat che vota e non costringe a scegliere un genere per chi gioca.
- **Bersagli e stereotipi:** evitare bersagli reali identificabili e stereotipi gratuiti.
- **Adattamento alla diretta:** usare tag editoriali separati per contenuti delicati e una modalità più prudente se il contesto della piattaforma o il pubblico lo richiede.


---

## Ricerca Reddit e originalità

Consultare regolarmente [r/WouldYouRather](https://www.reddit.com/r/WouldYouRather/) nelle sezioni **Top** (all time, anno, mese, settimana), **Hot** e **New**. Per la selezione usare quattro segnali, in ordine: (1) dilemma effettivo e comprensibile, (2) commenti che argomentano scelte *diverse*, (3) possibilità di ridurlo a **due opzioni autonome sotto i 90 caratteri**, (4) voti e visibilità come indizi secondari. Non considerare gli upvote una misura di qualità in sé: un post può diventare popolare per meme, attualità o polemica.

**Metodo in sei passaggi:**

1. Registrare nel registro delle fonti l'URL e la data di consultazione, il tema, il meccanismo e i motivi per cui il post ha generato discussione.
2. Leggere una selezione di commenti: identificare sia le ragioni di A e B, sia le scappatoie e le condizioni implicite contestate dagli utenti.
3. Estrarre soltanto il **pattern astratto** (es. ricompensa certa contro beneficio ripetuto), non la formulazione originale.
4. Ideare un contesto, un costo e una conseguenza **differenti**, comprensibili al pubblico italiano e coerenti col gioco.
5. Verificare autonomia, equilibrio, seconda persona plurale, limiti editoriali e tecnici, nonché duplicati semantici nell'intero database (anche con A e B invertite).
6. Selezionare solo le domande con valutazione sufficiente; tracciare i riferimenti **nei metadati**, non nelle sette colonne Livecade.

**Segnali d'allarme:** post con 3+ opzioni, dilemma risolvibile con una scappatoia, enorme quantità di regole nascoste nel corpo, casi traumatici usati per shock, conflitti che dipendono da abilità fisiche o disponibilità economiche non dichiarate, sondaggi il cui successo deriva soltanto dalla battuta. Reddit è un laboratorio di idee, **non** un dataset da copiare o tradurre in blocco.

Per esempi verificati, criteri di esclusione e una selezione di discussioni si veda [Ricerca Reddit](ricerca-reddit.md). Le categorie CSV e le intensità rimangono immutabili.
