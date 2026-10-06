<!-- ELUCENIA technical documentation · padua · de · no clinical/professional/rights approval -->

# Padua-Score

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/padua)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Aktiver Krebs (Metastasen oder Chemo-/Strahlentherapie in den letzten 6 Monaten)

`cancer`

### Frühere VTE (außer oberflächlicher Venenthrombose)

`tev`

### Verminderte Mobilität (Bettruhe mit Toilettengängen für ≥ 3 Tage)

`mobilidade`

### Bekannte Thrombophilie

`trombofilia`

### Trauma oder Operation im letzten Monat

`trauma`

### Alter ≥ 70 Jahre

`idade`

### Herz- und/oder Ateminsuffizienz

`icc`

### Akuter Myokardinfarkt oder ischämischer Schlaganfall

`iam`

### Akute Infektion und/oder rheumatologische Erkrankung

`infeccao`

### Adipositas (BMI ≥ 30 kg/m²)

`obesidade`

### Laufende Hormonbehandlung

`hormonio`

## Fassung der Methode

Padua Prediction Score/Barbar 2010: 11 Faktoren, 0–20; internistisch hospitalisierter Patient

## Dokumentierte Formel

3 Punkte: aktiver Krebs, frühere VTE, eingeschränkte Mobilität, Thrombophilie · 2 Punkte: kürzliches Trauma oder Operation · 1 Punkt: Alter ≥ 70, Herz-/Ateminsuffizienz, Herzinfarkt oder ischämischer Schlaganfall, akute Infektion oder rheumatologische Erkrankung, Adipositas, Hormontherapie. Maximum: 20.

## Grenzen und Population

Padua wurde bei internistisch hospitalisierten Patienten mit Nachverfolgung symptomatischer Thromboembolien bis zu 90 Tagen untersucht. Die Thromboserisikoeinteilung muss durch Bewertung von Blutung, Kontraindikationen und Prophylaxeprotokoll ergänzt werden. Die Summe ersetzt diese Analyse nicht und bedeutet keine automatische Anwendung auf chirurgische Populationen.

## Referenzen

- [Barbar S et al. A risk assessment model for the identification of hospitalized medical patients at risk for venous thromboembolism: the Padua Prediction Score. J Thromb Haemost, 2010.](https://doi.org/10.1111/j.1538-7836.2010.04044.x)

- [Kahn SR et al. Prevention of VTE in nonsurgical patients: antithrombotic therapy and prevention of thrombosis, 9th ed: American College of Chest Physicians evidence-based clinical practice guidelines. Chest, 2012.](https://doi.org/10.1378/chest.11-2296)

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

Niedriges Risiko: VTE bei 0,3 % ohne Prophylaxe

Eine medikamentöse Prophylaxe ist nicht indiziert; Mobilisation fördern.


### 2

Hohes Risiko: VTE bei 11 % ohne Prophylaxe

Pharmakologische Thromboseprophylaxe (LMWH, unfraktioniertes Heparin oder Fondaparinux) anzeigen, wenn kein hohes Blutungsrisiko besteht.


### 3

Hohes Risiko: VTE bei 11 % ohne Prophylaxe

Pharmakologische Thromboseprophylaxe (LMWH, unfraktioniertes Heparin oder Fondaparinux) anzeigen, wenn kein hohes Blutungsrisiko besteht.

