<!-- ELUCENIA technical documentation · curb-65 · fr · no clinical/professional/rights approval -->

# CURB-65

[conditions, sources et autorisations](https://elucenia.org/fr/outils/curb-65)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Confusion mentale (désorientation nouvelle dans le temps, le lieu ou les personnes)

`c`

### Urée \> 42 mg/dL (\> 7 mmol/L)

`u`

### FR ≥ 30 respirations/min

`r`

### Pression systolique \< 90 mmHg ou diastolique ≤ 60 mmHg (B : pression artérielle)

`b`

### Âge ≥ 65 ans

`i`

## Édition de la méthode

CURB-65/Lim 2003 : confusion, urée\>7 mmol/L, FR≥30, pression artérielle, âge≥65 ; 0–5

## Formule documentée

Un point par item : C (confusion), Urée \> 7 mmol/L, R (fréquence respiratoire) ≥ 30/min, B (pression basse : PAS \< 90 ou PAD ≤ 60 mmHg) et âge ≥ 65. Maximum : 5.

Le CRB-65 est identique sans urée (0–4), pour une utilisation sans laboratoire.

## Limites et population

Le CURB-65 de 2003 a été développé et validé chez des adultes hospitalisés pour une pneumonie communautaire, à partir de l’évaluation initiale et de la mortalité à 30 jours. L’âge ≥ 65 est un composant du score, pas l’âge minimal d’éligibilité. Les seuils originaux sont l’urée \> 7 mmol/L, la fréquence respiratoire ≥ 30/min et la pression systolique \< 90 ou diastolique ≤ 60 mmHg. Les exclusions et l’utilisation dans d’autres populations exigent la lecture du protocole complet.

## Références

- [Lim WS et al. Defining community acquired pneumonia severity on presentation to hospital: an international derivation and validation study. Thorax, 2003.](https://doi.org/10.1136/thorax.58.5.377)

- [Lim WS et al. BTS guidelines for the management of community acquired pneumonia in adults: update 2009. Thorax, 2009.](https://doi.org/10.1136/thx.2009.121434)

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
