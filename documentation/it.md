<!-- ELUCENIA technical documentation · funcao-discriminante-de-maddrey · it · no clinical/professional/rights approval -->

# Funzione discriminante di Maddrey

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/funcao-discriminante-de-maddrey)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Tempo di protrombina del paziente

`tp`

s · intervallo: 5–150

### Tempo di protrombina di controllo

`tpc`

s · intervallo: 5–30

### Bilirubina totale

`bili`

mg/dL · intervallo: 0,1–80

## Edizione del metodo

Maddrey modificata/Carithers 1989: 4,6×(TP paziente−TP controllo)+bilirubina; senza equazione originale TP assoluto 1978

## Formula documentata

DF = 4,6 × (TP del paziente − TP controllo, in secondi) + bilirubina totale (mg/dL).

## Limiti e popolazione

La funzione originale del 1978 è stata studiata nell’epatite alcolica. La forma locale modificata, con differenza del tempo di protrombina e soglia 32, deve corrispondere all’edizione successiva del 1989. Il totale non sostituisce la valutazione delle controindicazioni, delle infezioni e delle diagnosi alternative prima di qualsiasi decisione terapeutica.

## Riferimenti

- [Maddrey WC et al. Corticosteroid therapy of alcoholic hepatitis. Gastroenterology, 1978.](https://doi.org/10.1016/0016-5085(78)90401-8)

- [Carithers RL et al. Methylprednisolone therapy in patients with severe alcoholic hepatitis: a randomized multicenter trial. Ann Intern Med, 1989.](https://doi.org/10.7326/0003-4819-110-9-685)

- [Crabb DW et al. Diagnosis and treatment of alcohol-associated liver diseases: 2019 practice guidance from the American Association for the Study of Liver Diseases. Hepatology, 2020.](https://doi.org/10.1002/hep.30866)

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
