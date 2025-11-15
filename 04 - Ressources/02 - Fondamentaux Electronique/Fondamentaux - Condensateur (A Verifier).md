# Condensateurs

Ce document fait partie d'une série de notes sur les bases de l’électronique. L’objectif est d’expliquer de manière claire et structurée les composants essentiels, leur rôle, leur fonctionnement, et comment les utiliser dans des projets concrets.

**Sommaire**

- [[#Partie théorique]]
- [[#Paramètres à considérer]]
- [[#Exemple pratique]]
- [[#Intégration dans Altium Designer]]
- [[#Ressources utiles]]

---
## Partie théorique

Un **condensateur** est un composant électronique passif capable de stocker de l’énergie sous forme de champ électrique entre deux conducteurs séparés par un isolant (le diélectrique).

La **capacité** d’un condensateur, notée $C$, s’exprime en **farads (F)**. Elle dépend de la surface des plaques, de la distance qui les sépare et de la constante diélectrique du matériau isolant.

Le comportement d’un condensateur dépend du signal :
- Il **s’oppose aux variations rapides** de tension.
- Il **laisse passer le courant alternatif** (AC) mais **bloque le courant continu** (DC) une fois chargé.

Formule de la charge :
$$
Q = C \cdot U
$$

Relation courant-tension dans un condensateur :
$$
I(t) = C \cdot \frac{dU(t)}{dt}
$$

---
## Paramètres à considérer

Liste des paramètres importants à prendre en compte pour choisir un condensateur.

| Nom du paramètre       | Description                                                              | Valeur(s) typique(s)       |
|------------------------|---------------------------------------------------------------------------|-----------------------------|
| Capacité               | Quantité de charge qu’il peut stocker pour une tension donnée            | 100 nF, 10 µF, 1 µF         |
| Tension nominale       | Tension maximale qu’il peut supporter sans risque de claquage            | 16 V, 25 V, 50 V, etc.      |
| Type / technologie     | Matériau utilisé : céramique, électrolytique, tantale, film, etc.         | Céramique, électrolytique   |
| Polarité               | Certains sont polarisés (à connecter dans le bon sens)                   | Oui (électrolytiques)       |
| Package / Case         | Format physique (CMS ou traversant)                                      | 0603, 0805, radial           |
| Tolérance              | Variation admissible de la valeur réelle                                 | ±5 %, ±10 %, ±20 %          |
| ESR (Résistance série) | Résistance interne qui affecte les performances à haute fréquence        | < 1 Ω (céramique), > 1 Ω (électro) |

---
## Exemple pratique

### Cas d’utilisation : Filtrage d’une alimentation 5 V

Pour stabiliser une alimentation et réduire les variations de tension (bruit, ripple), on place des condensateurs entre l’alimentation et la masse.

#### Exemple :
- Alimentation : 5 V régulée
- Objectif : filtrer les pics de bruit haute fréquence
- Choix :
  - **1 µF céramique (CMS)** pour filtrer le HF
  - **100 µF électrolytique** pour lisser le ripple à basse fréquence

> Bonnes pratiques :
> - Placer les condensateurs de découplage **au plus proche des broches d’alimentation** des circuits intégrés.
> - Mélanger **petite capacité (rapide)** et **grande capacité (lent)** pour une meilleure couverture en fréquence.

---
## Intégration dans Altium Designer

### Démarche :
1. **Placer un condensateur dans le schéma**
   - Ouvrir le schéma.
   - Taper `C` pour ajouter un condensateur (`Place > Component` si besoin).
   - Sélectionner un condensateur dans la librairie (ex : `CAP`, `CAPACITOR`).

2. **Configurer ses propriétés**
   - Double-cliquer pour définir la valeur (ex : `100n`, `10uF`).
   - Vérifier la tension nominale et la polarité si applicable.

3. **Ajouter les empreintes (footprint)**
   - Associer l’empreinte correspondant au format physique (ex : `0603`, `radial`, `electrolytic`).

4. **Routage sur le PCB**
   - Placer au plus près des VCC / GND des circuits critiques.
   - Vérifier que les plans de masse et d'alimentation sont bien connectés.

---
## Notes complémentaires

- Un condensateur **polarisé** (électrolytique, tantale) doit **toujours être connecté dans le bon sens**.
- Les condensateurs **céramiques** sont non polarisés et idéaux pour le **découplage rapide**.
- Attention à la **tension de service** : toujours garder une **marge de sécurité** d’au moins 20 %.
- Certains condensateurs céramiques voient leur **valeur chuter avec la tension** (effet non linéaire à surveiller !)

---
## Ressources utiles

- [Condensateur – Wikipédia](https://fr.wikipedia.org/wiki/Condensateur)
- [Types de condensateurs – SparkFun](https://learn.sparkfun.com/tutorials/capacitors/all)
- [Calculateur de filtre RC](https://www.digikey.fr/en/resources/conversion-calculators/conversion-calculator-low-pass-filter)

---
**Auteur : [Ton Nom] – [Date]**
