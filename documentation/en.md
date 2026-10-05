<!-- ELUCENIA technical documentation · padua · en · no clinical/professional/rights approval -->

# Padua score

[conditions, sources and permissions](https://elucenia.org/en/tools/padua)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Active cancer (metastasis or chemotherapy/radiotherapy in the last 6 months)

`cancer`

### Previous VTE (excluding superficial venous thrombosis)

`tev`

### Reduced mobility (bed rest with bathroom privileges for ≥ 3 days)

`mobilidade`

### Known thrombophilia

`trombofilia`

### Trauma or surgery in the last month

`trauma`

### Age ≥ 70 years

`idade`

### Heart and/or respiratory failure

`icc`

### Acute myocardial infarction or ischemic stroke

`iam`

### Acute infection and/or rheumatological disease

`infeccao`

### Obesity (BMI ≥ 30 kg/m²)

`obesidade`

### Ongoing hormone treatment

`hormonio`

## Method edition

Padua Prediction Score/Barbar 2010: 11 factors, 0–20; hospitalized medical patient

## Documented formula

3 points: active cancer, previous VTE, reduced mobility, thrombophilia · 2 points: recent trauma or surgery · 1 point: age ≥ 70, heart/respiratory failure, MI or ischemic stroke, acute infection or rheumatological disease, obesity, hormone therapy. Maximum: 20.

## Limits and population

Padua was studied in medical inpatients in internal medicine, with follow-up for symptomatic thromboembolism up to 90 days. Thrombotic stratification must be accompanied by assessment of bleeding, contraindications and the prophylaxis protocol. The total does not replace that analysis or imply automatic application to surgical patients.

## References

- [Barbar S et al. A risk assessment model for the identification of hospitalized medical patients at risk for venous thromboembolism: the Padua Prediction Score. J Thromb Haemost, 2010.](https://doi.org/10.1111/j.1538-7836.2010.04044.x)

- [Kahn SR et al. Prevention of VTE in nonsurgical patients: antithrombotic therapy and prevention of thrombosis, 9th ed: American College of Chest Physicians evidence-based clinical practice guidelines. Chest, 2012.](https://doi.org/10.1378/chest.11-2296)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
