# Diodes

Ce document fait partie d'une série de notes sur les bases de l’électronique. L’objectif est d’expliquer de manière claire et structurée les composants essentiels, leur rôle, leur fonctionnement, et comment les utiliser dans des projets concrets.

**Sommaire**

- [[#Partie théorique]]
- [[#Paramètres à considérer]]
- [[#Exemple pratique]]
- [[#Intégration dans Altium Designer]]
- [[#Ressources utiles]]

---

## Partie théorique

Une **diode** est un composant électronique passif qui **laisse passer le courant dans un seul sens** (sens direct), et **le bloque dans l’autre sens** (sens inverse).

### Caractéristiques principales :
- En **polarisation directe**, la diode commence à conduire à partir d’une **tension seuil** ($V_f$), typiquement autour de **0.7 V pour une diode silicium**, et **0.3 V pour une diode germanium**.
- En **polarisation inverse**, elle bloque le courant **jusqu’à sa tension de claquage** ($V_{BR}$), au-delà de laquelle elle peut être endommagée (sauf dans le cas des diodes Zener).

Formule simplifiée :
- En direct : $U \approx V_f$
- En inverse : $I \approx 0$

### Types courants :
- **Diode de redressement** (1N4007, etc.)
- **Diode rapide / Schottky** (BAT54, 1N5819)
- **Diode Zener** (stabilisation de tension)
- **Diode de signal** (1N4148)
- **Diode de roue libre** (pour protéger contre les surtensions dans les bobines)

---

## Paramètres à considérer

Liste des paramètres importants à prendre en compte pour choisir une diode.

| Nom du paramètre        | Description                                                   | Valeur(s) typique(s)       |
|-------------------------|---------------------------------------------------------------|-----------------------------|
| Tension directe ($V_f$) | Tension minimale nécessaire pour qu’elle conduise             | 0.7 V (silicium), 0.3 V (germanium), 0.2 V (Schottky) |
| Courant maximal ($I_f$) | Courant maximal admissible en direct                          | 100 mA – 1 A – 3 A+         |
| Tension inverse ($V_R$) | Tension inverse maximale supportée sans claquage              | 50 V – 1000 V               |
| Temps de commutation    | Temps de passage du blocage à la conduction                   | µs (diode lente), ns (rapide) |
| Type / usage            | Type de diode (redressement, signal, roue libre, Zener...)    | 1N4001, 1N4148, ZM4728, etc. |
| Package / Case          | Format physique                                               | DO-35, SOD-123, SMA, etc.   |
| Polarité                | Composant polarisé : **cathode = trait sur le symbole**       | Oui                         |

---

## Exemple pratique

### Cas d’utilisation : Protection d’un relais avec une diode de roue libre

Lorsqu’on coupe le courant traversant une **bobine (relais, moteur, solénoïde)**, celle-ci génère une **surtension inverse** (induction de Lenz). Une diode en **roue libre** permet d’absorber cette surtension et de **protéger le transistor ou le circuit de commande**.

#### Schéma :
- Diode connectée **en parallèle sur la bobine**, cathode vers le +V, anode vers la masse.
- Quand la bobine est coupée, le courant passe par la diode et s’éteint en douceur.

#### Choix de la diode :
- **1N4007** pour relais standard
- **1N5819** pour des temps de commutation plus rapides (Schottky)

---

## Intégration dans Altium Designer

### Démarche :
1. **Placer une diode dans le schéma**
   - Ouvrir le schéma
   - Taper `D` ou chercher dans `Place > Component`
   - Choisir une diode standard (`DIODE`, `1N4007`, `ZENER`, etc.)

2. **Configurer ses propriétés**
   - Nom du composant, tension directe, type
   - Vérifier la polarité dans le symbole (cathode marquée)

3. **Ajouter les empreintes (footprint)**
   - Choisir selon le format physique (ex: `DO-35`, `SOD-123`, `SMA`, CMS, etc.)

4. **Routage sur le PCB**
   - Respecter le sens de la diode
   - Pour une diode de roue libre, placer au plus près du relais/moteur
   - Prévoir un bon plan de masse si protection contre surtension

---

## Notes complémentaires

- Une **diode Zener** est conçue pour fonctionner en **polarisation inverse** pour la régulation de tension.
- Une **diode Schottky** a une **tension directe très basse** (~0.2 V), idéale pour les circuits basse tension.
- Les **diodes rapides** sont indispensables pour les signaux numériques ou les commutations rapides (SMPS, PWM, etc.)
- Pour la **détection de polarité inversée**, on peut placer une diode en série à l’entrée d’un circuit.

---

## Ressources utiles

- [Diode – Wikipédia](https://fr.wikipedia.org/wiki/Diode)
- [Diodes – SparkFun Guide](https://learn.sparkfun.com/tutorials/diodes)
- [Calculateur de résistance Zener](https://www.digikey.fr/en/resources/conversion-calculators/conversion-calculator-zener-resistor)

---

**Auteur : [Ton Nom] – [Date]**
