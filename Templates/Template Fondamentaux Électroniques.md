# Titre : Fondamentaux — Nom 

## Introduction

Ce document fait partie d'une série de notes sur les bases de l’électronique. L’objectif est d’expliquer de manière claire et structurée les composants essentiels, leur rôle, leur fonctionnement, et comment les utiliser dans des projets concrets. 

---
## Partie théorique

La résistance électrique traduit la propriété d'un composant à s'opposer au passage d'un courant électrique. Elle est souvent désignée par la lettre R et son unité de mesure l'ohm (symbole : Ω). Elle est liée aux notions de résistivité et de conductivité électrique.

La résistance est responsable d'une dissipation d'énergie sous forme de chaleur. Cette propriété porte le nom d'effet Joule. Cette production de chaleur est parfois un effet souhaité (résistances de chauffage), parfois un effet néfaste (pertes Joule) mais souvent inévitable.

Elle obéit à la **loi d'Ohm**, qui s'exprime par la relation :

$$
U = R \cdot I
$$
avec :

- $U$ : tension aux bornes de la résistance (en volts, V)  
- $I$ : intensité du courant traversant la résistance (en ampères, A)  
- $R$ : valeur de la résistance (en ohms, $\Omega$)

### Types de résistances
- Résistances fixes (axiales, CMS)
- Résistances variables (potentiomètres, trimmers)
- Résistances de puissance, résistances de précision

---
## Exemple pratique

### Cas d’utilisation : Limiter le courant dans une LED
Pour protéger une LED, on insère une résistance en série pour limiter le courant.
#### Exemple :
Tension d'alimentation : 5 V  
Tension LED : 2 V  
Courant souhaité : 20 mA

Calcul de la résistance :
$$
R = \frac{5V - 2V}{0.02A} = 150\,\Omega
$$

> 💡 Il faut choisir une résistance de **150 Ω**. La plus proche norme E12 serait 150 Ω ou 180 Ω.

---
## Intégration dans Altium Designer

### Démarche :
1. **Placer une résistance dans le schéma**
   - Ouvrir le schéma.
   - Taper `R` pour ajouter une résistance (`Place > Component` si besoin).
   - Sélectionner une résistance dans la librairie (ex: `RESISTOR`).

2. **Configurer ses propriétés**
   - Double-cliquer pour définir la valeur (ex: `150R`).
   - Vérifier la puissance si nécessaire.

3. **Ajouter les empreintes (footprint)**
   - Associer l’empreinte correspondant au format physique (ex: `0603`, `1/4W axial`).

4. **Routage sur le PCB**
   - Vérifier l'espacement, placer proche de la LED.
   - Si CMS, vérifier les pads et le masque de soudure.

---
## Notes complémentaires
- Pour de meilleurs résultats, toujours choisir une résistance avec une **marge de sécurité** de puissance (ex: ne pas faire passer 0.5W dans une 0.25W).
- Utiliser une **librairie standardisée** dans Altium facilite la gestion des composants.

---
## Ressources utiles
- [Loi d’Ohm – Wikipédia](https://fr.wikipedia.org/wiki/Loi_d%27Ohm)
- [Code des couleurs des résistances (outil)](https://www.digikey.fr/en/resources/conversion-calculators/conversion-calculator-resistor-color-code)

---
**Nom de l’auteur – Date**