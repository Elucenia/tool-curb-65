<!-- ELUCENIA technical documentation · curb-65 · en · no clinical/professional/rights approval -->

# CURB-65

[conditions, sources and permissions](https://elucenia.org/en/tools/curb-65)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Confusion (new disorientation to time, place or person)

`c`

### Urea \> 42 mg/dL (\> 7 mmol/L)

`u`

### Respiratory rate ≥ 30 breaths/min

`r`

### Systolic blood pressure \< 90 mmHg or diastolic ≤ 60 mmHg (Blood pressure)

`b`

### Age ≥ 65 years

`i`

## Method edition

CURB-65/Lim 2003: confusion, urea\>7 mmol/L, RR≥30, blood pressure, age≥65; 0–5

## Documented formula

One point per item: Confusion, Urea \> 7 mmol/L, Respiratory rate ≥ 30/min, Blood pressure low (SBP \< 90 or DBP ≤ 60 mmHg) and age ≥ 65. Maximum: 5.

The CRB-65 is the same score without urea (0–4), for use without laboratory tests.

## Limits and population

The 2003 CURB-65 was derived and validated in hospitalized adults with community-acquired pneumonia, using initial-assessment data and 30-day mortality. Age ≥ 65 is a component of the score, not the minimum eligibility age. The original thresholds use urea \> 7 mmol/L, respiratory rate ≥ 30/min and systolic BP \< 90 or diastolic BP ≤ 60 mmHg. Exclusions and use in other populations require reading the full protocol.

## References

- [Lim WS et al. Defining community acquired pneumonia severity on presentation to hospital: an international derivation and validation study. Thorax, 2003.](https://doi.org/10.1136/thorax.58.5.377)

- [Lim WS et al. BTS guidelines for the management of community acquired pneumonia in adults: update 2009. Thorax, 2009.](https://doi.org/10.1136/thx.2009.121434)

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
