<!-- ELUCENIA technical documentation · funcao-discriminante-de-maddrey · fr · no clinical/professional/rights approval -->

# Fonction discriminante de Maddrey

[conditions, sources et autorisations](https://elucenia.org/fr/outils/funcao-discriminante-de-maddrey)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Temps de prothrombine du patient

`tp`

s · intervalle: 5–150

### Temps de prothrombine témoin

`tpc`

s · intervalle: 5–30

### Bilirubine totale

`bili`

mg/dL · intervalle: 0,1–80

## Édition de la méthode

Maddrey modifiée/Carithers 1989 : 4,6×(TP patient−TP témoin)+bilirubine ; sans équation originale TP absolu 1978

## Formule documentée

DF = 4,6 × (temps de prothrombine du patient − témoin, en secondes) + bilirubine totale (mg/dL).

## Limites et population

La fonction originale de 1978 a été étudiée dans l’hépatite alcoolique. La forme locale modifiée, avec une différence de temps de prothrombine et un seuil de 32, doit correspondre à l’édition ultérieure de 1989. Le total ne remplace pas l’évaluation des contre-indications, de l’infection et des diagnostics alternatifs avant toute décision thérapeutique.

## Références

- [Maddrey WC et al. Corticosteroid therapy of alcoholic hepatitis. Gastroenterology, 1978.](https://doi.org/10.1016/0016-5085(78)90401-8)

- [Carithers RL et al. Methylprednisolone therapy in patients with severe alcoholic hepatitis: a randomized multicenter trial. Ann Intern Med, 1989.](https://doi.org/10.7326/0003-4819-110-9-685)

- [Crabb DW et al. Diagnosis and treatment of alcohol-associated liver diseases: 2019 practice guidance from the American Association for the Study of Liver Diseases. Hepatology, 2020.](https://doi.org/10.1002/hep.30866)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

FD < 32 : hépatite alcoolique non sévère selon ce critère


### 2

FD ≥ 32 : hépatite alcoolique sévère, envisager un corticostéroïde


### 3

FD ≥ 32 : hépatite alcoolique sévère, envisager un corticostéroïde

