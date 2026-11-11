# Processori per laptop — analisi per longevità, autonomia e uso multimediale/design

**Data analisi:** 2026-11-11
**Scopo:** capire quali processori per portatili valgono la pena oggi per chi cerca:
- **longevità**: deve restare piacevole da usare per 5 o più anni;
- **autonomia** alta;
- **nessuna scheda video dedicata**: conta molto la grafica integrata (iGPU);
- **potenza** sufficiente per applicazioni multimediali e di design (foto, grafica, video leggero, impaginazione, presentazioni), con un'esperienza fluida;
- portatili tra **800 e 1.200 €**.

> **Non è una classifica.** I 10 processori sono raggruppati per produttore e l'ordine non indica una preferenza. Ognuno ha un profilo diverso; la sezione finale spiega quali sono compatibili con i vincoli del progetto (RAM espandibile, Carta del Docente). I vincoli ufficiali restano quelli di [CLAUDE.md](../CLAUDE.md): questa analisi **non li modifica**.

---

## Cosa conta davvero per multimedia e design senza GPU dedicata

| Fattore | Perché conta | Cosa guardare |
|---|---|---|
| **iGPU** | Senza scheda video dedicata, la grafica integrata gestisce anteprime, filtri, accelerazione video, monitor esterni | Numero di unità grafiche (CU AMD, core Xe Intel), banda di memoria |
| **Core CPU "veri"** | Export, rendering, tanti programmi aperti insieme | Almeno 8 core moderni; i core a basso consumo (Zen 5c, LP-E) aiutano l'autonomia ma pesano poco nei carichi pesanti |
| **Memoria** | Design e foto usano molta RAM; la iGPU usa la RAM di sistema come memoria video | 32 GB sono lo standard "longevo"; RAM veloce (LPDDR5X) = iGPU più rapida, ma di solito **saldata** |
| **NPU** | Funzioni IA locali (Copilot+, rimozione sfondi, effetti video, strumenti IA di Adobe e DaVinci) sempre più diffuse | ≥ 40–50 TOPS per i requisiti Copilot+ e i prossimi software |
| **Efficienza** | Autonomia e silenziosità | Test misurati (Notebookcheck Wi-Fi, MobileMark), non dichiarazioni |
| **Ecosistema** | Compatibilità dei programmi nel tempo | x86 (Intel/AMD) = compatibilità totale; ARM Windows (Snapdragon) = quasi totale; macOS = altro ecosistema |

**Compromesso chiave per la longevità:** le piattaforme con la iGPU più veloce e l'autonomia migliore (Intel Lunar Lake e serie X, Snapdragon, Apple) usano **RAM saldata** ad alta velocità. Le piattaforme con **RAM SO-DIMM espandibile** (AMD Ryzen AI 300/400 nelle linee business, alcuni Intel Core Ultra serie 3 non-X) hanno una iGPU un po' meno veloce, ma permettono di arrivare a 32–64 GB più avanti. Con RAM saldata, per durare nel tempo bisogna **comprare subito 32 GB**.

---

## I 10 processori

### AMD

#### Ryzen AI 7 350 / AI 7 PRO 350 — "Krackan Point" (Zen 5, 2025)

| Voce | Dato |
|---|---|
| CPU | 8 core / 16 thread (4 Zen 5 + 4 Zen 5c), fino a 5,0 GHz, 28 W (15–54 W) |
| iGPU | Radeon 860M, 8 CU RDNA 3.5 |
| NPU | XDNA 2, 50 TOPS (Copilot+) |
| Memoria | DDR5-5600 **SO-DIMM** o LPDDR5X-8000 (dipende dal portatile) |
| Autonomia misurata | **13,8 h** (ThinkPad T14 Gen 6) · **14,0 h** (ASUS ExpertBook PM3), test Wi-Fi Notebookcheck |
| Fascia di prezzo | Portatili da ~800 a ~1.300 € |

- **Multimedia e design:** CPU molto valida per export ed editing foto; la 860M basta per Photoshop, Illustrator, Affinity, Canva, video 1080p, ma è al limite con video 4K pesanti.
- **Longevità:** buona. Architettura recente, NPU Copilot+, molti modelli con RAM espandibile fino a 64 GB.
- **Note:** è il riferimento attuale del progetto, con il miglior equilibrio tra prezzo, autonomia ed espandibilità.

#### Ryzen AI 7 450 / AI 7 PRO 450 — "Gorgon Point" (Zen 5, 2026)

| Voce | Dato |
|---|---|
| CPU | 8 core / 16 thread, come il 350 ma +100 MHz |
| iGPU | Radeon 860M, frequenza leggermente più alta |
| NPU | XDNA 2, ~50–55 TOPS |
| Memoria | DDR5-5600 SO-DIMM o LPDDR5X fino a 8533 |
| Prestazioni | **+5–6 %** sul 350 (Blender, benchmark aggregati) |
| Fascia di prezzo | Oggi ~1.340 € e oltre (EliteBook 6/8 G2a, ThinkPad T14 Gen 7) |

- **Multimedia e design:** come il 350.
- **Longevità:** come il 350, ma con un anno di supporto "in più" sulla carta.
- **Note:** è un aggiornamento minimo. **Conviene solo se costa come un 350.** I prezzi dovrebbero scendere nel 2027.

#### Ryzen AI 9 HX 370 (e AI 9 365) — "Strix Point" (Zen 5, 2024–2025)

| Voce | Dato |
|---|---|
| CPU | HX 370: 12 core / 24 thread (4 Zen 5 + 8 Zen 5c), fino a 5,1 GHz · 365: 10 core / 20 thread |
| iGPU | HX 370: **Radeon 890M, 16 CU** · 365: Radeon 880M, 12 CU |
| NPU | XDNA 2, 50 TOPS |
| Memoria | Quasi sempre LPDDR5X **saldata**; raramente SO-DIMM |
| Autonomia | Di solito **1–3 h in meno** del 350 a parità di batteria (stima da recensioni; dipende molto dal portatile) |
| Fascia di prezzo | ~1.000–1.400 € (Vivobook S, Zenbook, alcuni ProArt) |

- **Multimedia e design:** la **migliore iGPU AMD nella fascia di prezzo**. La 890M è circa il doppio della 860M nei carichi grafici: utile per editing video, Lightroom e DaVinci Resolve.
- **Longevità:** ottima potenza di riserva, ma con RAM saldata serve comprare subito 32 GB.
- **Note:** scalda e consuma più del 350. Ha senso se il design e il video sono il lavoro principale.

#### Ryzen AI 9 HX 470 (e AI 9 465) — "Gorgon Point" (Zen 5, 2026)

| Voce | Dato |
|---|---|
| CPU | 12 core / 24 thread, frequenze leggermente più alte dell'HX 370 |
| iGPU | Radeon 890M, 16 CU |
| NPU | XDNA 2, ~55 TOPS |
| Memoria | LPDDR5X o DDR5 (dipende dal portatile) |
| Fascia di prezzo | Oggi ~1.700 € e oltre (es. ExpertBook P5 G2 a 1.699 € da Giannone); in calo nel 2027 |

- **Multimedia e design:** come l'HX 370, con qualche punto percentuale in più.
- **Longevità:** la piattaforma AMD senza GPU dedicata più potente nella fascia "normale" (esclusi i Ryzen AI Max).
- **Note:** oggi è fuori budget. Da tenere d'occhio in caso di offerte o modelli usciti da poco.

### Intel

#### Core Ultra X7 358H (serie X, "Panther Lake", Intel 18A, 2026)

| Voce | Dato |
|---|---|
| CPU | 16 core (4 P + 8 E + 4 LP-E), fino a ~4,8 GHz |
| iGPU | **Arc B390, 12 core Xe3**, la iGPU più potente in commercio sui portatili x86 "normali" |
| NPU | ~50 TOPS |
| Memoria | LPDDR5X ad alta velocità, **saldata** |
| Autonomia | Molto alta in ufficio e video: oltre 17 h MobileMark sull'X9 388H; ~12 h d'uso reale secondo PCWorld |
| Fascia di prezzo | Oggi soprattutto **sopra i 1.200 €** (XPS 14, Zenbook, ExpertBook Ultra) |

- **Multimedia e design:** **il migliore senza GPU dedicata in ambito Windows**. Intel dichiara prestazioni grafiche vicine a una RTX 4050 portatile (dato del produttore, non verificato in modo indipendente).
- **Longevità:** eccellente come potenza, ma la RAM è saldata: servono 32 GB dall'inizio.
- **Note:** è il riferimento per chi fa design o video. In fascia 1.200 € lo si trova solo con offerte.

#### Core Ultra X5 338H (serie X "entry", Panther Lake, 2026)

| Voce | Dato |
|---|---|
| CPU | 12 core (4 P + 4 E + 4 LP-E) |
| iGPU | Arc B370, **10 core Xe3** |
| NPU | ~50 TOPS |
| Memoria | LPDDR5X, **saldata** |
| Fascia di prezzo | La versione serie X più accessibile; modelli verso i ~1.000–1.300 € |

- **Multimedia e design:** iGPU di poco inferiore alla B390, molto superiore a Radeon 860M e Arc 140V.
- **Longevità:** buona, ma con RAM saldata.
- **Note:** sulla carta è il **miglior compromesso grafico/prezzo** del 2026. La disponibilità in Italia va verificata.

#### Core Ultra 7 355 (e Core Ultra 5 325) — Panther Lake "non X" (2026)

| Voce | Dato |
|---|---|
| CPU | 8 core (4 P + 4 LP-E); il 325 è quasi identico (benchmark Notebookcheck molto vicini) |
| iGPU | Arc con **solo 4 core Xe3**: sufficiente, ma nettamente sotto le versioni X |
| NPU | ~50 TOPS |
| Memoria | LPDDR5X o **DDR5 SO-DIMM**: ad esempio il ThinkPad E14 Gen 8 Intel ha DDR5 SODIMM con Core Ultra 5 332 e 7 355 |
| Autonomia | **Eccellente**: Notebookcheck parla di "batteria lunga/molto lunga" su XPS 14 e Dell 14S; altre testate oltre 20 h di navigazione |
| Fascia di prezzo | ~900–1.300 € (Dell 14S, XPS 14 base, ThinkPad E14 Gen 8 Intel, IdeaPad Slim 5i) |

- **Multimedia e design:** CPU paragonabile al Ryzen AI 7 350, iGPU simile o leggermente inferiore alla 860M.
- **Longevità:** buona, ed esistono **modelli con RAM espandibile**.
- **Note:** è **l'alternativa Intel più vicina** al profilo cercato in questo progetto: autonomia superiore al Ryzen AI 7 350, RAM SO-DIMM disponibile in alcuni ThinkPad.

#### Core Ultra 7 258V / 256V — "Lunar Lake" (2024)

| Voce | Dato |
|---|---|
| CPU | 8 core (4 P + 4 LP-E), senza Hyper-Threading |
| iGPU | Arc 140V, 8 core Xe2: ottima per la sua generazione, superiore alla Radeon 860M |
| NPU | 47–48 TOPS |
| Memoria | **16 o 32 GB integrati nel processore** (on-package): **mai espandibile** |
| Autonomia misurata | **19,4 h** (ThinkPad T14 Gen 6 Intel) · 21 h (T14s Gen 6), test Wi-Fi Notebookcheck |
| Fascia di prezzo | Oggi scontato: ~800–1.200 € |

- **Multimedia e design:** iGPU buona; CPU più debole delle altre nei carichi pesanti multi-core (export lunghi).
- **Longevità:** **limitata dalla RAM fissa**. Ha senso solo nella versione da 32 GB.
- **Note:** è il **re dell'autonomia** su Windows ed è a buon prezzo perché è di generazione precedente.

### Qualcomm

#### Snapdragon X2 Elite (ARM, Windows, 2026)

| Voce | Dato |
|---|---|
| CPU | 12–18 core Oryon di terza generazione: prestazioni da primato in single e multi-core in diversi test (HotHardware) |
| iGPU | Adreno X2 |
| NPU | **80 TOPS**, la più alta della fascia |
| Memoria | LPDDR5X, **saldata** |
| Autonomia | Variabile: **10,5 h** (Tom's Hardware, Zenbook A16, X2 Elite Extreme) – ~20 h (HotHardware). Mantiene le prestazioni a batteria |
| Fascia di prezzo | ~1.100–1.500 € (Zenbook A16, HP OmniBook) |

- **Multimedia e design:** Photoshop, Lightroom e After Effects ora sono nativi ARM; **Premiere Pro e alcuni plug-in o driver** (stampanti, tavolette grafiche particolari, software CAD) restano punti deboli.
- **Longevità:** ottima come potenza ed efficienza, ma con RAM saldata e un rischio di compatibilità da valutare programma per programma.
- **Note:** la scelta giusta solo se i programmi usati sono tutti nativi ARM. Il precedente Snapdragon X Plus/X1 (prima generazione) è molto più debole.

### Apple

#### Apple M5 (MacBook Air 13"/15", 2026)

| Voce | Dato |
|---|---|
| CPU | 10 core (4 prestazioni + 6 efficienza) |
| GPU | GPU integrata Apple (8–10 core secondo la configurazione) con accelerazione IA nei core grafici |
| NPU | Neural Engine 16 core; Apple dichiara IA fino a 4 volte più veloce dell'M4 |
| Memoria | Memoria unificata **saldata**, 16 GB di base (24/32 GB opzionali) · SSD 512 GB di base |
| Autonomia | Apple dichiara fino a 18 h; nella pratica è tra le migliori della categoria |
| Prezzo Italia | Listino **1.249 €** (13"), istruzione **1.139 €**; visto su Amazon a **1.099 €** nel 2026 |

- **Multimedia e design:** probabilmente **l'esperienza più fluida della fascia** per foto, grafica e video (Final Cut, Affinity, Adobe nativi, Pixelmator). Nessuna ventola, silenzioso.
- **Longevità:** molto buona per supporto software (macOS di solito per 6–8 anni), ma **RAM e SSD non sono espandibili**: va comprato subito con la memoria che serve.
- **Note:** cambia ecosistema (macOS). Con 16 GB è accettabile oggi; per durare 5 anni o più nel design sarebbero meglio 24 GB, che però escono dal budget. Se Apple accetti la Carta del Docente con pagamento misto è **da verificare**.

---

## Riepilogo comparativo (non è una classifica)

| Processore | CPU | iGPU per design/video | Autonomia | RAM espandibile? | Prezzo tipico portatile | Ecosistema |
|---|---|---|---|---|---|---|
| Ryzen AI 7 350 | ●●●● | ●●● | ●●●● | **Spesso sì** (business) | 800–1.300 € | Windows x86 |
| Ryzen AI 7 450 | ●●●● | ●●● | ●●●● | **Spesso sì** (business) | 1.300 € e oltre (in calo) | Windows x86 |
| Ryzen AI 9 HX 370 / 365 | ●●●●● | ●●●● | ●●● | Raramente | 1.000–1.400 € | Windows x86 |
| Ryzen AI 9 HX 470 / 465 | ●●●●● | ●●●● | ●●● | Raramente | 1.700 € e oltre (oggi) | Windows x86 |
| Core Ultra X7 358H | ●●●●● | ●●●●● | ●●●●● | No | 1.300 € e oltre (oggi) | Windows x86 |
| Core Ultra X5 338H | ●●●● | ●●●●● | ●●●●● | No | 1.000–1.300 € | Windows x86 |
| Core Ultra 7 355 / 5 325 | ●●●● | ●●● | ●●●●● | **A volte sì** (ThinkPad E14 Gen 8 Intel) | 900–1.300 € | Windows x86 |
| Core Ultra 7 258V (Lunar Lake) | ●●● | ●●●● | ●●●●● | **Mai** | 800–1.200 € | Windows x86 |
| Snapdragon X2 Elite | ●●●●● | ●●●● | ●●●●(●) | No | 1.100–1.500 € | Windows ARM |
| Apple M5 | ●●●●● | ●●●●● | ●●●●● | No | 1.099–1.249 € | macOS |

Pallini indicativi (●●●●● = eccellente nella fascia di prezzo), basati sulle recensioni citate nelle fonti; non sono misure.

## Esclusi dall'elenco e perché

| Processore | Motivo |
|---|---|
| Ryzen AI 5 340 / 330, Ryzen AI 7 345 / 445, Ryzen AI 5 430 / 435 / 440 | Solo 4–6 core: meno longevi per design ed export |
| Ryzen 200 (220/230/250/260), Ryzen 7 8840HS/U | Zen 4 di generazione precedente, NPU debole (non Copilot+) |
| Intel Core 5/7 serie 300 "Wildcat Lake" (es. Core 7 350) | Fascia economica, iGPU minima |
| Intel Core Ultra 200H/U "Arrow Lake" | Superati da Panther Lake in efficienza e grafica |
| Snapdragon X Plus / X1 (prima generazione) | CPU e GPU deboli rispetto alla seconda generazione |
| Ryzen AI Max 385/390/395 ("Strix Halo"), Apple M5 Pro | Ottimi, ma i portatili costano molto oltre i 1.200 € |
| CPU HX con GPU dedicata (Ryzen 9 HX, Core Ultra HX) | Pensate per portatili gaming con scheda video, esclusi dal progetto |

---

## Cosa significa per la nostra ricerca

Il vincolo attuale del progetto (in [CLAUDE.md](../CLAUDE.md)) è: **minimo Ryzen AI 7 350, RAM SO-DIMM espandibile, solo grafica integrata, ≤ 1.200 €, Carta del Docente**. Incrociandolo con questa analisi:

1. **Pienamente compatibili:** **Ryzen AI 7 350 / PRO 350** e **Ryzen AI 7 450 / PRO 450**. Sono gli unici con RAM SO-DIMM diffusa nelle linee business (ExpertBook P3, ThinkPad E/L/T, EliteBook/ProBook G1a/G2a, IdeaPad Slim 5 AKP10).
2. **Compatibili sulla carta ma rari con SO-DIMM:** Ryzen AI 9 HX 370 / 470. Quasi sempre hanno RAM saldata, quindi di fatto restano fuori dal vincolo "RAM espandibile".
3. **Possibile allargamento (da decidere con l'utente):** gli **Intel Core Ultra 7 355 / Core Ultra 5 325 (Panther Lake)** hanno CPU paragonabile al Ryzen AI 7 350, **autonomia migliore**, NPU da 50 TOPS ed esistono **con DDR5 SO-DIMM** (ThinkPad E14 Gen 8 Intel). Oggi il vincolo "AMD Ryzen AI 7 350 minimo" li esclude solo per il marchio. Ammetterli **aumenterebbe le offerte disponibili** senza perdere longevità. Va però verificato modello per modello che la RAM sia SO-DIMM.
4. **Incompatibili con "RAM espandibile":** Intel Lunar Lake e serie X, Snapdragon X2 e Apple M5. Sono ottimi per design e autonomia, ma la RAM è saldata. Si considerano solo se l'utente decide di rinunciare all'espandibilità in cambio di grafica e autonomia migliori, e in quel caso con **32 GB già dall'inizio** (24 GB per Apple, che però escono dal budget).

**Domanda aperta per l'utente** (annotata in [statoRicerca.md](statoRicerca.md)): ammettere gli Intel Core Ultra serie 3 "non X" con RAM SO-DIMM come alternativa equivalente al Ryzen AI 7 350?

---

## Fonti (consultate il 2026-11-11)

- Notebookcheck: [ThinkPad T14 Gen 6 AMD (Ryzen AI 7 PRO 350, con tabella di confronto delle autonomie)](https://www.notebookcheck.net/AMD-Ryzen-AI-meets-classic-ThinkPad-Lenovo-ThinkPad-T14-Gen-6-AMD-laptop-review.1222690.0.html) · [ASUS ExpertBook PM3](https://www.notebookcheck.net/Asus-ExpertBook-PM3-Review-Office-laptop-with-AMD-long-battery-life-and-Copilot.1200511.0.html) · [Ryzen AI 7 350 vs AI 7 450](https://www.notebookcheck.net/Ryzen-AI-7-350-vs-Ryzen-AI-7-450_19172_20425.247596.0.html) · [Ryzen AI 7 PRO 450](https://www.notebookcheck.net/AMD-Ryzen-AI-7-PRO-450-Processor-Benchmarks-and-Specs.1198883.0.html) · [Dell XPS 14 Core Ultra 7 355](https://www.notebookcheck.net/Dell-XPS-14-Core-Ultra-7-355-review-Still-great-but-not-nearly-as-special.1222645.0.html) · [Dell 14S DS14260](https://www.notebookcheck.net/Dell-14S-DS14260-review-As-powerful-as-an-XPS-14.1366869.0.html) · [Dell XPS 14 2026 Panther Lake X7](https://www.notebookcheck.net/Dell-XPS-14-2026-review-Fully-reborn-with-Intel-Panther-Lake-X7.1218670.0.html) · [Core Ultra 5 325 vs 7 355 (PL)](https://www.notebookcheck.pl/Nasze-pierwsze-testy-porownawcze-Core-Ultra-5-325-sa-juz-dostepne-a-wyniki-sa-niemal-identyczne-jak-w-przypadku-Core-Ultra-7-355.1255882.0.html) · [ThinkPad T14 Gen 7 vs Gen 6 (Lunar Lake)](https://www.notebookcheck.net/Lunar-Lake-is-still-the-Intel-battery-life-king-ThinkPad-T14-Gen-7-vs-T14-Gen-6.1313676.0.html)
- Nanoreview: [Ryzen AI 7 450 vs AI 7 350](https://nanoreview.net/en/cpu-compare/amd-ryzen-ai-7-450-vs-amd-ryzen-ai-7-350)
- Panther Lake: [PCWorld, Core Ultra X9 388H](https://www.pcworld.com/article/3034214/intel-core-ultra-x9-388h-review-epic-graphics-battery-life.html) · [PCWorld, ExpertBook Ultra](https://www.pcworld.com/article/3044102/asus-expertbook-ultra-review.html) · [Club386](https://www.club386.com/intel-core-ultra-series-3-panther-lake-review/) · [HardwareZone](https://www.hardwarezone.com.sg/pc/laptops/intel-core-ultra-x9-388h-mobile-processor-laptop-review) · [Wccftech, Zenbook Duo](https://wccftech.com/review/asus-zenbook-duo-intel-core-ultra-x9-388h-panther-lake-laptop-review/) · [Tom's Hardware, serie X e Xe3](https://www.tomshardware.com/pc-components/cpus/intel-doubles-down-on-gaming-with-panther-lake-claims-76-percent-faster-gaming-performance-new-x-series-chips-deliver-up-to-12-xe3-cores) · [VideoCardz, elenco SKU](https://videocardz.com/newz/intel-core-ultra-300-panther-lake-sku-lineup-leaked-up-to-16-cpu-cores-5-1-ghz-boost-and-arc-b390-xe3-graphics) · [PC Gamer, autonomia XPS 14](https://pcgamer.com/hardware/gaming-laptops/dell-xps-14-laptop-with-a-panther-lake-chip-manages-a-staggering-43-hour-battery-life-result-thrashing-the-latest-macbook-air)
- Snapdragon X2: [Tom's Hardware, Zenbook A16](https://www.tomshardware.com/laptops/ultrabooks-ultraportables/asus-zenbook-a16-snapdragon-x2-elite-review) · [HotHardware](https://hothardware.com/reviews/qualcomm-snapdragon-x2-elite-benchmarks-and-performance?page=2) · [Windows Central](https://www.windowscentral.com/hardware/qualcomm/snapdragon-x2-elite-month-believer)
- Apple M5: [SmartWorld, MacBook Air M5 e prezzi Italia](https://www.smartworld.it/news/macbook-air-m5-apple-caratteristiche-prezzo.html) · [Fastweb Plus](https://www.fastweb.it/fastweb-plus/digital-dev-security/nuovo-macbook-air-con-chip-m5-caratteristiche-e-prezzo/) · [Macitynet, prezzi MacBook 2026](https://www.macitynet.it/prezzi-macbook-pro-macbook-air-2026/)
- Prezzi italiani dei portatili: dalle ricerche 1–5 in [elencoOfferte.md](elencoOfferte.md) (Lenovo.com, IT-Partners, MediaWorld, Giannone, Amazon.it).

> Limiti: alcuni dati (iGPU della serie X5, prezzi italiani di Panther Lake serie X e Snapdragon X2, autonomia dell'HX 370 in modelli specifici) vengono da recensioni estere o da fonti non ancora confermate. Vanno ricontrollati quando si valuta un portatile preciso.
