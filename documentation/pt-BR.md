<!-- ELUCENIA technical documentation · funcao-discriminante-de-maddrey · pt-BR · no clinical/professional/rights approval -->

# Função discriminante de Maddrey

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/funcao-discriminante-de-maddrey)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Tempo de protrombina do paciente

`tp`

s · intervalo: 5–150

### Tempo de protrombina controle

`tpc`

s · intervalo: 5–30

### Bilirrubina total

`bili`

mg/dL · intervalo: 0,1–80

## Edição do método

Modified Maddrey/Carithers 1989:4,6×(TPpaciente−TPcontrole)+bilirrubina; sem equação original TPabsoluto 1978

## Fórmula documentada

FD = 4,6 × (TP do paciente − TP controle, em segundos) + bilirrubina total (mg/dL).

## Limites e população

A função original de 1978 foi estudada em hepatite alcoólica. A forma modificada local, com diferença de tempo de protrombina e corte 32, precisa corresponder à edição posterior de 1989. O total não substitui avaliação de contraindicações, infecção e alternativas diagnósticas antes de qualquer decisão terapêutica.

## Referências

- [Maddrey WC et al. Corticosteroid therapy of alcoholic hepatitis. Gastroenterology, 1978.](https://doi.org/10.1016/0016-5085(78)90401-8)

- [Carithers RL et al. Methylprednisolone therapy in patients with severe alcoholic hepatitis: a randomized multicenter trial. Ann Intern Med, 1989.](https://doi.org/10.7326/0003-4819-110-9-685)

- [Crabb DW et al. Diagnosis and treatment of alcohol-associated liver diseases: 2019 practice guidance from the American Association for the Study of Liver Diseases. Hepatology, 2020.](https://doi.org/10.1002/hep.30866)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

FD < 32: hepatite alcoólica não grave por este critério


### 2

FD ≥ 32: hepatite alcoólica grave, considerar corticoide


### 3

FD ≥ 32: hepatite alcoólica grave, considerar corticoide

