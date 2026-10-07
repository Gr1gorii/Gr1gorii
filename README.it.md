[English](README.md) | [Italiano](README.it.md)

# Hryhorii Klymenko

**Data Analyst / Junior Data Scientist · Analisi dei dati per retail, e-commerce e hospitality**

MSc in Informatica. Costruisco analisi che portano a una decisione di business: quanto riordinare, chi contattare, quanto vale un cliente e se uno sconto è reale. Python e SQL, con validazione temporale e intervalli di confidenza invece di un singolo numero.

Disponibile per ruoli junior nei dati in Italia e da remoto (UE). Autorizzato a lavorare in Italia, senza necessità di visto né di supporto per il trasferimento.

[LinkedIn](https://www.linkedin.com/in/hryhorii-klymenko/) · [Devpost](https://devpost.com/GKL1) · [X](https://x.com/HKL1ne)

## In corso

### [Gli sconti del Black Friday sono reali? Italia 2026](https://github.com/Gr1gorii/price-tracker)

Con la direttiva Omnibus (art. 17-bis del Codice del Consumo), uno sconto annunciato deve essere calcolato sul prezzo più basso dei 30 giorni precedenti. Monitoro **circa 1.800 prodotti in 5 negozi online italiani due volte al giorno** per verificare se gli sconti del Black Friday (27 novembre 2026) rispettano questa regola.

- Raccolta pianificata: rispetta robots.txt, limita la frequenza delle richieste, salva in Parquet + DuckDB, due esecuzioni al giorno
- Verifica di conformità: vero minimo a 30 giorni, sconto dichiarato vs sconto reale, segnalazione di prezzi di riferimento gonfiati e di aumenti di prezzo subito prima dello sconto
- **Risultati: inizio dicembre 2026**

Python · httpx · DuckDB · pandas · GitHub Actions · pytest

## Progetti selezionati

### 1. [Retail Demand Planner](https://github.com/Gr1gorii/retail-demand-planner/blob/main/README.it.md)

**Quale previsione garantisce a un supermercato il riordino settimanale più economico?**

- Previsioni giornaliere per **1.437 prodotti alimentari** (Walmart M5) su quattro finestre cronologiche: LightGBM contro naive stagionale e media mobile a 28 giorni
- Previsioni trasformate in una politica di riordino settimanale con lead time di due giorni e scorta di sicurezza calibrata solo sui dati di validazione
- **Risultato:** LightGBM ha il costo di magazzino simulato più basso, **il 20,8% in meno del naive stagionale**, ed è il più economico in tutte e quattro le finestre e in tutti i nove scenari di costo

Python · LightGBM · pandas · Streamlit (EN/IT)

<a href="https://github.com/Gr1gorii/retail-demand-planner/blob/main/README.it.md">
  <img src="https://raw.githubusercontent.com/Gr1gorii/retail-demand-planner/main/assets/it/overview.png" alt="Costo di magazzino simulato per metodo di previsione e risparmio per finestra" width="760">
</a>

### 2. [Email Campaign Uplift](https://github.com/Gr1gorii/discount-uplift/blob/main/README.it.md)

**Conviene inviare l'email solo ai clienti che la campagna convince davvero?**

- Esperimento randomizzato Hillstrom, **42.613 clienti**: l'email aumenta la conversione di **0,68 punti percentuali** (IC 95% 0,50–0,86)
- Modello di uplift, profitto incrementale per politica di targeting, intervalli bootstrap e sensibilità al costo di contatto e al valore del coupon
- **Risultato:** inviare solo al top 30% non è significativamente più redditizio che inviare a tutti (−66 $ ogni 10.000 clienti, IC 95% da −989 $ a 804 $), quindi raccomando un nuovo pilota randomizzato prima del rilascio

Python · scikit-learn · bootstrap · Streamlit (EN/IT)

<details>
<summary>Anteprima: profitto per politica di targeting</summary>

![Profitto incrementale e intervalli bootstrap per politica di targeting](https://raw.githubusercontent.com/Gr1gorii/discount-uplift/main/reports/policy_profit_it.png)

</details>

### 3. [Customer Lifetime Value & Segmentation](https://github.com/Gr1gorii/ecommerce-clv-segmentation/blob/main/README.it.md)

**Quanto vale ogni cliente nel prossimo anno e cosa fare con ciascun segmento?**

- Modello BG/NBD + Gamma-Gamma sulle transazioni UK di Online Retail II, testato su tre finestre temporali contro due baseline
- Il modello supera entrambe le baseline nella quota di ricavi catturata dal top 10% e dal top 20% dei clienti in tutte e tre le finestre; lo uso per ordinare i clienti, non per prevedere il ricavo esatto
- **Risultato:** intervalli di riferimento per il CAC e un'azione per ogni segmento, incluso un test di riattivazione con costi stimati per 104 clienti dormienti ad alto valore

Python · lifetimes · pandas · Streamlit (EN/IT)

<details>
<summary>Anteprima: dashboard del portafoglio clienti</summary>

![Dashboard Streamlit con contributo per segmento e distribuzione del valore dei clienti](https://raw.githubusercontent.com/Gr1gorii/ecommerce-clv-segmentation/main/reports/figures/it/dashboard.jpg)

</details>

### 4. [Hotel Booking Analytics](https://github.com/Gr1gorii/hotel-booking-analytics)

**Da dove arrivano le cancellazioni e si possono prevedere quelle tardive?**

- **119.390 prenotazioni** analizzate con viste SQL, una dashboard interattiva e un report per la direzione
- **Risultato:** il 41,7% delle prenotazioni è stato cancellato nel city hotel contro il 27,8% nel resort; il tasso di cancellazione è del 57,0% per le prenotazioni fatte con oltre 180 giorni di anticipo, contro il 9,6% a 0–7 giorni
- Modello per le cancellazioni tardive con validazione temporale e verifica delle variabili contro il data leakage; resta offline perché il piccolo miglioramento comporta molti falsi allarmi

Python · SQL (SQLite) · scikit-learn · Streamlit

<details>
<summary>Anteprima: dashboard delle prenotazioni</summary>

![Dashboard hotel con prenotazioni, tassi di cancellazione e andamento mensile](https://raw.githubusercontent.com/Gr1gorii/hotel-booking-analytics/main/docs/images/overview.jpg)

</details>

### 5. [Document Search RAG](https://github.com/Gr1gorii/document-search-rag/blob/main/README.it.md)

**Un piccolo modello locale può rispondere a domande sulla documentazione con fonti verificabili?**

- RAG locale (BM25 + Ollama) su 12 pagine della documentazione FastAPI, con citazioni e astensione quando mancano prove
- Pagina attesa tra i primi quattro risultati per 45/45 domande con risposta; astensione su 15/15 domande fuori ambito; casi di errore documentati

Python · FastAPI · BM25 · Ollama

## Competenze

**Analisi:** Python, pandas, SQL (DuckDB, SQLite), dashboard Streamlit  
**Statistica e ML:** test A/B e uplift, intervalli bootstrap, previsione della domanda (LightGBM), modelli CLV, scikit-learn, validazione temporale  
**Data engineering:** raccolta di dati dal web, Parquet, pipeline pianificate (GitHub Actions), pytest  
**AI:** RAG locale e valutazione delle risposte del modello

## Altri progetti

[Customer Repeat Purchase Analysis](https://github.com/Gr1gorii/customer-repeat-purchase-analysis/blob/main/README.it.md) · [Processing Efficiency Study](https://github.com/Gr1gorii/processing-efficiency-study/blob/main/README.it.md) · [TON Tracker](https://github.com/Gr1gorii/ton-tracker) · [HeatRelay](https://github.com/Gr1gorii/HeatRelay) · [Tutti i repository](https://github.com/Gr1gorii?tab=repositories)

Progetti di portfolio su dati pubblici. Ogni repository documenta fonti, controlli e limiti.
