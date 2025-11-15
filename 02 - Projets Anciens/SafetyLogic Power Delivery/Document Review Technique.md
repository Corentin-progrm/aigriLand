
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


**Designateur :   
Part number : **

**Problème :**  

**Solution :**  





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
