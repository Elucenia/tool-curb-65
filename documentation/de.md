<!-- ELUCENIA technical documentation · curb-65 · de · no clinical/professional/rights approval -->

# CURB-65

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/curb-65)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### C: Verwirrtheit (neue Desorientierung zu Zeit, Ort oder Person)

`c`

### U: Harnstoff \> 42 mg/dL (\> 7 mmol/L)

`u`

### Atemfrequenz ≥ 30 Atemzüge/min

`r`

### Systolischer Blutdruck \< 90 mmHg oder diastolischer ≤ 60 mmHg (B: Blutdruck)

`b`

### Alter ≥ 65 Jahre

`i`

## Fassung der Methode

CURB-65/Lim 2003: Verwirrtheit, Harnstoff\>7 mmol/L, Atemfrequenz≥30, Blutdruck, Alter≥65; 0–5

## Dokumentierte Formel

Ein Punkt je Item: C (Verwirrtheit), U (Harnstoff) \> 7 mmol/L, R (Atemfrequenz) ≥ 30/min, B (niedriger Blutdruck: systolisch \< 90 oder diastolisch ≤ 60 mmHg) und Alter ≥ 65. Maximum: 5.

Der CRB-65 ist derselbe Score ohne Harnstoff (0–4), ohne Labor einsetzbar.

## Grenzen und Population

CURB-65 von 2003 wurde bei hospitalisierten Erwachsenen mit ambulant erworbener Pneumonie anhand der Erstbeurteilung und 30-Tage-Mortalität entwickelt und validiert. Alter ≥ 65 ist eine Scorekomponente, kein Mindestalter für die Eignung. Die Originalschwellen sind Harnstoff \> 7 mmol/L, Atemfrequenz ≥ 30/min und systolischer Druck \< 90 oder diastolischer Druck ≤ 60 mmHg. Ausschlüsse und Anwendung in anderen Populationen erfordern die Lektüre des vollständigen Protokolls.

## Referenzen

- [Lim WS et al. Defining community acquired pneumonia severity on presentation to hospital: an international derivation and validation study. Thorax, 2003.](https://doi.org/10.1136/thorax.58.5.377)

- [Lim WS et al. BTS guidelines for the management of community acquired pneumonia in adults: update 2009. Thorax, 2009.](https://doi.org/10.1136/thx.2009.121434)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Niedriges Risiko: 30-Tage-Mortalität von 1,5%

| Ergebnisdetails | |
| --- | --- |
| CRB-65 (ohne Harnstoff) | 0 (niedriges Risiko (Mortalität < 1%)) |
| Vorgeschlagenes Vorgehen | Kandidat für eine ambulante Behandlung, wenn es keinen anderen Grund für eine Aufnahme gibt. |


### 2

Mittleres Risiko: 30-Tage-Mortalität von 9,2%

| Ergebnisdetails | |
| --- | --- |
| CRB-65 (ohne Harnstoff) | 2 (erhöhtes Risiko (1 bis 10%): Krankenhauseinweisung erwägen) |
| Vorgeschlagenes Vorgehen | Krankenhausaufnahme erwägen (oder kurze überwachte Beobachtung). |


### 3

Hohes Risiko: 30-Tage-Mortalität von 22%

| Ergebnisdetails | |
| --- | --- |
| CRB-65 (ohne Harnstoff) | 3 (hohes Risiko (> 10%): dringende Krankenhausaufnahme) |
| Vorgeschlagenes Vorgehen | Aufnehmen; bei 4 oder 5 Punkten den Bedarf an einer Intensivstation beurteilen. |


### 4

Niedriges Risiko: 30-Tage-Mortalität von 1,5%

| Ergebnisdetails | |
| --- | --- |
| CRB-65 (ohne Harnstoff) | 0 (niedriges Risiko (Mortalität < 1%)) |
| Vorgeschlagenes Vorgehen | Kandidat für eine ambulante Behandlung, wenn es keinen anderen Grund für eine Aufnahme gibt. |

