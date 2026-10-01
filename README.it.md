[English](README.md) | [Italiano](README.it.md)

# Hryhorii Klymenko

**Junior Data / AI · Python e SQL**

Mi concentro sull'analisi dei dati e sull'AI applicata: trasformare dati grezzi in risultati chiari, dashboard e prototipi valutati con attenzione. Cerco opportunità junior nell'analisi dei dati e nell'AI applicata.

[LinkedIn](https://www.linkedin.com/in/hryhorii-klymenko/) · [Devpost](https://devpost.com/GKL1) · [X](https://x.com/HKL1ne)

## Progetti selezionati

### 1. [Hotel Booking Analytics](https://github.com/Gr1gorii/hotel-booking-analytics)

**Come variano le prenotazioni e le cancellazioni tra hotel e canali di vendita?**

Python · pandas · SQLite · scikit-learn · Streamlit

- Analisi di **119.390 prenotazioni storiche**, con preparazione riproducibile dei dati, riepiloghi SQL e dashboard interattiva
- Valutazione ML con suddivisione temporale, controlli sulla disponibilità delle variabili, confronto con baseline e analisi degli errori
- **Risultato:** il 41,7% delle prenotazioni è stato cancellato nel city hotel, contro il 27,8% nel resort. Sono differenze osservate, non effetti causali
- Il modello di cancellazione resta un **esperimento offline**: il piccolo miglioramento nel ranking comporta molti falsi allarmi

[Repository e demo locale](https://github.com/Gr1gorii/hotel-booking-analytics) · [Risultati per la gestione](https://github.com/Gr1gorii/hotel-booking-analytics/blob/main/reports/management_brief.md) · [Valutazione del modello](https://github.com/Gr1gorii/hotel-booking-analytics/blob/main/reports/model_results.md)

<a href="https://github.com/Gr1gorii/hotel-booking-analytics">
  <img src="https://raw.githubusercontent.com/Gr1gorii/hotel-booking-analytics/main/docs/images/overview.jpg" alt="Dashboard hotel con prenotazioni, tassi di cancellazione e andamento mensile" width="760">
</a>

### 2. [Customer Repeat Purchase Analysis](https://github.com/Gr1gorii/customer-repeat-purchase-analysis)

**Quali clienti acquistano di nuovo e come cambia l'attività di acquisto per coorte?**

Python · SQL · DuckDB · pandas

- Pipeline per **541.909 righe sorgente di UCI Online Retail**, con regole di qualità documentate e risultati SQL riconciliati con pandas
- Analisi delle coorti e degli acquisti ripetuti a 30/60/90 giorni, con denominatori limitati ai clienti osservabili per l'intera finestra
- **Risultato:** 907 dei 4.070 clienti idonei (**22,3%**) hanno acquistato con un'altra fattura entro 30 giorni. È attività storica di acquisto, non un incremento di business misurato

[Repository e demo locale](https://github.com/Gr1gorii/customer-repeat-purchase-analysis/blob/main/README.it.md) · [Risultati](https://github.com/Gr1gorii/customer-repeat-purchase-analysis/blob/main/reports/management_summary.md) · [SQL degli acquisti ripetuti](https://github.com/Gr1gorii/customer-repeat-purchase-analysis/blob/main/sql/02_repeat.sql)

<details>
<summary>Anteprima del grafico delle coorti</summary>

![Grafico reale dell'attività delle coorti; le celle grigie indicano osservazioni incomplete](https://raw.githubusercontent.com/Gr1gorii/customer-repeat-purchase-analysis/main/reports/cohort-activity.png)

</details>

### 3. [Document Search RAG](https://github.com/Gr1gorii/document-search-rag)

**Un assistente locale può rispondere a domande sulla documentazione e rendere facilmente consultabili le fonti?**

Python · FastAPI · BM25 · Ollama

- Ricerca e RAG locale su **12 pagine della documentazione FastAPI**, con estratti delle fonti, citazioni e possibilità di astenersi dalla risposta
- Modalità di sola ricerca quando il modello locale non è disponibile; nessuna API a pagamento richiesta
- Controlli pubblicati su recupero delle fonti, citazioni, astensione e latenza, compresi i casi di errore. Parole chiave corrispondenti e ID di citazione validi **non dimostrano la correttezza dei fatti**

[Repository e demo locale](https://github.com/Gr1gorii/document-search-rag/blob/main/README.it.md) · [Valutazione e limiti](https://github.com/Gr1gorii/document-search-rag/blob/main/reports/QUALITY.md)

<details>
<summary>Anteprima di una risposta e della fonte</summary>

![Risposta reale del RAG locale con l'estratto della fonte FastAPI aperto](https://raw.githubusercontent.com/Gr1gorii/document-search-rag/main/reports/ui-answer.png)

</details>

## Strumenti usati nei progetti

**Dati:** Python, SQL, pandas, DuckDB, SQLite  
**ML e AI:** scikit-learn, valutazione dei modelli, ricerca BM25, Ollama  
**Applicazioni e verifica:** Streamlit, FastAPI, Git, pytest, workflow locali riproducibili

## Altri progetti

[TON Tracker](https://github.com/Gr1gorii/ton-tracker) · [HeatRelay](https://github.com/Gr1gorii/HeatRelay) · [Tutti i repository](https://github.com/Gr1gorii?tab=repositories)

## Ambito dei progetti

Sono progetti di portfolio e apprendimento. Nei repository sono disponibili riferimenti alle fonti, codice eseguibile, controlli e limiti.
