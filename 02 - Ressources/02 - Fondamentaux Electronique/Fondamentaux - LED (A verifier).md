---

---

---
Ce document fait partie d'une série de notes sur les bases de l’électronique. L’objectif est d’expliquer de manière claire et structurée les composants essentiels, leur rôle, leur fonctionnement, et comment les utiliser dans des projets concrets.

**Sommaire**

- [[#Partie théorique]]
- [[#Paramètres à considérer]]
- [[#Exemple pratique]]
- [[#Intégration dans Altium Designer]]
- [[#Ressources utiles]]

---

## Partie théorique

Une **LED** (Light Emitting Diode) est une diode qui émet de la lumière lorsqu’un courant la traverse dans le sens direct. Elle ne fonctionne que dans un seul sens : **la cathode doit être connectée au GND**, et **l’anode à la tension d’alimentation via une résistance**.

Comme toute diode, elle présente une **tension directe** $V_f$ (forward voltage), qui varie selon la couleur :
- Rouge : ~1.8 V
- Vert : ~2.0 V
- Bleu / Blanc : ~3.0 – 3.3 V

Contrairement à une ampoule, une LED **ne supporte pas un courant trop élevé**, d’où l’importance d’ajouter une résistance pour limiter le courant.

---

## Paramètres à considérer

Liste des paramètres importants à prendre en compte pour choisir une LED.

| Nom du paramètre      | Description                                                  | Valeur(s) typique(s)     |
|-----------------------|--------------------------------------------------------------|---------------------------|
| Couleur / type        | Détermine la longueur d’onde / tension directe               | Rouge, Verte, Bleue, RGB  |
| Tension directe $V_f$ | Tension requise pour s’allumer                               | 1.8 V – 3.3 V             |
| Courant nominal       | Courant recommandé pour une bonne luminosité                | 5 mA – 20 mA              |
| Intensité lumineuse   | Luminosité en mcd (millicandela)                             | 100 – 2000 mcd            |
| Angle de vue          | Largeur du faisceau lumineux                                | 20° – 120°                |
| Polarité              | Composant polarisé, attention à l'orientation               | Oui                       |
| Package / Case        | Format physique                                              | CMS (0603, 0805), 5 mm, etc. |

---

## Exemple pratique

### Cas d’utilisation : Allumer une LED avec une résistance série

#### Données :
- Tension d’alimentation : 5 V
- Tension directe de la LED : 2 V (ex : LED rouge)
- Courant désiré : 10 mA

#### Calcul de la résistance :
$$
R = \frac{V_{alimentation} - V_f}{I} = \frac{5V - 2V}{0.01A} = 300\,\Omega
$$

> On choisira une valeur standard proche : **330 Ω**

> Pour une luminosité modérée, un courant de 5 mA est souvent suffisant.

---

## Intégration dans Altium Designer

### Démarche :
1. **Placer une LED dans le schéma**
   - Taper `P`, puis chercher `LED`, ou utiliser `Place > Component`
   - Choisir dans la librairie une LED adaptée (ex: `LED-RED`, `LED-RGB`)

2. **Configurer ses propriétés**
   - Nom, couleur, tension directe
   - Ajouter une résistance en série dans le schéma

3. **Ajouter les empreintes (footprint)**
   - Choisir selon le format physique (ex: `LED_0603`, `LED_TH_5MM`, `RGB_SMD`)

4. **Routage sur le PCB**
   - Respecter la polarité : anode/cathode
   - Placer la résistance en série à proximité si possible
   - Pour les LED CMS, vérifier les pads et le masque de soudure

---

## Notes complémentaires

- Une **LED connectée sans résistance** risque de griller instantanément.
- Toujours vérifier la **tension directe $V_f$** dans la datasheet du modèle utilisé.
- Les **LEDs RGB** comportent plusieurs LED dans un même b
