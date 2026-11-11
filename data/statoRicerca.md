# Stato della ricerca — diario e memoria di progetto

> File di passaggio di consegne: contiene **tutto ciò che serve per riprendere la ricerca da zero**, anche da un altro PC o in una nuova sessione.
> Ordine di lettura per ripartire: [CLAUDE.md](../CLAUDE.md) → questo file → [elencoOfferte.md](elencoOfferte.md).
> **Questo file è il punto di partenza**: le nuove ricerche online cercano solo novità rispetto allo stato descritto qui (sezioni 4, 7 e 9).

**Ultimo aggiornamento:** 2026-11-11 (sessione 2, ricerche n. 4–6)

---

## 1. In una riga

Cerco un portatile con **CPU almeno di livello Ryzen AI 7 350** (AMD Ryzen AI 7 350/450 o Intel Core Ultra serie 3 Panther Lake ≥ 8 core, ammessi dal 2026-11-11), **solo grafica integrata**, RAM DDR5 **SO-DIMM espandibile**, SSD espandibile, buona autonomia, affidabile, **max 1.200 €**, da **negozio italiano** e **pagabile con la Carta del Docente**. L'utente riceve la Carta **per la prima volta** (2026/27), che però non è ancora attiva (attesa entro il 30/01/2027): **l'acquisto avverrà nel 2027**. **Candidato principale al 2026-11-11: ASUS ExpertBook B3 G2 14" B3405CAA-LY0285X (Core Ultra 5 325) da Giannone Computers a 1.154,85 €.**

## 2. Requisiti e vincoli (riassunto; il dettaglio è in CLAUDE.md)

| Voce | Valore deciso | Note / perché |
|---|---|---|
| CPU | **Minimo livello Ryzen AI 7 350**: AMD Ryzen AI 7 350/450 o Intel Core Ultra serie 3 ≥ 8 core (325/335/355/365/356H, serie X) | L'utente vuole una macchina "per il futuro": niente Zen 4 (8840HS, Ryzen 200/260), niente CPU a 4–6 core (AI 5 340, AI 7 345/445, AI 5 430/440), niente Intel Wildcat Lake / Arrow Lake / Lunar Lake. Gli Intel Panther Lake sono stati ammessi il 2026-11-11 dopo l'analisi in processori.md |
| GPU | **Solo integrata** | Il 2026-11-11 un'amica ha proposto di ammettere la GPU dedicata per allargare il campo; l'utente ha **respinto** la proposta |
| RAM | 16 GB DDR5 minimo, **SO-DIMM** | RAM tutta saldata (LPDDR5/LPDDR5X) = esclusione. Metà saldata = penalità forte |
| Storage | 512 GB – 1 TB, M.2 sostituibile | Ideale 2 slot M.2 |
| Autonomia | Alta | Preferire test misurati Notebookcheck (Wi-Fi websurfing) |
| Affidabilità | Alta | Linee business preferite; alluminio/MIL-STD sono un plus |
| Schermo | Bassa priorità | Va bene 14" WUXGA IPS 60 Hz 300 nit |
| Prezzo | **≤ 1.200 €** IVA e spedizione incluse | Tetto rigido |
| Negozio | **Solo italiani** | Niente prezzi esteri (Bechtle DE/AT, galaxus, LDLC…) |
| Pagamento | **Carta del Docente** | Niente marketplace. Buono + differenza a carico dell'utente |
| Situazione Carta | **Prima erogazione nel 2026/27** | Può comprare hardware, ma solo dopo l'attivazione della Carta 2026/27 (decreto atteso entro il 30/01/2027) |
| Zona utente | Genova | Utile per i negozi fisici |

## 3. Cronologia delle decisioni

| Data | Ricerca | Cosa è cambiato |
|---|---|---|
| 2026-11-10 | n. 1 | Prima ricerca senza vincoli di negozio e budget: classifica guidata dall'ExpertBook P3 PM3406CKA (Ryzen AI 7 350, 70 Wh, 14 h misurate) |
| 2026-11-10 | n. 2 | Aggiunti i vincoli: negozi italiani, max 1.200 €, Carta del Docente. Scoperto l'IdeaPad Slim 5 14AKP10 a 799 € su Unieuro |
| 2026-11-10 | n. 3 | **CPU minima Ryzen AI 7 350** (rigida). Esclusi ExpertBook PM3406CHA (8840HS), ProBook, E14 Gen 7, IdeaPad 16" con AI 5 340. IdeaPad esaurito online; con CAP di Genova il ritiro in negozio è disattivato |
| 2026-11-10 | — | Creato il repository git: i file `.md` sono la fonte primaria |
| 2026-11-11 | n. 4 | Note dell'amica integrate: Amazon.it accetta la Carta (solo venduto e spedito da Amazon); aggiunto **Giannone Computers**; **IdeaPad Slim 5 non disponibile in tutta Italia** (verificato dall'utente) → archiviato; Euronics e Reware senza modelli idonei (verificato dall'utente). Proposta GPU dedicata **respinta**. Scoperto il **vincolo dei 4 anni** (finestra hardware chiusa il 31/08/2026 per chi aveva già la Carta); l'utente conferma che è la **prima erogazione** → può comprare dopo l'attivazione della Carta 2026/27. Euronics accetta la Carta (pagina ufficiale). Giannone: unico modello idoneo ≤ 1.200 € è il Vivobook 14 M1407KA a 899 € |
| 2026-11-11 | — | Creato `data/processori.md`: analisi dei 10 processori per laptop migliori per longevità, autonomia e multimedia/design senza GPU dedicata (800–1.200 €). Ne emerge una domanda aperta: ammettere gli Intel Core Ultra 7 355 / 5 325 (Panther Lake) con RAM SO-DIMM come equivalenti al Ryzen AI 7 350 |
| 2026-11-11 | n. 6 (verifica) | Cercata una recensione con l'autonomia dell'ExpertBook B3 G2: **non ne esistono ancora con test misurati**. ASUS dichiara 19–20 h, ma con batterie da 63–70 Wh; in Italia è elencata solo quella da 50 Wh. Il riferimento più vicino (ThinkBook 14 G9, Core Ultra 5 325, 48 Wh) fa **8,7 h** su Notebookcheck → stima **~9–11 h**, punteggio da 85 a 81. Resta comunque il candidato principale |
| 2026-11-11 | n. 6 | **Ammessi gli Intel Core Ultra serie 3 (Panther Lake) ≥ 8 core** (decisione dell'utente). Trovato il nuovo **candidato principale: ASUS ExpertBook B3 G2 14" B3405CAA-LY0285X** (Core Ultra 5 325, 16 GB DDR5 SO-DIMM fino a 96 GB, 3 slot M.2 in totale, 50 Wh, Thunderbolt 4, RJ45, MIL-STD 810H, 3 anni di garanzia) da **Giannone a 1.154,85 €** (85 punti). Anche il 16" B3605CAA-MB0018X a 1.192,55 €. Samsung Galaxy Book6 (Amazon/Unieuro) scartato per RAM saldata |
| 2026-11-11 | n. 5 | **Amazon.it esplorato** (solo venduto da Amazon): con Ryzen AI 7 350 ci sono solo HP OmniBook 5 16 e OmniBook X Flip, entrambi con **LPDDR5X saldata** → nessuna offerta valida. I modelli con SO-DIMM sono venduti solo da terzi (es. Vivobook 14 M1407KA da Giannone a 999,90 € su Amazon, contro 899 € sul suo sito) |

## 4. Situazione attuale e candidati

**Candidato principale (dal 2026-11-11): ASUS ExpertBook B3 G2 14" Intel, B3405CAA-LY0285X (MPN 90NX0A01-M009Y0)**
- **Dove e quanto:** Giannone Computers, **1.154,85 €** IVA inclusa (promo, 55 pezzi). Da IT-Partners costa 1.236,57 €.
- **Perché:** rispetta tutti i vincoli. Core Ultra 5 325, 16 GB DDR5 **SO-DIMM con slot libero fino a 96 GB**, SSD 512 GB più **due slot M.2 liberi** (2280 e 2230), Thunderbolt 4, RJ45, Wi-Fi 7, **MIL-STD 810H**, **3 anni di garanzia ASUS**, 1,45 kg, Windows 11 Pro.
- **Punti deboli:** **autonomia stimata solo ~9–11 h** con la batteria da 50 Wh. Non ci sono test della B3 G2; il riferimento misurato è il ThinkBook 14 G9 con lo stesso Core Ultra 5 325 e 48 Wh: 8,7 h (Notebookcheck). Inoltre schermo base da 300 nit e CPU senza Hyper-Threading. Punteggio sceso da 85 a **81** dopo questa verifica.
- **Prossime azioni:** chiedere a Giannone conferma di prezzo, spedizione, pagamento misto con la Carta e **capacità della batteria** (esistono versioni da 63/70 Wh?); ricontrollare a inizio 2027 se è uscita una recensione misurata; ricontrollare il prezzo quando la Carta 2026/27 sarà attiva.

**Alternative valide ma secondarie:**
- ExpertBook B3 G2 16" B3605CAA-MB0018X, 1.192,55 € da Giannone (82 punti): più grande, senza vantaggi;
- ASUS Vivobook 14 M1407KA-LY053W, 899 € da Giannone (59 punti): RAM in parte saldata, batteria piccola;
- ASUS Vivobook 16 M1607KA-MB053W, 599,90 € da Unieuro (57 punti).

**Ex candidato principale (archiviato il 2026-11-11):** Lenovo IdeaPad Slim 5 14AKP10 (83HX006FIX), Ryzen AI 7 350, 32 GB SO-DIMM, 2 slot SSD, 60 Wh, 799 € su Unieuro. Non disponibile in nessun negozio Unieuro in Italia (verificato dall'utente). Altrove costava ~975–990 € (Yeppon, Dagimarket), in negozi che non accettano la Carta. **Se ricompare ≤ 1.200 € in un negozio accreditato torna subito il n. 1.**

**Strategia (aggiornata il 2026-11-11):** visto che si compra nel 2027, l'ExpertBook B3 G2 14" resta il riferimento da battere. Intanto si **monitorano** i modelli della sezione 7 (ExpertBook P3 PM3406CKA/PM3606CKA, EliteBook 8 G1a, ThinkPad E14 Gen 8 Intel) nel caso scendano sotto i 1.200 € in un negozio accreditato.

## 5. Negozi e Carta del Docente: cosa abbiamo verificato

| Negozio | Esito | Dettagli utili |
|---|---|---|
| **Giannone Computers** | **Accetta** (anche online) | Asus Gold Store, Modica (RG), tel. 0932 906688. Shop: shop.giannonecomputers.it, pagamenti: carta, PayPal, Klarna, bonifico, Carta del Docente. Catalogo ampio (ASUS, HP, Lenovo, Acer) |
| **Amazon.it** | **Accetta** (confermato dall'utente) | Solo prodotti nuovi **venduti e spediti da Amazon**. Esplorato il 2026-11-11: con Ryzen AI 7 350 vende solo HP OmniBook con RAM saldata → **nessun modello idoneo**. Filtro venditore Amazon nell'URL: `&rh=p_6%3AA11IL2PNWYJU7H` |
| **Euronics** | **Accetta** (pagina ufficiale) | Online: un buono per ordine, differenza con carta o PayPal; in negozio con il buono. Nessun modello idoneo al 2026-11-11 (utente) |
| **Unieuro** | Accetta (secondo le guide 2026) | Pagamento misto e promo da chiedere in negozio. Prodotti esauriti = niente ritiro in negozio online |
| **MediaWorld** | Accetta **solo** prodotti "venduti e spediti da MediaWorld" | **Quasi tutti i notebook business sono di venditori terzi del marketplace** → niente Carta |
| **Lenovo.com/it** | Accetta | Lenovo Istruzione + email a `cartadocente@lenovo.com`; differenza via bonifico. Con CPU ≥ 350 e SO-DIMM si parte da ~1.400 € |
| **IT-Partners** | Accetta | Metodo "Carta del Docente" al checkout, differenza via bonifico. Nulla con CPU ≥ 350 sotto i 1.200 € |
| **Campustore** | Accetta | Catalogo notebook minimo |
| **Reware** | Accetta | Solo ricondizionati; nessun modello idoneo al 2026-11-11 (utente) |
| **Yeppon** | **Non accetta** | Metodi: carte, PayPal, Klarna, bonifico |

**Elenco ufficiale esercenti del Ministero:** visibile solo dopo il login SPID/CIE nell'**Area Docenti** di cartadeldocente.istruzione.it (ricerca per provincia e categoria). Claude non può consultarlo: **lo deve fare l'utente**, cercando "Hardware e Software" in provincia di Genova, così da individuare anche **negozi fisici senza sito online**.

**Regole Carta del Docente (DM 59/2026):**
- hardware solo alla **prima erogazione** e poi ogni **4 anni**;
- per chi aveva già la Carta, la finestra 2025/26 si è chiusa il 31/08/2026 e la prossima è nel 2029/30; i residui non valgono per l'hardware;
- per chi la riceve per la **prima volta nel 2026/27** (il caso dell'utente) l'acquisto è consentito nell'anno della prima erogazione;
- importo 2026/27 e attivazione: decreto atteso entro il 30/01/2027 (nel 2025/26 erano 383 €).

## 6. Cosa abbiamo imparato (trappole da evitare)

1. **RAM saldata ovunque**: la maggior parte dei portatili consumer con Ryzen AI 300 ha LPDDR5X saldata (Zenbook, Vivobook S, Yoga, OmniBook 5, IdeaPad 5 2-in-1, Dell 14/Pro 14 Plus, T14s). I Vivobook 14/16 M1407/M1607 hanno **metà saldata + 1 slot**. Le eccezioni con SO-DIMM completo sono: IdeaPad Slim 5 14/16AKP10, ExpertBook P3, ThinkPad E/L/T14 (non T14s), HP ProBook/EliteBook 6/8 G1a/G2a, MSI Venture A16.
2. **Lo stesso modello cambia tra SKU**: batteria (es. ThinkPad E14 G8: 64 Wh testato, 48 Wh sullo SKU italiano), formato SSD, RAM 1×16 o 2×8. Controllare sempre il codice esatto.
3. **Prezzi netti vs lordi**: i prezzi B2B (Bechtle, Giannone) mostrano anche il prezzo IVA esclusa. Usare sempre quello **IVA inclusa**.
4. **Nomi ingannevoli**: Ryzen AI 7 345 e AI 7 445 hanno 6 core; Ryzen AI 5 430 ne ha 4; Ryzen 7 260 è Zen 4. "AI 7" nel nome non garantisce 8 core.
5. **Schede negozio contraddittorie**: es. Vivobook 16 M1607KA, che risulta sia "On-board" sia "2x SO-DIMM". Fa fede la scheda del produttore (PSREF Lenovo, QuickSpecs HP, ASUS).
6. **Il marketplace MediaWorld è la trappola principale**: lì ci sono prezzi buoni (es. EliteBook 8 G1a Ryzen AI 7 350 a 1.117 €), ma non sono pagabili con la Carta. Su Amazon vale la stessa regola (solo "venduto e spedito da Amazon").
7. **L'efficienza di Panther Lake dipende dal portatile**: con lo stesso tipo di processore Notebookcheck ha misurato 8,7 h (ThinkBook 14 G9, Core Ultra 5 325, 48 Wh) e 19,1 h (Dell 14S, Core Ultra 7 355, 70 Wh). Le dichiarazioni dei produttori (fino a 20 h) sono fatte con video a bassa luminosità e batterie più grandi: non usarle mai come stima.
8. **Le offerte spariscono**: l'IdeaPad a 799 € è sparito in un giorno. Quando si trova un'offerta valida e la Carta è attiva, conviene decidere in fretta.

## 7. Modelli da tenere d'occhio (se scendono di prezzo o compaiono in un negozio accreditato)

| Modello | CPU | Perché interessa | Ultimo prezzo visto |
|---|---|---|---|
| ASUS ExpertBook P3 PM3406CKA / PM3606CKA | Ryzen AI 7 350 | 2 SO-DIMM, 2 SSD, 70 Wh, **14 h misurate**, 3 anni di garanzia | **1.299 € da Giannone** (PM3606CKA-MB0184X, accetta la Carta) · 1.202–1.275 € altrove (marketplace) |
| HP EliteBook 8 G1a 14 (D76LTET / AD4J5ET) | Ryzen AI 7 350 | 2 SO-DIMM, 62 Wh, **14,2 h misurate**, linea business | 1.117–1.180 € (solo marketplace MediaWorld) |
| Lenovo IdeaPad Slim 5 14AKP10 (83HX006FIX) | Ryzen AI 7 350 | Ex candidato principale, 32 GB SO-DIMM | 799 € Unieuro (sparito) · ~975 € altrove |
| Lenovo IdeaPad Slim 5 16AKP10 con Ryzen AI 7 350 | Ryzen AI 7 350 | Come il 14", batteria fino a 80 Wh | non trovato in Italia |
| HP EliteBook 6/8 G2a | Ryzen AI 7 450 | Nuova generazione, SO-DIMM | 1.344 €+ (Giannone, MediaWorld, IT-Partners) |
| Lenovo ThinkPad E14 Gen 8 Intel | Core Ultra 5 325 / 7 355 | DDR5 SO-DIMM, 2 slot SSD, ThinkPad | 1.275,72 € (IT-Partners, Ultra 5 325) · 1.079 € (marketplace MediaWorld, non pagabile con la Carta) |
| ASUS ExpertBook B3 G2 con Core Ultra 7 356H | Core Ultra 7 356H (16 core) | Stessa scocca del candidato, CPU più potente | 1.339 € e oltre (Giannone, configurazioni con altra RAM o SSD) |
| ThinkPad T14 Gen 7 AMD | Ryzen AI 7 PRO 450 | 75 Wh, ThinkPad T | 1.546 €+ |

## 8. Come cercare in modo efficiente (note tecniche per la prossima sessione)

- **Giannone Computers**: i prodotti del distributore hanno come nome la **serie + codice** (es. "Expertbook PM3 Series", "1_PM366CKA-MB184X"); quelli con prefisso `2_` hanno la descrizione completa. La ricerca funziona per **nome serie**, non per CPU né per codice: `https://shop.giannonecomputers.it/index.php?route=product/search&search=<testo>&source=nuh&category_id=0&limit=100`. Parole utili: `ExpertBook`, `G2a`, `G1a`, `ProBook`, `EliteBook`, `ThinkPad`, `Vivobook`, `Zenbook`. Mostra prezzi IVA inclusa ed esclusa.
- **Amazon.it**: aggiungere `&i=computers&rh=p_6%3AA11IL2PNWYJU7H` alla ricerca per vedere solo i prodotti venduti da Amazon. Nella pagina prodotto (`/dp/<ASIN>`) il riquadro "Spedizione / Venditore" indica chi vende, e la tabella tecnica riporta "RAM Memory Technology" (LPDDR5x = saldata).
- **IT-Partners** (Shopify): `https://www.it-partners.it/it-it/search/suggest.json?q=<testo>&resources[type]=product&resources[limit]=10`; scheda con `/it-it/products/<handle>.js`.
- **MediaWorld**: nella pagina prodotto cercare "Venduto e spedito da …". Se manca il nome di un venditore terzo, è venduto da MediaWorld. Il prezzo è nel JSON `"price"`.
- **Unieuro**: specifiche nel JSON della pagina prodotto (coppie `"featureValues":[{"value":…}],"name":…`). Ricerca: `/online/products?q=<testo>`.
- **Lenovo.com**: ricerca `/it/it/search?text=<testo>`; le schede mostrano "SODIMM" o "saldata" nell'elenco.
- **Lenovo PSREF**: `psref.lenovo.com/syspool/Sys/PDF/IdeaPad/<Modello>/<Modello>_Spec.html`.
- **Notebookcheck**: autonomie misurate a metà/fine pagina; usare la versione .net se la .it dà 403.
- Non consultabili in automatico: Euronics (Cloudflare), elenco esercenti del Ministero (serve SPID), alcune pagine notebookcheck.it (403).

## 9. Cosa resta da fare

- [ ] **Utente**: entrare nell'Area Docenti (SPID/CIE) e consultare l'elenco esercenti "Hardware e Software" in provincia di Genova; annotare eventuali negozi fisici senza sito.
- [ ] **Utente**: quando esce il decreto 2026/27 (entro il 30/01/2027), verificare l'attivazione della Carta e l'importo.
- [ ] **Utente**: chiedere a Giannone Computers un preventivo per **ExpertBook P3 PM3406CKA** (14", Ryzen AI 7 350) o PM3606CKA sotto i 1.200 € con pagamento tramite Carta del Docente (è un Asus Gold Store).
- [ ] Ricontrollare a inizio 2027 se è uscita una **recensione con l'autonomia misurata** dell'ExpertBook B3 G2 (Notebookcheck, HardwareLuxx). Al 2026-11-11 non ce ne sono: si usa la stima ~9–11 h.
- [ ] **Utente**: chiedere a Giannone (0932 906688) conferma per l'ExpertBook B3 G2 B3405CAA-LY0285X: prezzo, spese di spedizione, disponibilità a inizio 2027, pagamento con Carta del Docente più differenza, **capacità della batteria (50 Wh?) ed eventuale versione da 63/70 Wh**.
- [x] ~~Decidere se ammettere gli Intel Core Ultra serie 3~~: **sì**, ammessi dall'utente il 2026-11-11 (CLAUDE.md aggiornato).
- [ ] Ricontrollare **Amazon.it** solo come monitoraggio (saldi): al 2026-11-11 nessun modello idoneo venduto da Amazon.
- [ ] Verificare la scheda completa ASUS del Vivobook 14 M1407KA-LY053W (batteria, slot M.2, peso).
- [ ] Monitorare periodicamente i modelli della sezione 7 nei negozi accreditati (soprattutto saldi di gennaio 2027).
- [x] ~~Chiamare i negozi Unieuro per l'IdeaPad~~: non disponibile in tutta Italia (utente, 2026-11-11).
- [x] ~~Verificare Euronics~~: accetta la Carta; nessun modello idoneo (2026-11-11).
- [x] ~~Esplorare Reware~~: nessun modello idoneo (utente, 2026-11-11).
- [x] ~~Verificare il diritto all'acquisto di hardware~~: prima erogazione, quindi consentito dopo l'attivazione 2026/27.
- [x] ~~Creare il repository git~~ (2026-11-10).
