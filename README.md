# Would You Rather Questions

Linee guida per scrivere le domande "Preferiresti…" del gioco: controverse, provocatorie, divertenti, imbarazzanti, curiose o riflessive e, quando serve, spietate. Le domande sono pensate per il formato CSV di **Livecade** e per un pubblico adulto, anche in live.

> **Nota:** questa repository contiene contenuti pensati per un pubblico adulto.

## Indice

- [Documentazione](#documentazione)
- [Filosofia delle domande](#filosofia-delle-domande)
- [Formato e vincoli](#formato-e-vincoli)
- [Checklist della domanda](#checklist-della-domanda)
- [Checklist del file CSV](#checklist-del-file-csv)

---

## Documentazione

| File | Contenuto |
| --- | --- |
| [Linee guida di scrittura](docs/linee-guida.md) | Anatomia di una domanda, intensità, meccanismi, macrotemi, aggettivi, tono, glossario per le live, regole di qualità e limiti |
| [Protocollo di generazione e selezione](docs/protocollo.md) | Qualità e distribuzione dinamica, generazione, metadati, punteggio editoriale, controlli periodici, motivazioni |
| [Live](docs/live.md) | Durata minima, scorta di domande, rotazione, checklist di preparazione della live |
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
| Pubblico | Adulti, anche in live |
| Terza opzione | Nessuna: la scelta è sempre obbligatoria |

Le categorie sono **vincoli tecnici**, non i nomi dei filoni creativi: non inserire nel campo `category` valori come `Spicy`, `Hot`, `Insopportabile` o `Piccante/Hot/Tabù`. Il CSV conserva le sette colonne indicate; le classificazioni creative restano nella guida o in un archivio interno separato.

Il conteggio dei 90 caratteri include spazi, accenti e punteggiatura: vale **separatamente** per `optionA` e `optionB`. Verificare anche che `ref` sia univoco e che entrambi i testi siano valorizzati.

**Esportazione affidabile:** scrivere il CSV con un esportatore conforme alle regole CSV, non concatenando manualmente i campi con virgole; usare correttamente le virgolette per testi contenenti virgole, virgolette o ritorni a capo. Per gli import, evitare ritorni a capo nelle opzioni. Testare il file con una reimportazione, controllando il numero esatto di righe e colonne. Non aggiungere `A.`, `B.`, `Preferiresti` o `Preferireste` dentro le opzioni se l'interfaccia li mostra già.

**Separatori e spazi:** non introdurre spazi aggiuntivi *fuori dai campi* prima o dopo le virgole separatrici (es. `love,tough`, non `love, tough`). Non eliminare gli spazi che fanno legittimamente parte dei testi delle opzioni: una virgola interna al testo è consentita e richiede la corretta quotatura CSV. Validare sempre i valori parsati, non solo l'aspetto del file aperto come testo.

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
10. Se va in live: niente di sessualmente esplicito?
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
