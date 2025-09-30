
---
## Introduction

Cette documentation vise à retracer le contexte de création de ce projet, mais aussi à fournir des explications techniques sur l'intégration mécanique ainsi que sur certaines fonctions complexes nécessitant plus de précision. Évidemment, cette documentation est en lien avec le fichier Excel associé à ce projet.

**Sommaire**

- [[#Contexte & Besoin]]
- [[#Fonctions principales]]
- [[#Integration mecanique]]
- [[#BOM & Prix]]
- [[#Conclusion]]
- [[#Ressources utiles]]

**Historique de version**

| Version | Auteur           | Date       | Description      |
| ------- | ---------------- | ---------- | ---------------- |
| 1.0     | Corentin Coueron | 2025-09-29 | Version initiale |

---
## Contexte & Besoin

Le projet **P002 - HLM** est né de la volonté de refaire l’intégralité de l’électronique présente dans les sous-marins, afin de la rendre plus fiable, amovible et mieux adaptée aux besoins actuels de l’équipe électrique et des sous-marins.

Cette documentation constitue le cahier des charges général du projet HLM. Nous verrons plus bas que ce grand projet sera découpé en plusieurs sous-projets, correspondant la plupart du temps à une carte électronique dédiée, qui viendra ensuite s’assembler avec les autres pour constituer le projet HLM complet.

---
## Synoptique

Ci-dessous, vous trouverez le synoptique du projet, représentant à haut niveau ses fonctions principales.

Attention ceci n'a pas encore ete valider par l'equipe

![[Pasted image 20250929210931.png]]



---
## Fonctions principales

Ci-dessous, vous trouverez plus de détails sur les fonctions principales du projet :

- **Convertisseur de tension**  
    Le convertisseur de tension permet de transformer une tension fixe de 5 V en une tension fixe de 3,3 V. Le convertisseur utilisé peut fournir un courant de sortie élevé (jusqu’à 1 A), afin de répondre aux besoins des utilisateurs.
    
- **Sélecteur de tension**  
    Les sélecteurs de tension permettent de basculer facilement entre deux niveaux d'alimentation (5 V ou 3,3 V) pour chacune des deux lignes d'alimentation de la breadboard.


---
## Integration mecanique





---
## BOM & Prix

Ci-dessous, vous trouverez une liste des composants principaux du projet, ainsi que leur prix, afin d’estimer le coût total du projet.  
Dans le but de réduire les coûts, les quantités indiquées sont basées sur une production de 10 cartes.

| Composantes     | Quantite | Supplier | Manufacturer Part Number | Prix      |
| --------------- | -------- | -------- | ------------------------ | --------- |
| PCB             | 10       | JLCPCB   |                          | ??        |
| Regulateur      | 10       | Digikey  | AP62300TWU-7             | 3.22$     |
| Header 2x3      | 20       | Digikey  | M20-9980346              | 5.92$     |
| Switch          | 20       | Digikey  | SLW-1678105-6A-N-D       | 17.82$    |
| USB-C           | 10       | Digikey  | USB4105-GF-A             | 9.48$     |
| Header 1x2      | 10       | Digikey  | 691137710002             | 4.70$     |
| **Total/carte** |          |          |                          | **4.11$** |

---
## Conclusion

Ce projet, qui a pour but de développer les compétences en conception de cartes électroniques chez les nouveaux membres, est volontairement simple à mettre en place et peu coûteux. Il permet aux nouveaux membres de réaliser leur première carte électronique.

---
## Ressources utiles

- [[P001-Synoptique.canvas|P001-Synoptique]]

---
**Corentin Coueron – 2025-08-06**
