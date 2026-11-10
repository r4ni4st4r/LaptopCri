# Stato della ricerca — diario e memoria di progetto

> File di passaggio di consegne: contiene **tutto ciò che serve per riprendere la ricerca da zero**, anche da un altro PC o in una nuova sessione.
> Ordine di lettura per ripartire: [CLAUDE.md](../CLAUDE.md) → questo file → [elencoOfferte.md](elencoOfferte.md).
> **Questo file è il punto di partenza**: le nuove ricerche online cercano solo novità rispetto allo stato descritto qui (sezioni 4, 7 e 9).

**Ultimo aggiornamento:** 2026-11-10 (sessione 1, ricerche n. 1–3)

---

## 1. In una riga

Cerco un portatile con **almeno Ryzen AI 7 350**, RAM DDR5 **SO-DIMM espandibile**, SSD espandibile, buona autonomia, affidabile, **max 1.200 €**, da **negozio italiano** e **pagabile con la Carta del Docente**. Al 2026-11-10 l'unica offerta che rispetta tutto è il **Lenovo IdeaPad Slim 5 14AKP10 (83HX006FIX) a 799 € su Unieuro**, che però è **esaurito**.

## 2. Requisiti e vincoli (riassunto; il dettaglio è in CLAUDE.md)

| Voce | Valore deciso | Note / perché |
|---|---|---|
| CPU | **Minimo Ryzen AI 7 350** (8 core Zen 5 + NPU 50 TOPS) | L'utente vuole una macchina "per il futuro": niente Zen 4 (8840HS, Ryzen 200), niente CPU a 4–6 core (AI 5 340, AI 7 345/445, AI 5 430/440) |
| GPU | Integrata | GPU dedicata non richiesta, anzi è un difetto per consumi e calore |
| RAM | 16 GB DDR5 minimo, **SO-DIMM** | RAM saldata (LPDDR5/LPDDR5X) = esclusione. Mezza saldata = penalità forte |
| Storage | 512 GB – 1 TB, M.2 sostituibile | Ideale 2 slot M.2 |
| Autonomia | Alta | Preferire test misurati Notebookcheck (Wi-Fi websurfing) |
| Affidabilità | Alta | Linee business preferite; alluminio/MIL-STD sono un plus |
| Schermo | Bassa priorità | Va bene 14" WUXGA IPS 60 Hz 300 nit |
| Prezzo | **≤ 1.200 €** IVA e spedizione incluse | Tetto rigido |
| Negozio | **Solo italiani** | Niente prezzi esteri (Bechtle DE/AT, galaxus, LDLC…) |
| Pagamento | **Carta del Docente** | Niente marketplace. Buono 383 € + differenza a carico dell'utente |
| Zona utente | Genova | Utile per verificare la disponibilità nei negozi fisici |

## 3. Cronologia delle decisioni

| Data | Ricerca | Cosa è cambiato |
|---|---|---|
| 2026-11-10 | n. 1 | Prima ricerca senza vincoli di negozio e budget: classifica guidata dall'ExpertBook P3 PM3406CKA (Ryzen AI 7 350, 70 Wh, 14 h misurate) |
| 2026-11-10 | n. 2 | Aggiunti i vincoli: negozi italiani, max 1.200 €, Carta del Docente. Scoperto l'IdeaPad Slim 5 14AKP10 a 799 € su Unieuro |
| 2026-11-10 | n. 3 | **CPU minima Ryzen AI 7 350** (rigida). Esclusi ExpertBook PM3406CHA (8840HS), ProBook, E14 Gen 7, IdeaPad 16" con AI 5 340. Verificata la disponibilità a Genova: esaurito, ritiro in negozio disattivato |

## 4. Candidato principale: Lenovo IdeaPad Slim 5 14AKP10 (83HX006FIX)

- **Perché è il migliore:** Ryzen AI 7 350, **32 GB** DDR5-5600 SO-DIMM (2 slot, entrambi occupati), SSD 1 TB M.2 2242 + **secondo slot M.2 2280 libero**, 60 Wh, alluminio, MIL-STD-810H, 1,47 kg, Wi-Fi 7, USB-C 65 W.
- **Prezzo:** 799 € su Unieuro (listino 1.099 €). Negli altri negozi italiani costa ~975–990 € (Yeppon 974,99 €, Dagimarket 985,63 €).
- **Stato al 2026-11-10:** "Non disponibile" online; con il CAP di Genova il ritiro in negozio è disattivato.
- **Prossima azione utente:** telefonare o andare nei negozi Unieuro della zona (elenco e domande da fare in elencoOfferte.md) e attivare "Notifica disponibilità".
- **Promo:** -22% Unieuro Club fino al 12/11/2026 (spesa ≥ 199 €), ~623 €. Da chiedere se si cumula con la Carta del Docente.

## 5. Negozi e Carta del Docente: cosa abbiamo verificato

| Negozio | Esito | Dettagli utili |
|---|---|---|
| **Unieuro** | Accetta (secondo le guide 2026) | Pagamento misto e cumulabilità con le promo da chiedere in negozio. Prodotti esauriti = niente ritiro in negozio online |
| **MediaWorld** | Accetta **solo** prodotti "venduti e spediti da MediaWorld" | Online: "Ritiro e pagamento in negozio" + buono + documento + codice fiscale. **Quasi tutti i notebook business sono di venditori terzi del marketplace** (TecnoPrice, MC Distribuzione, ESSEEFFE COM…) → niente Carta |
| **Lenovo.com/it** | Accetta | Registrarsi a Lenovo Istruzione, prodotto nel carrello, email a `cartadocente@lenovo.com` con il buono; differenza via bonifico; risposta entro 2 giorni lavorativi. I prezzi pubblici con CPU ≥ 350 e SO-DIMM partono da ~1.400 € |
| **IT-Partners** | Accetta | Metodo "Carta del Docente" al checkout, differenza via bonifico, prezzi IVA inclusa. Nulla con CPU ≥ 350 sotto i 1.200 € |
| **Campustore** | Accetta | Catalogo notebook minimo |
| **Reware** | Accetta | Solo ricondizionati (non ancora esplorato) |
| **Yeppon** | **Non accetta** | Metodi: carte, PayPal, Klarna, bonifico |
| **Euronics** | Non verificato | Il sito blocca la consultazione automatica (Cloudflare) |
| **Amazon.it** | Fonti contrastanti | Da evitare |

**Regole Carta del Docente (DM 59/2026):** buono 2025/26 = 383 €; l'hardware si può comprare solo alla prima erogazione e poi **ogni 4 anni**; residui spendibili fino al 31/08/2027 ma con lo stesso vincolo. L'utente deve verificare su cartadeldocente.istruzione.it di poter comprare hardware.

## 6. Cosa abbiamo imparato (trappole da evitare)

1. **RAM saldata ovunque**: la maggior parte dei portatili consumer con Ryzen AI 300 ha LPDDR5X saldata (Zenbook, Vivobook S, Yoga, OmniBook 5, IdeaPad 5 2-in-1, Dell 14/Pro 14 Plus, T14s). Le eccezioni con SO-DIMM sono: **IdeaPad Slim 5 14/16AKP10**, ExpertBook P3, ThinkPad E/L/T14 (non T14s), HP ProBook/EliteBook 6/8 G1a, MSI Venture A16.
2. **Lo stesso modello cambia tra SKU**: batteria (es. ThinkPad E14 G8: 64 Wh testato, 48 Wh sullo SKU italiano), formato SSD, RAM 1×16 o 2×8. Controllare sempre il codice esatto.
3. **Prezzi netti vs lordi**: i prezzi B2B (es. Bechtle) possono essere IVA esclusa. Il "1.075 €" della ricerca 1 era netto (1.328,58 € IVA inclusa).
4. **Nomi ingannevoli**: Ryzen AI 7 345 e AI 7 445 hanno 6 core; Ryzen AI 5 430 ne ha 4. "AI 7" nel nome non garantisce 8 core.
5. **Schede negozio contraddittorie**: es. Vivobook 16 M1607KA, che risulta sia "On-board" sia "2x SO-DIMM". In caso di dubbio fa fede il PSREF Lenovo, i QuickSpecs HP o la scheda ASUS.
6. **Il marketplace MediaWorld è la trappola principale**: lì ci sono prezzi buoni (es. EliteBook 8 G1a Ryzen AI 7 350 a 1.117 €), ma non sono pagabili con la Carta.

## 7. Modelli da tenere d'occhio (se scendono di prezzo o compaiono in un negozio accreditato)

| Modello | CPU | Perché interessa | Ultimo prezzo visto |
|---|---|---|---|
| HP EliteBook 8 G1a 14 (D76LTET / AD4J5ET) | Ryzen AI 7 350 | 2 SO-DIMM, 62 Wh, **14,2 h misurate**, linea business | 1.117–1.180 € (marketplace MediaWorld) |
| ASUS ExpertBook P3 PM3406CKA / PM3606CKA | Ryzen AI 7 350 | 2 SO-DIMM, 2 SSD, 70 Wh, **14 h misurate**, 3 anni di garanzia | 1.202–1.275 € |
| Lenovo IdeaPad Slim 5 16AKP10 con Ryzen AI 7 350 | Ryzen AI 7 350 | Come il 14", batteria fino a 80 Wh | non trovato in Italia |
| ThinkPad T14 Gen 7 AMD | Ryzen AI 7 PRO 450 | 75 Wh, ThinkPad T | 1.546 €+ |
| HP EliteBook 6/8 G2a | Ryzen AI 7 450 | Nuova generazione, SO-DIMM | 1.397 €+ |

## 8. Come cercare in modo efficiente (note tecniche per la prossima sessione)

- **IT-Partners** (Shopify): ricerca rapida con `https://www.it-partners.it/it-it/search/suggest.json?q=<testo>&resources[type]=product&resources[limit]=10`; scheda tecnica completa con `/it-it/products/<handle>.js` (campo `description`, tabella specifiche).
- **MediaWorld**: nella pagina prodotto cercare "Venduto e spedito da …". Se manca il nome di un venditore terzo, è venduto da MediaWorld. Il prezzo è nel JSON `"price"`.
- **Unieuro**: le specifiche sono nel JSON della pagina prodotto (coppie `"featureValues":[{"value":…}],"name":…`): Slot memoria, Fattore di forma memoria, Capacità della batteria. Ricerca: `/online/products?q=<testo>`.
- **Lenovo.com**: ricerca `/it/it/search?text=<testo>`; le schede mostrano "SODIMM" o "saldata" direttamente nell'elenco.
- **Lenovo PSREF**: `psref.lenovo.com/syspool/Sys/PDF/IdeaPad/<Modello>/<Modello>_Spec.html`. È la fonte più affidabile per slot RAM, SSD e batteria.
- **Notebookcheck**: le autonomie misurate sono a metà/fine pagina (oltre 200.000 caratteri); le recensioni .it a volte rispondono 403, la versione .net funziona.
- Siti non consultabili in automatico: Euronics (Cloudflare), alcune pagine notebookcheck.it (403).

## 9. Cosa resta da fare

- [ ] **Utente**: chiamare i negozi Unieuro della zona di Genova per l'IdeaPad Slim 5 14AKP10 (83HX006FIX); attivare "Notifica disponibilità".
- [ ] **Utente**: verificare sul portale Carta del Docente di avere diritto all'acquisto di hardware quest'anno.
- [ ] Verificare Euronics (a mano, dal browser) per l'IdeaPad Slim 5 14AKP10 o altri modelli con Ryzen AI 7 350 e SO-DIMM.
- [ ] Esplorare **Reware** (ricondizionati business con Carta del Docente), se l'utente accetta l'usato garantito.
- [ ] Se l'IdeaPad non si trova: decidere con l'utente quale vincolo allargare (budget fino a ~1.250 € oppure negozi senza Carta del Docente).
- [ ] Creare il repository git e fare il primo commit (vedi CLAUDE.md, "Repository e continuità").
