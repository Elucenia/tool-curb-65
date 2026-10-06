<!-- ELUCENIA technical documentation · curb-65 · it · no clinical/professional/rights approval -->

# CURB-65

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/curb-65)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Confusione mentale (nuovo disorientamento nel tempo, nello spazio o rispetto alla persona)

`c`

### Urea \> 42 mg/dL (\> 7 mmol/L)

`u`

### FR ≥ 30 atti/min

`r`

### Pressione sistolica \< 90 mmHg o diastolica ≤ 60 mmHg (B: pressione arteriosa)

`b`

### Età ≥ 65 anni

`i`

## Edizione del metodo

CURB-65/Lim 2003: confusione, urea\>7 mmol/L, FR≥30, pressione, età≥65; 0–5

## Formula documentata

Un punto per item: C (confusione), Urea \> 7 mmol/L, R (frequenza respiratoria) ≥ 30/min, B (pressione bassa: PAS \< 90 o PAD ≤ 60 mmHg) ed età ≥ 65. Massimo: 5.

Il CRB-65 è lo stesso punteggio senza urea (0–4), per uso senza laboratorio.

## Limiti e popolazione

Il CURB-65 del 2003 è stato derivato e validato in adulti ricoverati con polmonite acquisita in comunità, usando i dati della valutazione iniziale e la mortalità a 30 giorni. L’età ≥ 65 è una componente del punteggio, non l’età minima di ammissibilità. Le soglie originali usano urea \> 7 mmol/L, frequenza respiratoria ≥ 30/min e pressione arteriosa sistolica \< 90 o diastolica ≤ 60 mmHg. Esclusioni e uso in altre popolazioni richiedono la lettura del protocollo completo.

## Riferimenti

- [Lim WS et al. Defining community acquired pneumonia severity on presentation to hospital: an international derivation and validation study. Thorax, 2003.](https://doi.org/10.1136/thorax.58.5.377)

- [Lim WS et al. BTS guidelines for the management of community acquired pneumonia in adults: update 2009. Thorax, 2009.](https://doi.org/10.1136/thx.2009.121434)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Basso rischio: mortalità a 30 giorni dell’1,5%

| Dettagli del risultato | |
| --- | --- |
| CRB-65 (senza l’urea) | 0 (basso rischio (mortalità < 1%)) |
| Condotta suggerita | Candidato al trattamento ambulatoriale, se non vi sono altri motivi per il ricovero. |


### 2

Rischio intermedio: mortalità a 30 giorni del 9,2%

| Dettagli del risultato | |
| --- | --- |
| CRB-65 (senza l’urea) | 2 (rischio aumentato (1 a 10%): considerare il ricovero in ospedale) |
| Condotta suggerita | Considerare il ricovero (o una breve osservazione sorvegliata). |


### 3

Alto rischio: mortalità a 30 giorni del 22%

| Dettagli del risultato | |
| --- | --- |
| CRB-65 (senza l’urea) | 3 (alto rischio (> 10%): ricovero urgente) |
| Condotta suggerita | Ricoverare; con 4 o 5 punti, valutare la necessità di terapia intensiva. |


### 4

Basso rischio: mortalità a 30 giorni dell’1,5%

| Dettagli del risultato | |
| --- | --- |
| CRB-65 (senza l’urea) | 0 (basso rischio (mortalità < 1%)) |
| Condotta suggerita | Candidato al trattamento ambulatoriale, se non vi sono altri motivi per il ricovero. |

