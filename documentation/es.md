<!-- ELUCENIA technical documentation · funcao-discriminante-de-maddrey · es · no clinical/professional/rights approval -->

# Función discriminante de Maddrey

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/funcao-discriminante-de-maddrey)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Tiempo de protrombina del paciente

`tp`

s · intervalo: 5–150

### Tiempo de protrombina de control

`tpc`

s · intervalo: 5–30

### Bilirrubina total

`bili`

mg/dL · intervalo: 0,1–80

## Edición del método

Maddrey modificada/Carithers 1989: 4,6×(TP paciente−TP control)+bilirrubina; no ecuación original de TP absoluto 1978

## Fórmula documentada

FD = 4,6 × (TP del paciente − TP control, en segundos) + bilirrubina total (mg/dL).

## Límites y población

La función original de 1978 se estudió en hepatitis alcohólica. La forma modificada local, con diferencia de tiempo de protrombina y punto de corte 32, debe corresponder a la edición posterior de 1989. El total no sustituye la evaluación de contraindicaciones, infección y diagnósticos alternativos antes de cualquier decisión terapéutica.

## Referencias

- [Maddrey WC et al. Corticosteroid therapy of alcoholic hepatitis. Gastroenterology, 1978.](https://doi.org/10.1016/0016-5085(78)90401-8)

- [Carithers RL et al. Methylprednisolone therapy in patients with severe alcoholic hepatitis: a randomized multicenter trial. Ann Intern Med, 1989.](https://doi.org/10.7326/0003-4819-110-9-685)

- [Crabb DW et al. Diagnosis and treatment of alcohol-associated liver diseases: 2019 practice guidance from the American Association for the Study of Liver Diseases. Hepatology, 2020.](https://doi.org/10.1002/hep.30866)

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

FD < 32: hepatitis alcohólica no grave según este criterio


### 2

FD ≥ 32: hepatitis alcohólica grave, considerar corticoide


### 3

FD ≥ 32: hepatitis alcohólica grave, considerar corticoide

