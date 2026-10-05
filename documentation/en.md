<!-- ELUCENIA technical documentation · funcao-discriminante-de-maddrey · en · no clinical/professional/rights approval -->

# Maddrey discriminant function

[conditions, sources and permissions](https://elucenia.org/en/tools/funcao-discriminante-de-maddrey)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Patient prothrombin time

`tp`

s · range: 5–150

### Control prothrombin time

`tpc`

s · range: 5–30

### Total bilirubin

`bili`

mg/dL · range: 0.1–80

## Method edition

Modified Maddrey/Carithers 1989: 4.6×(patient PT−control PT)+bilirubin; excludes original 1978 absolute-PT equation

## Documented formula

DF = 4.6 × (patient PT − control PT, in seconds) + total bilirubin (mg/dL).

## Limits and population

The original 1978 function was studied in alcoholic hepatitis. The local modified form, with a prothrombin-time difference and cutoff of 32, must correspond to the later 1989 edition. The total does not replace assessment of contraindications, infection and alternative diagnoses before any therapeutic decision.

## References

- [Maddrey WC et al. Corticosteroid therapy of alcoholic hepatitis. Gastroenterology, 1978.](https://doi.org/10.1016/0016-5085(78)90401-8)

- [Carithers RL et al. Methylprednisolone therapy in patients with severe alcoholic hepatitis: a randomized multicenter trial. Ann Intern Med, 1989.](https://doi.org/10.7326/0003-4819-110-9-685)

- [Crabb DW et al. Diagnosis and treatment of alcohol-associated liver diseases: 2019 practice guidance from the American Association for the Study of Liver Diseases. Hepatology, 2020.](https://doi.org/10.1002/hep.30866)

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
