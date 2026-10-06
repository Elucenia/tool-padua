<!-- ELUCENIA technical documentation · padua · fr · no clinical/professional/rights approval -->

# Score de Padoue

[conditions, sources et autorisations](https://elucenia.org/fr/outils/padua)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Cancer actif (métastase ou chimiothérapie/radiothérapie dans les 6 derniers mois)

`cancer`

### Antécédent de MTEV (hors thrombose veineuse superficielle)

`tev`

### Mobilité réduite (alitement avec accès aux toilettes pendant ≥ 3 jours)

`mobilidade`

### Thrombophilie connue

`trombofilia`

### Traumatisme ou chirurgie au cours du dernier mois

`trauma`

### Âge ≥ 70 ans

`idade`

### Insuffisance cardiaque et/ou respiratoire

`icc`

### Infarctus aigu du myocarde ou AVC ischémique

`iam`

### Infection aiguë et/ou maladie rhumatologique

`infeccao`

### Obésité (IMC ≥ 30 kg/m²)

`obesidade`

### Traitement hormonal en cours

`hormonio`

## Édition de la méthode

Padua Prediction Score/Barbar 2010 : 11 facteurs, 0–20 ; patient médical hospitalisé

## Formule documentée

3 points : cancer actif, MTEV antérieure, mobilité réduite, thrombophilie · 2 points : traumatisme ou chirurgie récente · 1 point : âge ≥ 70, insuffisance cardiaque/respiratoire, infarctus du myocarde ou AVC ischémique, infection aiguë ou maladie rhumatologique, obésité, hormonothérapie. Maximum : 20.

## Limites et population

Le Padua a été étudié chez des patients médicaux hospitalisés en médecine interne, avec suivi des thromboembolies symptomatiques jusqu’à 90 jours. La stratification thrombotique doit s’accompagner d’une évaluation des saignements, des contre-indications et du protocole de prophylaxie. Le total ne remplace pas cette analyse et n’implique pas une application automatique à la population chirurgicale.

## Références

- [Barbar S et al. A risk assessment model for the identification of hospitalized medical patients at risk for venous thromboembolism: the Padua Prediction Score. J Thromb Haemost, 2010.](https://doi.org/10.1111/j.1538-7836.2010.04044.x)

- [Kahn SR et al. Prevention of VTE in nonsurgical patients: antithrombotic therapy and prevention of thrombosis, 9th ed: American College of Chest Physicians evidence-based clinical practice guidelines. Chest, 2012.](https://doi.org/10.1378/chest.11-2296)

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

Faible risque : TVE à 0,3 % sans prophylaxie

La prophylaxie pharmacologique n’est pas indiquée ; encourager la mobilisation.


### 2

Risque élevé : TVE à 11 % sans prophylaxie

Indiquer une thromboprophylaxie pharmacologique (HBPM, héparine non fractionnée ou fondaparinux) s’il n’existe pas de risque hémorragique élevé.


### 3

Risque élevé : TVE à 11 % sans prophylaxie

Indiquer une thromboprophylaxie pharmacologique (HBPM, héparine non fractionnée ou fondaparinux) s’il n’existe pas de risque hémorragique élevé.

