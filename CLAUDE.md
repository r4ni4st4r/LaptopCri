# LaptopCri — Ricerca laptop

Progetto di ricerca e confronto offerte per l'acquisto di un laptop. Nessun codice: solo raccolta dati, confronto e classifica.
Lingua di lavoro: **italiano**. Mercato: **solo negozi italiani, prezzi in € IVA inclusa, budget massimo 1.200 €, acquisto con Carta del Docente** (vedi "Vincoli di acquisto").

## ⭐ FONTI PRIMARIE E PUNTO DI PARTENZA (leggere per primo)

**Le fonti primarie di questo progetto sono i file `.md` del repository git, non il web e non la memoria della chat.**

| Priorità | File | Ruolo |
|---|---|---|
| 1 | `CLAUDE.md` | Regole: requisiti, vincoli, CPU ammesse, criteri di punteggio, negozi validi |
| 2 | `data/statoRicerca.md` | **Punto di partenza**: stato attuale, decisioni prese, cosa resta da fare, modelli da tenere d'occhio, trappole note |
| 3 | `data/elencoOfferte.md` | Ultima classifica valida, con schede tecniche, prezzi datati, esclusi e fonti web |

**Procedura obbligatoria per ogni nuova sessione:**
1. `git pull`, poi leggere i tre file nell'ordine indicato. **Non si rifanno da capo** ricerche già documentate e non si rimettono in discussione decisioni già registrate, a meno che l'utente lo chieda.
2. Lo stato descritto nei file è la **base di confronto**. Le nuove ricerche online servono **solo a trovare novità rispetto a quello stato**:
   - il candidato principale è tornato disponibile, o il suo prezzo è cambiato?
   - i "modelli da tenere d'occhio" sono scesi sotto i 1.200 € o sono comparsi in un negozio accreditato?
   - sono uscite offerte o modelli nuovi che rispettano tutti i vincoli?
   - ci sono punti aperti della lista "Cosa resta da fare" che si possono chiudere?
3. Le pagine web (negozi, recensioni, PSREF) sono **fonti secondarie**: si citano nei file con link e data di rilevazione. Ciò che conta è che il risultato venga riportato nei `.md`.
4. A fine sessione si aggiornano i file (vedi "Repository e continuità") e si fa commit, così la sessione successiva riparte dal punto più aggiornato.

Se un'informazione trovata online contraddice un file, si verifica, si aggiorna il file indicando data e fonte, e si annota il cambiamento nella cronologia di `data/statoRicerca.md`.

## Requisiti dell'utente

| Requisito | Priorità | Note |
|---|---|---|
| CPU **minimo AMD Ryzen AI 7 350** (vincolo rigido, pensato per durare nel tempo) | Obbligatoria | Vedi "CPU ammesse" sotto. Nulla al di sotto del Ryzen AI 7 350 |
| GPU dedicata | **Esclusa: solo grafica integrata** | iGPU Radeon 840M/860M sufficiente. I portatili con GPU dedicata (gaming/creator con RTX) **non si considerano**. Il 2026-11-11 è stata proposta l'apertura alla dGPU per allargare il campo, ma l'utente l'ha **respinta** |
| Affidabilità | Alta | Preferire linee business (ThinkPad, EliteBook/ProBook, ExpertBook), garanzia lunga, chassis robusto, aggiornamenti BIOS |
| Autonomia | Alta | Basarsi su test misurati (Notebookcheck Wi-Fi websurfing v1.3), non sulle dichiarazioni del produttore |
| RAM 16 GB DDR5 **espandibile** | Obbligatoria | Serve SO-DIMM (ideale 2 slot, 1 libero). RAM saldata (LPDDR5/LPDDR5X) = **esclusione** |
| Storage 512 GB – 1 TB **espandibile** | Alta | M.2 NVMe sostituibile; ideale 2 slot M.2 |
| Schermo | Bassa | Si può risparmiare: 14" WUXGA IPS 60 Hz va benissimo |

### CPU ammesse (vincolo rigido)

| Ammesse ✅ | Escluse ❌ (anche se "equivalenti" in multi-core) |
|---|---|
| Ryzen AI 7 350 / AI 7 PRO 350 (8C/16T Zen 5, NPU 50 TOPS) | Ryzen AI 5 340 / PRO 340 (6C), Ryzen AI 5 330 (4C) |
| Ryzen AI 7 PRO 360, Ryzen AI 9 365 / HX 370 / HX 375 | Ryzen AI 7 345, Ryzen AI 7 445 (6C), Ryzen AI 5 430/435/440 |
| Ryzen AI 7 450 / AI 7 PRO 450 e superiori Ryzen AI 400 (≥ 8 core) | Tutta la serie Zen 4: Ryzen 200 (220/230/250), 8840HS/U, 7000/8000 |
| | Qualsiasi CPU senza NPU Copilot+ |

Regola: **8 core Zen 5 (o più recenti) + NPU ≥ 50 TOPS**. Nel dubbio verificare core/thread sul sito AMD.

## Vincoli di acquisto (OBBLIGATORI — un'offerta che non li rispetta non entra in classifica)

1. **Solo negozi italiani** (sito .it / sede in Italia, spedizione in Italia, prezzi in € IVA inclusa). Niente Bechtle DE/AT, galaxus, LDLC ecc.
2. **Prezzo massimo 1.200 €** IVA e spedizione incluse. È un tetto rigido: 1.201 € = fuori. Le offerte appena sopra (≤ 1.250 €) si annotano solo in "Quasi in budget".
3. **Pagabile con la Carta del Docente.** Regole da rispettare:
   - Il negozio deve essere esercente accreditato e il prodotto deve rientrare nella categoria "Hardware e Software" (notebook ammessi).
   - **Marketplace esclusi**: su MediaWorld vale solo "venduto e spedito da MediaWorld", su Amazon solo "venduto e spedito da Amazon" (i venditori terzi non accettano il buono). Stessa verifica su Unieuro.
   - Il buono 2025/26 vale **383 €** (DM 59/2026): la differenza va pagata a parte → serve un negozio che consenta il **pagamento misto** (buono + bonifico/carta).
   - Dal 2025/26 l'hardware si può comprare con la Carta **solo alla prima erogazione e poi ogni 4 anni**: l'utente deve verificare di averne diritto sul portale cartadeldocente.istruzione.it.
   - ⚠️ **PUNTO BLOCCANTE (scoperto il 2026-11-11):** per chi riceveva già la Carta, il 2025/26 era la "prima finestra utile" e **si è chiusa il 31/08/2026**; la prossima sarà nel **2029/30**. Neanche i residui 2025/26, spendibili fino al 31/08/2027, valgono per l'hardware. Fa eccezione solo chi riceve la Carta **per la prima volta nel 2026/27** (es. neoassunti o primi incarichi), ma l'importo e la piattaforma 2026/27 sono attesi entro il 30/01/2027. Fonti: FAQ MIM citate da OrizzonteScuola (2026-06-18) e Orizzonte Docenti (2026-09-01). **Prima di qualsiasi acquisto con la Carta, la situazione personale va verificata sul portale.**
   - ✅ **Situazione dell'utente (confermata il 2026-11-11):** è la **prima volta** che riceve la Carta del Docente, quindi rientra nell'eccezione e può comprare il notebook nell'anno della prima erogazione (2026/27). **Vincolo di tempo:** la Carta 2026/27 non è ancora attiva (decreto atteso entro il 30/01/2027), quindi l'acquisto con il buono sarà possibile **solo dopo l'attivazione**, verosimilmente tra febbraio e marzo 2027. Fino ad allora la ricerca resta in modalità monitoraggio: si seguono prezzi e disponibilità, ma non si compra.
4. Indicare sempre per ogni offerta: negozio, venditore effettivo, prezzo, data di rilevazione, disponibilità, modalità d'uso della Carta del Docente.

### Negozi verificati per la Carta del Docente (stato al 2026-11-11)

Fonte da consultare sempre per nuovi esercenti: l'**elenco degli esercenti aderenti** sul portale ministeriale cartadeldocente.istruzione.it (ricerca per provincia e categoria "Hardware e Software"), compresi i **negozi fisici di Genova** che potrebbero non avere un sito.

| Negozio | Accetta Carta Docente | Come funziona / limiti |
|---|---|---|
| **Amazon.it** | **Sì** (confermato dall'utente il 2026-11-11) | Solo prodotti **nuovi, venduti e spediti da Amazon**. Esclusi venditori terzi e usato/Warehouse |
| **Giannone Computers** | **Sì** (segnalato dall'utente; "Carta del Docente" tra i metodi di pagamento dello shop, verificato il 2026-11-11) | Asus Gold Store a Modica (RG), via Vanella Macallè 5, tel. 0932 906688. Shop online: shop.giannonecomputers.it (pagamenti: carta, PayPal, Klarna, bonifico, Carta del Docente). I prodotti hanno per nome il codice modello: si cerca per **codice SKU**, non per CPU (`index.php?route=product/search&search=<codice>&source=nuh&category_id=0`). Da includere sempre nella ricerca |
| **Lenovo.com/it** | Sì | Registrarsi su Lenovo Istruzione (prezzi riservati), mettere il prodotto nel carrello, inviare buono a `cartadocente@lenovo.com`; differenza via **bonifico**; risposta entro 2 giorni lavorativi |
| **IT-Partners (it-partners.it)** | Sì | Metodo di pagamento "Carta del Docente" al checkout, invio PDF del buono; differenza via **bonifico**; prezzi IVA inclusa |
| **MediaWorld** | Sì, solo prodotti venduti da MediaWorld | Online scegliere "Ritiro e pagamento in negozio" e presentare buono + documento + codice fiscale; **marketplace escluso** (quasi tutti i notebook business su mediaworld.it sono marketplace) |
| **Unieuro** | Sì (secondo guide 2026; da confermare in negozio) | Categoria PC/notebook ammessa; verificare pagamento misto e cumulabilità con promo Unieuro Club |
| **Campustore** | Sì | Catalogo notebook molto ridotto |
| **Reware** | Sì | Solo ricondizionati; differenza con carta/PayPal/bonifico. Al 2026-11-11 nessun modello con CPU ammessa (verificato dall'utente) |
| Yeppon | **No** (non tra i metodi di pagamento) | — |
| **Euronics** | **Sì** (pagina ufficiale euronics.it/carta-del-docente.html, verificata il 2026-11-11) | Online: metodo "Carta del docente" in "Pagamento e fatturazione", **un solo buono per ordine**, differenza con carta o PayPal. In negozio: si porta il buono. Al 2026-11-11 nessun modello con CPU ammessa (verificato dall'utente). Il sito blocca la consultazione automatica (Cloudflare) |

## Criteri di punteggio (totale 100)

| Criterio | Punti | Come si assegna |
|---|---|---|
| CPU | 10 | 10 = Ryzen AI 7 350 / PRO 350 / AI 7 450; 10 anche per CPU superiori (nessun bonus: la GPU/CPU extra non serve). CPU sotto il 350 = **esclusione**, non punteggio basso |
| RAM | 20 | 20 = DDR5 SO-DIMM 2 slot con 1 libero (max ≥ 64 GB); 15 = 2 slot ma entrambi occupati (2×8); 10 = 1 slot + saldata; 0 = tutta saldata (esclusa) |
| Storage | 15 | 15 = 2 slot M.2; 11–12 = 1 slot M.2 2280 sostituibile; meno se 2230/2242 o non sostituibile |
| Autonomia | 25 | Da test Wi-Fi Notebookcheck: ≥ 15 h = 25; 14 h ≈ 22; 13 h ≈ 21; 12 h ≈ 18; 10 h ≈ 14. Se non misurata: stima da Wh (≈ 0,2 h/Wh per Krackan Point) con penalità di incertezza |
| Affidabilità | 20 | Linea di prodotto, materiali, garanzia (36 mesi = bonus), riparabilità, storico del marchio, voto recensioni |
| Prezzo | 10 | Sotto i 1.200 € (vincolo): 10 = ≤ 850 €, 8 = ≤ 1.000 €, 6 = ≤ 1.150 €, 5 = ≤ 1.200 € |

GPU dedicata: **esclusione** (non punteggio basso).

Disponibilità: un'offerta "non disponibile online" resta in classifica ma va segnalata con ⚠️ e non può essere la raccomandazione principale.

## Repository e continuità (fonte di verità)

I file `.md` di questo progetto, versionati in un **repository git**, sono l'**unica fonte di verità** della ricerca. Non affidarsi alla memoria della chat o a note locali: chi riprende il lavoro, anche da un altro PC, deve trovare tutto nel repository.

**All'inizio di ogni sessione:**
1. `git pull` per avere la versione più aggiornata.
2. Leggere nell'ordine: `CLAUDE.md` → `data/statoRicerca.md` → `data/elencoOfferte.md`.
3. Ripartire dalla sezione "Cosa resta da fare" di `data/statoRicerca.md`.

**Durante e alla fine di ogni sessione:**
1. Aggiornare `data/elencoOfferte.md` (classifica, schede, prezzi con data) e incrementare il numero di ricerca.
2. Aggiornare `data/statoRicerca.md`: cronologia delle decisioni, nuove scoperte o trappole, stato del candidato principale, "Cosa resta da fare".
3. Se cambiano requisiti, vincoli o regole, aggiornarli **qui in CLAUDE.md** (non solo nella chat).
4. Fare commit con un messaggio descrittivo (es. `Ricerca n. 4: verificato Euronics, aggiornati prezzi`) e `git push`, **solo dopo conferma dell'utente**.

**Regole:**
- Ogni informazione utile emersa in chat (preferenze dell'utente, decisioni, negozi verificati) va scritta in un file `.md` prima di chiudere la sessione.
- Niente dati sensibili nei file: no codici della Carta del Docente, no credenziali, no dati personali oltre alla zona di ricerca (Genova).
- Le date vanno sempre in formato assoluto (AAAA-MM-GG).

## Struttura dei file

- `CLAUDE.md`: questo file, con requisiti, vincoli, criteri di punteggio e regole di lavoro.
- `data/statoRicerca.md`: **diario e passaggio di consegne**, con riepilogo, cronologia delle decisioni, negozi verificati, trappole, modelli da tenere d'occhio, tecniche di ricerca e cosa resta da fare.
- `data/elencoOfferte.md`: **archivio delle offerte**, con classifica, scheda tecnica completa di ogni laptop, esclusi con motivo e fonti.

### Formato di ogni scheda in `data/elencoOfferte.md`

Ogni laptop deve avere tutti questi campi (scrivere `n.d.` o `da verificare` se mancanti, mai inventare):
modello e codice SKU · CPU (core/thread) · iGPU · RAM (tipo, velocità, slot, max) · storage (capacità, formato M.2, PCIe, n. slot) ·
display · batteria (Wh) · autonomia misurata/stimata · alimentatore (W, tipo connettore) · consumi (idle/carico) · peso (+ alimentatore) ·
dimensioni · porte · wireless · materiali/costruzione · garanzia · manutenibilità · voto recensioni · prezzo (€, negozio, data) · punteggio · pro/contro · fonti.

## Regole di lavoro

1. **Verificare sempre la RAM**: molte versioni consumer con Ryzen AI 300 usano LPDDR5X saldata. Controllare scheda tecnica (PSREF Lenovo, QuickSpecs HP, sito ASUS) o recensione. Anche lo stesso modello può cambiare tra SKU (es. batteria 48 vs 64 Wh sull'E14 G8).
2. **Autonomia**: citare sempre la fonte e il test (Wi-Fi websurfing, video, carico). Distinguere chiaramente *misurata* da *stimata*.
3. **Prezzi**: indicare sempre negozio, venditore effettivo, data di rilevazione e se IVA inclusa. Prezzi esteri non ammessi in classifica; tastiera non italiana va segnalata.
4. **Aggiornamenti**: quando si aggiunge o aggiorna un'offerta, ricalcolare il punteggio e riordinare la classifica; aggiornare la data in testa al file. Le offerte scadute vanno spostate nella sezione "Archivio / non più disponibili", non cancellate.
5. **Esclusi**: i modelli scartati vanno elencati nella sezione "Esclusi" con il motivo, per non ri-analizzarli.
6. Contesto mercato (nov 2026): crisi dei prezzi della memoria → la RAM aggiuntiva costa cara; i modelli con slot libero permettono di comprare 16 GB ora ed espandere dopo.
