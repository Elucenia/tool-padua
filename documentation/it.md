<!-- ELUCENIA technical documentation · padua · it · no clinical/professional/rights approval -->

# Punteggio di Padova

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/padua)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Cancro attivo (metastasi o chemio/radioterapia negli ultimi 6 mesi)

`cancer`

### TEV pregresso (esclusa la trombosi venosa superficiale)

`tev`

### Mobilità ridotta (allettamento con accesso al bagno per ≥ 3 giorni)

`mobilidade`

### Trombofilia nota

`trombofilia`

### Trauma o intervento nell’ultimo mese

`trauma`

### Età ≥ 70 anni

`idade`

### Insufficienza cardiaca e/o respiratoria

`icc`

### Infarto miocardico acuto o ictus ischemico

`iam`

### Infezione acuta e/o malattia reumatologica

`infeccao`

### Obesità (IMC ≥ 30 kg/m²)

`obesidade`

### Trattamento ormonale in corso

`hormonio`

## Edizione del metodo

Padua Prediction Score/Barbar 2010: 11 fattori, 0–20; paziente medico ricoverato

## Formula documentata

3 punti: cancro attivo, TEV precedente, mobilità ridotta, trombofilia · 2 punti: trauma o intervento recente · 1 punto: età ≥ 70, insufficienza cardiaca/respiratoria, infarto o ictus ischemico, infezione acuta o malattia reumatologica, obesità, terapia ormonale. Massimo: 20.

## Limiti e popolazione

Il Padua è stato studiato in pazienti medici ricoverati in medicina interna, con follow-up del tromboembolismo sintomatico fino a 90 giorni. La stratificazione trombotica deve essere accompagnata dalla valutazione del sanguinamento, delle controindicazioni e del protocollo di profilassi. Il totale non sostituisce tale analisi e non implica l’applicazione automatica alla popolazione chirurgica.

## Riferimenti

- [Barbar S et al. A risk assessment model for the identification of hospitalized medical patients at risk for venous thromboembolism: the Padua Prediction Score. J Thromb Haemost, 2010.](https://doi.org/10.1111/j.1538-7836.2010.04044.x)

- [Kahn SR et al. Prevention of VTE in nonsurgical patients: antithrombotic therapy and prevention of thrombosis, 9th ed: American College of Chest Physicians evidence-based clinical practice guidelines. Chest, 2012.](https://doi.org/10.1378/chest.11-2296)

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
