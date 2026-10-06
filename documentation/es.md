<!-- ELUCENIA technical documentation · curb-65 · es · no clinical/professional/rights approval -->

# CURB-65

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/curb-65)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Confusión mental (nueva desorientación en tiempo, lugar o persona)

`c`

### Urea \> 42 mg/dL (\> 7 mmol/L)

`u`

### FR ≥ 30 respiraciones/min

`r`

### Presión sistólica \< 90 mmHg o diastólica ≤ 60 mmHg (B: presión arterial)

`b`

### Edad ≥ 65 años

`i`

## Edición del método

CURB-65/Lim 2003: confusión, urea\>7 mmol/L, FR≥30, presión arterial, edad≥65; 0–5

## Fórmula documentada

Un punto por ítem: C (confusión), Urea \> 7 mmol/L, R (frecuencia respiratoria) ≥ 30/min, B (presión baja: PAS \< 90 o PAD ≤ 60 mmHg) y edad ≥ 65. Máximo: 5.

El CRB-65 es igual sin urea (0–4), para uso sin laboratorio.

## Límites y población

El CURB-65 de 2003 se derivó y validó en adultos hospitalizados con neumonía adquirida en la comunidad, utilizando datos de la evaluación inicial y mortalidad a 30 días. La edad ≥ 65 es un componente de la puntuación, no la edad mínima de elegibilidad. Los umbrales originales utilizan urea \> 7 mmol/L, frecuencia respiratoria ≥ 30/min y presión arterial sistólica \< 90 o diastólica ≤ 60 mmHg. Las exclusiones y el uso en otras poblaciones requieren leer el protocolo completo.

## Referencias

- [Lim WS et al. Defining community acquired pneumonia severity on presentation to hospital: an international derivation and validation study. Thorax, 2003.](https://doi.org/10.1136/thorax.58.5.377)

- [Lim WS et al. BTS guidelines for the management of community acquired pneumonia in adults: update 2009. Thorax, 2009.](https://doi.org/10.1136/thx.2009.121434)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

Bajo riesgo: mortalidad a 30 días del 1,5%

| Detalles del resultado | |
| --- | --- |
| CRB-65 (sin la urea) | 0 (bajo riesgo (mortalidad < 1%)) |
| Conducta sugerida | Candidato para tratamiento ambulatorio, si no hay otro motivo para internación. |


### 2

Riesgo intermedio: mortalidad a 30 días del 9,2%

| Detalles del resultado | |
| --- | --- |
| CRB-65 (sin la urea) | 2 (riesgo aumentado (1 a 10%): considerar derivación al hospital) |
| Conducta sugerida | Considerar hospitalización (o una breve observación supervisada). |


### 3

Alto riesgo: mortalidad a 30 días de 22%

| Detalles del resultado | |
| --- | --- |
| CRB-65 (sin la urea) | 3 (alto riesgo (> 10%): hospitalización urgente) |
| Conducta sugerida | Ingresar; con 4 o 5 puntos, evaluar la necesidad de UCI. |


### 4

Bajo riesgo: mortalidad a 30 días del 1,5%

| Detalles del resultado | |
| --- | --- |
| CRB-65 (sin la urea) | 0 (bajo riesgo (mortalidad < 1%)) |
| Conducta sugerida | Candidato para tratamiento ambulatorio, si no hay otro motivo para internación. |

