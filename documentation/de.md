<!-- ELUCENIA technical documentation · funcao-discriminante-de-maddrey · de · no clinical/professional/rights approval -->

# Maddrey-Diskriminanzfunktion

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/funcao-discriminante-de-maddrey)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Prothrombinzeit des Patienten

`tp`

s · Bereich: 5–150

### Kontroll-Prothrombinzeit

`tpc`

s · Bereich: 5–30

### Gesamtbilirubin

`bili`

mg/dL · Bereich: 0,1–80

## Fassung der Methode

Modifizierter Maddrey/Carithers 1989: 4,6×(Patienten-PT−Kontroll-PT)+Bilirubin; ohne Originalformel mit absoluter PT 1978

## Dokumentierte Formel

DF = 4,6 × (Prothrombinzeit Patient − Kontrolle, in Sekunden) + Gesamtbilirubin (mg/dL).

## Grenzen und Population

Die Originalfunktion von 1978 wurde bei alkoholischer Hepatitis untersucht. Die modifizierte lokale Form mit Prothrombinzeitdifferenz und Schwelle 32 muss zur späteren Ausgabe von 1989 passen. Die Summe ersetzt vor jeder Therapieentscheidung nicht die Bewertung von Kontraindikationen, Infektion und alternativen Diagnosen.

## Referenzen

- [Maddrey WC et al. Corticosteroid therapy of alcoholic hepatitis. Gastroenterology, 1978.](https://doi.org/10.1016/0016-5085(78)90401-8)

- [Carithers RL et al. Methylprednisolone therapy in patients with severe alcoholic hepatitis: a randomized multicenter trial. Ann Intern Med, 1989.](https://doi.org/10.7326/0003-4819-110-9-685)

- [Crabb DW et al. Diagnosis and treatment of alcohol-associated liver diseases: 2019 practice guidance from the American Association for the Study of Liver Diseases. Hepatology, 2020.](https://doi.org/10.1002/hep.30866)

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
