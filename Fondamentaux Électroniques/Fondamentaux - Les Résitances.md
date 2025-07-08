## Introduction
Ce document fait partie d'une série de notes sur les bases de l’électronique. L’objectif est d’expliquer de manière claire et structurée les composants essentiels, leur rôle, leur fonctionnement, et comment les utiliser dans des projets concrets.  
Ici, on se penche sur **les résistances**, un des composants les plus courants en électronique.

---
## Partie théorique

### Qu’est-ce qu’une résistance ?
Une résistance est un composant électronique passif dont le rôle est de **limiter le courant électrique** dans un circuit.  
Elle obéit à la loi d’Ohm :  
\[
U = R \times I
\]  
où :
- \( U \) est la tension (en volts),
- \( I \) est le courant (en ampères),
- \( R \) est la résistance (en ohms, \( \Omega \)).

### Types de résistances
- Résistances fixes (axiales, CMS)
- Résistances variables (potentiomètres, trimmers)
- Résistances de puissance, résistances de précision

### Code couleur des résistances
Les résistances axiales utilisent un **code de couleur** pour indiquer leur valeur. Exemple :
- Rouge – Violet – Marron – Or → **270 Ω ±5 %**

---
## Exemple pratique

### Cas d’utilisation : Limiter le courant dans une LED
Pour protéger une LED, on insère une résistance en série pour limiter le courant.

#### Exemple :
Tension d'alimentation : 5 V  
Tension LED : 2 V  
Courant souhaité : 20 mA

Calcul de la résistance :
\[
R = \frac{5V - 2V}{0.02A} = 150\,\Omega
\]

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