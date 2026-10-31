# Would You Rather Questions

Linee guida per scrivere le domande "Preferiresti…" del gioco: controverse, provocatorie, divertenti, imbarazzanti, curiose o riflessive e, quando serve, spietate. Le domande sono pensate per il formato CSV di **Livecade** e per un pubblico adulto, anche in live.

> **Nota:** questa repository contiene contenuti pensati per un pubblico adulto.

## Indice

- [Documentazione](#documentazione)
- [Filosofia delle domande](#filosofia-delle-domande)
- [Formato e vincoli](#formato-e-vincoli)
- [Categorie editoriali](#categorie-editoriali)
- [Checklist della domanda](#checklist-della-domanda)
- [Checklist del file CSV](#checklist-del-file-csv)

---

## Documentazione

| File | Contenuto |
| --- | --- |
| [Linee guida di scrittura](docs/linee-guida.md) | Anatomia di una domanda, intensità, meccanismi, macrotemi, aggettivi, tono, glossario per le live, regole di qualità e limiti |
| [Protocollo di generazione e selezione](docs/protocollo.md) | Qualità e distribuzione dinamica, generazione, metadati, punteggio editoriale, controlli periodici, motivazioni |
| [Live](docs/live.md) | Durata minima, scorta di domande, rotazione, checklist di preparazione della live |
| [Categorie sperimentali](docs/CATEGORIE_SPERIMENTALI.md) | Categorie editoriali da provare e sovrapposizioni da risolvere prima dell'approvazione |

---

## Filosofia delle domande

**Non aumentare indiscriminatamente la cattiveria: aumenta la difficoltà della scelta.** L'obiettivo è costruire domande facili da capire, difficili da scegliere e interessanti da discutere. La forza di un dilemma nasce dall'equilibrio delle alternative, dalla sorpresa, dalle conseguenze e dal conflitto psicologico o morale; non dipende soltanto da volgarità, disgusto o provocazione.

La domanda ideale produce un **conflitto autentico**: anche quando i due scenari sono assurdi, ciascuno offre un motivo plausibile per essere scelto e un motivo plausibile per essere evitato. Una reazione forte non richiede necessariamente una situazione estrema. Misurare soprattutto la capacità di dividere il pubblico e generare una discussione, senza richiedere confessioni reali.

---

## Formato e vincoli

Ogni domanda è un "preferiresti" a due opzioni, destinato al CSV di Livecade.

> **Regola inamovibile: categorie e intensità non sono modificabili.**
> I 14 valori di `category` e i 2 valori di `intensity` (`light`, `tough`) sono fissi. Non si aggiungono, rinominano, traducono, uniscono o eliminano valori, nemmeno in via temporanea o sperimentale. Questa regola non si deroga e non si rimette in discussione: nuovi livelli, sottolivelli o etichette creative (es. "preferirei morire", `insopportabile`, macrotemi) restano nei metadati editoriali interni e non entrano mai nel CSV.

| Parametro | Regola |
| --- | --- |
| Formato | Due alternative autonome: ognuna si capisce da sola e l'opzione B non dipende mai dall'opzione A (vedi [Alternative autonome](docs/linee-guida.md#alternative-autonome)) |
| Persona | Seconda persona plurale (*voi*): verbi, pronomi e possessivi al plurale ("il vostro capo", "vi lamentate") |
| Lunghezza | Massimo 90 caratteri per opzione |
| Intensità | Solo `light` o `tough`, nessun altro valore (non modificabile) |
| Categorie | `food`, `money`, `fantasy`, `time-travel`, `school-work`, `social`, `love`, `survival`, `sports`, `fame`, `gross`, `lifestyle`, `silly`, `dilemmas` (non modificabili) |
| Intestazione CSV | `ref,source,language,category,intensity,optionA,optionB` (7 colonne separate da virgole) |
| Lingua | `it` |
| Codifica consigliata | UTF-8 (eventualmente UTF-8 con BOM per Excel) |
| Pubblico | Adulti, anche in live; le domande sessualmente esplicite restano fuori dalle live |
| Terza opzione | Nessuna: la scelta è sempre obbligatoria |

Le categorie sono **vincoli tecnici**, non i nomi dei filoni creativi: non inserire nel campo `category` valori come `Spicy`, `Hot`, `Insopportabile` o `Piccante/Hot/Tabù`. Il CSV conserva le sette colonne indicate; le classificazioni creative restano nella guida o in un archivio interno separato.

Il conteggio dei 90 caratteri include spazi, accenti e punteggiatura: vale **separatamente** per `optionA` e `optionB`. Verificare anche che `ref` sia univoco e che entrambi i testi siano valorizzati.

**Esportazione affidabile:** scrivere il CSV con un esportatore conforme alle regole CSV, non concatenando manualmente i campi con virgole; usare correttamente le virgolette per testi contenenti virgole, virgolette o ritorni a capo. Per gli import, evitare ritorni a capo nelle opzioni. Testare il file con una reimportazione, controllando il numero esatto di righe e colonne. Non aggiungere `A.`, `B.`, `Preferiresti` o `Preferireste` dentro le opzioni se l'interfaccia li mostra già.

**Separatori e spazi:** non introdurre spazi aggiuntivi *fuori dai campi* prima o dopo le virgole separatrici (es. `love,tough`, non `love, tough`). Non eliminare gli spazi che fanno legittimamente parte dei testi delle opzioni: una virgola interna al testo è consentita e richiede la corretta quotatura CSV. Validare sempre i valori parsati, non solo l'aspetto del file aperto come testo.

---

## Categorie editoriali

Le categorie editoriali sono un secondo livello di classificazione, più preciso delle 14 categorie CSV: servono a generare le domande, organizzare l'archivio e filtrare le scalette. **Non sono valori del CSV.** Per la [regola inamovibile](#formato-e-vincoli), ogni domanda esportata conserva nel campo `category` uno dei 14 valori Livecade; la categoria editoriale si registra solo nei metadati interni (`categoria_editoriale`).

### Direttiva di generazione

- Ogni categoria editoriale ha una categoria CSV di riferimento, ma la categoria CSV finale si decide sempre dal contenuto dominante della singola domanda.
- Valgono tutte le regole delle [linee guida](docs/linee-guida.md): alternative autonome, seconda persona plurale, massimo 90 caratteri, equilibrio e limiti di contenuto.
- Nessuna quota: una categoria editoriale cresce solo con domande che superano la stessa [selezione editoriale](docs/protocollo.md).
- Se due categorie editoriali si sovrappongono, si usa quella più specifica rispetto al contenuto.
- `spicy` e `deep` servono anche da filtri di scaletta: si esclude `spicy` quando la live richiede prudenza e si usa `deep` come pausa tra i picchi.

### Categorie approvate

| Categoria editoriale | Contenuto | CSV di riferimento | Altre CSV | Attenzioni |
| --- | --- | --- | --- | --- |
| `spicy` | Flirt, desideri e situazioni intime tra adulti consenzienti | `love` | `silly` | Può essere esplicita solo fuori dalla live (tag `esplicito`); in live sempre allusiva |
| `deep` | Domande riflessive su identità, memoria, valori e scelte di vita | `dilemmas` | `fantasy`, `time-travel`, `lifestyle` | Di norma `light` |
| `family` | Parenti, suoceri, pranzi della domenica, feste comandate, eredità | `social` | `food`, `love`, `dilemmas` | |
| `tech` | Smartphone, IA, social, notifiche, privacy, vita digitale | `lifestyle` | `fame`, `social`, `silly` | |
| `travel` | Voli, hotel, compagni di viaggio, vacanze rovinate | `lifestyle` | `survival`, `money`, `silly` | |
| `pop-culture` | Serie, videogiochi, fandom, spoiler, fenomeni pop | `lifestyle` | `fame`, `silly`, `social` | Preferire riferimenti generici ("la vostra serie preferita") a titoli specifici |
| Paranormale Comico & Misteri | Fantasmi, case infestate, UFO, misteri irrisolti in chiave comica | `fantasy` | `silly`, `survival` | Comico, mai horror grafico |
| Clima, Stagioni & Meteo Personale | Caldo e freddo estremi, stagioni eterne, un meteo che vi segue | `lifestyle` | `silly`, `fantasy`, `survival` | |
| Epoche & Nostalgia | Vivere in altre epoche, mode e oggetti del passato, nostalgia | `time-travel` | `lifestyle`, `silly` | |
| Voce, Lingua & Tic Verbali | Voce, accenti, intercalari, lingue, parlare in modi impossibili | `silly` | `social`, `school-work` | Niente prese in giro di accenti o dialetti come stereotipo |
| Traffico, Mezzi & Spostamenti | Auto, parcheggi, navigatori, code, mezzi privati | `lifestyle` | `survival`, `silly`, `money` | |
| Trasporti & Pendolarismo da Incubo | Treni, metro, autobus, ritardi, pendolarismo | `lifestyle` | `school-work`, `survival` | |
| Età, Giovinezza & Invecchiamento | Tornare giovani, invecchiare di colpo, l'età giusta per fare qualcosa | `time-travel` | `lifestyle`, `fantasy`, `dilemmas` | Niente malattie né stereotipi anagrafici |
| Crimine Perfetto & Fuga | Colpi impossibili, evasioni e fughe rocambolesche | `survival` | `silly`, `money`, `dilemmas` | Solo finzione comica: nessun metodo realistico, nessuna confessione |
| Scuola, Esami & Università | Interrogazioni, esami, professori, compagni, ricordi di scuola | `school-work` | `social`, `time-travel` | Solo ricordi da adulti o università; mai combinata con `spicy` |
| Tifo & Fede Sportiva | Squadra del cuore, derby, rivalità tra tifosi | `sports` | `social`, `fame` | Squadra generica, mai insulti a tifoserie reali |
| Arte, Musica & Talento | Suonare, cantare, dipingere, esibirsi | `lifestyle` | `fame`, `fantasy`, `silly` | |
| Estetica, Look & Apparenza | Vestiti, capelli, tatuaggi, mode, prime impressioni | `lifestyle` | `social`, `fame`, `silly` | Solo ciò che si può cambiare, mai difetti fisici |
| Burocrazia & Attese Infernali | Uffici pubblici, moduli, code, call center, timbri | `lifestyle` | `school-work`, `money`, `silly` | |
| Giochi, Sfide & Competizioni Assurde | Giochi da tavolo, quiz, sfide tra amici, tornei improbabili | `silly` | `sports`, `social`, `money` | |
| Arte, Creatività & Riconoscimento | Opere, merito, plagio, critica, successo tardivo | `fame` | `money`, `dilemmas` | |
| Universi Paralleli & Vite Alternative | Altre versioni di voi, vite non scelte, mondi alternativi | `fantasy` | `time-travel`, `dilemmas` | |
| Acquisti, Truffe & Abbonamenti | Saldi, acquisti sbagliati, abbonamenti impossibili da disdire, truffe subite | `money` | `lifestyle`, `silly` | Le truffe si subiscono in chiave comica, non si spiegano |
| Galateo & Convenzioni Sociali | Buone maniere, regole non scritte, imbarazzi di etichetta | `social` | `food`, `school-work` | |
| Natura & Vita Selvaggia | Campeggio, animali selvatici, natura estrema, vita all'aperto | `survival` | `lifestyle`, `gross` | |

**Collegamenti con i macrotemi:** `spicy`, `family`, `tech`, `travel` e `pop-culture` corrispondono ai macrotemi Spicy & Sotto le Lenzuola, Famiglia & Parenti, Tecnologia & Dipendenze Digitali, Viaggi & Vacanze e Spoiler, Fandom & Cultura Pop; `deep` raccoglie Grandi Domande e Identità & Ricordi. *Scuola, Esami & Università*, *Tifo & Fede Sportiva*, *Arte, Musica & Talento* ed *Estetica, Look & Apparenza* sono i candidati delle linee guida, ora promossi a definitivi. *Crimine Perfetto & Fuga* affianca il sottogenere definitivo *Crimine & Giustizia*: il primo riguarda colpi ed evasioni comiche, il secondo colpe, processi e giustizia immaginari, sempre senza confessioni vere.

**Confini tra categorie vicine:**

- *Traffico, Mezzi & Spostamenti* riguarda i mezzi privati; *Trasporti & Pendolarismo da Incubo* quelli pubblici.
- *Arte, Musica & Talento* riguarda il saper fare; *Arte, Creatività & Riconoscimento* quello che succede all'opera (merito, plagio, fama).
- *Universi Paralleli & Vite Alternative* riguarda altre versioni di voi; `deep` la riflessione sui valori; il Caos temporale i paradossi e i viaggi nel tempo.
- *Galateo & Convenzioni Sociali* riguarda regole reali di buone maniere; *Unpopular Opinion* le opinioni; *Regole Sociali Umilianti* regole inventate e assurde.
- *Natura & Vita Selvaggia* riguarda l'ambiente e gli animali selvatici; *Animali & Convivenza Assurda* gli animali domestici e le situazioni comiche.
- *Epoche & Nostalgia* riguarda un periodo storico; *Età, Giovinezza & Invecchiamento* la vostra età.

### Nuove proposte

Categorie che non si sovrappongono né alle 14 categorie CSV né ai macrotemi né alle categorie approvate. Da provare prima di approvarle.

| Categoria editoriale | Contenuto | CSV di riferimento | Altre CSV | Perché è nuova |
| --- | --- | --- | --- | --- |
| Futuro & Spazio | Colonie su Marte, vita nel 3000, robot domestici, viaggi spaziali | `fantasy` | `survival`, `lifestyle` | `tech` riguarda il presente e il Caos temporale i paradossi: il futuro lontano non è coperto |
| Mestieri Insoliti & Lavori Impossibili | Lavori strani, estremi o inventati, una giornata in un mestiere improbabile | `school-work` | `silly`, `money`, `gross` | Ufficio & Carriera riguarda la vita d'ufficio, non il tipo di lavoro |
| Città, Paesi & Luoghi dove Vivere | Metropoli o paesino, isole, case insolite, vivere per sempre in un posto | `lifestyle` | `survival`, `money` | Casa riguarda la convivenza, `travel` i soggiorni temporanei |
| Tempo, Orari & Puntualità | Ritardi, sveglie, giornate più lunghe o più corte, essere sempre in anticipo | `lifestyle` | `silly`, `school-work`, `time-travel` | Riguarda il tempo quotidiano, non il passato o il futuro |
| Nomi & Soprannomi | Soprannomi imbarazzanti, nomi da cambiare, essere chiamati per sempre in un certo modo | `silly` | `social`, `fame` | Nessun tema copre oggi nomi e soprannomi; mai nomi di persone reali né soprannomi offensivi |
| Regali & Sorprese | Regali sbagliati, riciclo dei regali, sorprese indesiderate, pacchi misteriosi | `social` | `money`, `love` | Feste riguarda l'evento e Acquisti la spesa: il regalo come gesto non è coperto |

---

## Checklist della domanda

Una domanda entra nel CSV solo se supera tutti i controlli **e** la selezione editoriale. Il punteggio non sostituisce i vincoli obbligatori.

1. Ogni opzione ha **al massimo** 90 caratteri, contando spazi e punteggiatura?
2. Ogni opzione si capisce da sola e l'opzione B non dipende mai dall'opzione A?
3. Verbi, pronomi e possessivi sono alla seconda persona plurale (*voi*)?
4. Nessuna delle due domina chiaramente l'altra per il pubblico di riferimento, considerando gravità, durata, probabilità e reversibilità?
5. L'opzione resta equilibrata anche cambiando genere, reddito, relazione sentimentale o contesto di chi gioca, oppure il pubblico è stato definito esplicitamente?
6. Ha almeno un meccanismo riconoscibile tra i **16**?
7. Se usa il **Dilemma Insopportabile**: entrambe le opzioni sono da rifiutare, concrete, equilibrate, narrativamente efficaci e senza scappatoie, e c'è almeno un secondo meccanismo concreto?
8. Provoca almeno una reazione chiara: risata, imbarazzo, disgusto, sorpresa, curiosità o riflessione?
9. La categoria rispecchia il contenuto dominante e l'intensità (`light` o `tough`) corrisponde al disagio che provoca?
10. Se contiene riferimenti sessualmente espliciti: riguarda solo adulti consenzienti ed è marcata `esplicito`, così resta fuori dalle live?
11. È diversa dalle domande **dell'intero archivio** per concetto, non soltanto per parole o inversione A/B?
12. Ha superato la **valutazione editoriale** (soglia iniziale 4/5) oppure è stata rivalutata e motivatamente approvata?
13. È stata ammessa per la sua **qualità**, non per raggiungere una quota di categoria o intensità? Contribuisce alla varietà tematica, meccanica o emotiva?

---

## Checklist del file CSV

Da controllare su tutto il file prima di ogni importazione su Livecade.

1. Il file ha esattamente le sette colonne `ref,source,language,category,intensity,optionA,optionB`?
2. Ogni `ref` è valorizzato e univoco?
3. `language` è sempre `it` e tutti i campi richiesti sono valorizzati?
4. Ogni `category` è tra i 14 valori ammessi e ogni `intensity` è esattamente `light` o `tough`?
5. Nessuna opzione supera i 90 caratteri o contiene ritorni a capo?
6. I separatori non hanno spazi aggiunti prima o dopo (`social,tough`, non `social, tough`), salvo gli spazi interni ai campi quotati?
7. Il file è stato esportato con un esportatore CSV e riletto con un parser, con lo stesso numero di righe e colonne e con virgole e virgolette nei campi gestite correttamente?
