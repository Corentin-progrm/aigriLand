
---

## Introduction

Ce document vise a garder en memeoire les differentes modification, reparation des projet antierieur. afin de pouvoir les reutiliser si beasoin et de ce souvenir des erreur passer.

**Sommaire**

- [[#ECOs]]
- 
- [[#Ressources utiles]]

**Historique de version**

| Version | Auteur           | Date       | Description      |
| ------- | ---------------- | ---------- | ---------------- |
| 1.0     | Corentin Coueron | 2025-11-15 | Version initiale |


---
## ECOs

**Designateur : U5  
Part number : PI4ULS5V201TAEX**

**Problème :**  
Une résistance de pull-down (R16) est placée en externe sur la broche 1, alors qu’une pull-up interne est déjà présente. Cela crée un diviseur de tension et entraîne une consommation de courant inutile. La tension d’entrée reste néanmoins dans la plage acceptable, donc le circuit fonctionne, mais ce n’est pas optimal.

**Solution :**  
Retirer la résistance de pull-down R16.

---

**Designateur :** Q1 et Q2  
**Part number :** DMG2305UX-13

**Problème :** Le MOSFET en question a un absolute maximum rating de ±8 V pour le Vgs, alors que le Vgs peut atteindre –16,8 V en fonctionnement normal, entraînant probablement sa défaillance.

**Solution :** Remplacer le MOSFET par un modèle supportant ±20 V en Vgs. On utilise donc un **SI3407-TP**.


---

**Designateur :   
Part number : **

**Problème :**  

**Solution :**  


---
## Verifications

Cette partie vise a mettre clairement les valeur de fonctionnemetn attentdu durant les tests dans different constexte afin de valider qu'on a bien des valeur attendu

- **Alimentation :** 16.3V


**Cartes utilisées :** Main, MCU, Safety.
- **Tension KILL ON (0V) :** 0.24A
- **Tension KILL OFF (5V) :** 0.03A

**Cartes utilisées :** Main, MCU, Safety, Motor (x1).
- **Tension KILL ON (0V) :** 0.03A
- **Tension KILL OFF (5V) :** 0.28A

 **Cartes utilisées :** Main, MCU, Safety, Motor (x2).
- **Tension KILL ON (0V) :** 0.03A
- **Tension KILL OFF (5V) :** 0.31A

**Cartes utilisées :** Main, MCU, Safety, Motor (x3).
- **Tension KILL ON (0V) :** 0.03A
- **Tension KILL OFF (5V) :** 0.35A

**Cartes utilisées :** Main, MCU, Safety, Motor (x4).
- **Tension KILL ON (0V) :** 0.03A
- **Tension KILL OFF (5V) :** 0.39A


****



---


## Notes complémentaires

- [Bonne pratique 1]
- [Bonne pratique 2]

---

## Ressources utiles

- [[Nom de la ressource – Source]](lien)
- [[Calculateur ou outil en ligne]](lien)

---

**Auteur : Corentin Couëron – 15-11-25**
