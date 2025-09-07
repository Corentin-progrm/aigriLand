
---
## Introduction

Ce guide a pour but de vous faire découvrir le matériel de soudure, de comprendre théoriquement ce qu’est une soudure, puis de vous apprendre comment vous exercer de manière pratique.

Nous sommes conscients que certains membres sortant du cégep n’ont probablement jamais soudé, ou très peu, et qu’il existe malheureusement peu de contextes pour apprendre à le faire à l’ÉTS. Pourtant, cet aspect technique est essentiel à maîtriser. En effet, même en tant qu’ingénieur — et surtout dans le domaine de l’électronique — il vous arrivera régulièrement de devoir modifier des cartes ou des prototypes vous-même, par exemple pour faire des tests. Il est donc important de connaître les bases de la soudure.

**Sommaire**

- [[#Matériels utilisés]]
- [[#Différents types de soudure]]
- [[#Les erreurs de soudure]]
- [[#Exercice de soudure]]
- [[#Conclusion]]
- [[#Ressources utiles]]

**Historique de version**

| Version | Auteur           | Date       | Description      |
| ------- | ---------------- | ---------- | ---------------- |
| 1       | Corentin Coueron | 2025-07-10 | Version initiale |

**Matériel requis :**

- Boot ELE
- PCB
- Composantes électroniques

---
## Matériels utilisés

Vous trouverez ici la liste des outils que nous utilisons majoritairement pour faire de la soudure, avec une courte explication de leur utilité.

| Nom                 | Description                                                                         | Digikey Part Number |
| ------------------- | ----------------------------------------------------------------------------------- | ------------------- |
| Poste à souder      | Appareil qui permet de chauffer le fer à souder à la température souhaitée          | FM203-01            |
| Fer à souder        | Tige métallique utilisée pour faire fondre l’étain et souder les composants         | T0058770715         |
| Pince               | Outil permettant de manipuler les composants avec précision                         |                     |
| Laiton (brass coil) | Laine de laiton utilisée pour nettoyer la panne du fer à souder                     | AOREF98B            |
| Étain               | Métal utilisé pour souder les composants entre eux                                  |                     |
| Flux                | Produit chimique facilitant la soudure en évitant l’oxydation                       |                     |
| Alcool 99,9 %       | Alcool presque pur utilisé pour nettoyer les cartes après soudure                   |                     |
| Pâte à braser       | Mélange d’étain et de flux sous forme de pâte, utilisé pour la soudure par refusion |                     |

> Le numéro Digikey est fourni à titre d’illustration.

---
## Différents types de soudure

Il existe différentes manières de souder des composants sur un PCB. Chacune a ses avantages et ses inconvénients.

### Soudure par refusion

Sur une carte vierge, on dépose de la pâte à souder (mélange d’étain et de flux) sur les empreintes des composants. Ensuite, on place les composants sur les pads, puis on chauffe la carte à l’aide d’un four ou d’un fer à air chaud.

Une fois la température atteinte, la pâte fond et fixe le composant sur le pad.

### Soudure au fer à souder

C’est la méthode la plus classique. Elle consiste à chauffer l’endroit de la soudure avec le fer, à déposer de l’étain fondu sur le pad du composant, puis à placer manuellement le composant dessus. On retire ensuite le fer pour que l’étain se solidifie.

---
## Les erreurs de soudure

**Court-circuits et ponts de soudure**
Ce sont des connexions indésirables entre deux pattes ou deux composants. Elles peuvent causer des courts-circuits et endommager la carte.

**Soudure insuffisante**
Une quantité trop faible d’étain peut provoquer une mauvaise connexion électrique ou une soudure fragile.

**Billes de soudure**
Des éclaboussures d’étain fondu peuvent se déposer sur le PCB. Ces petites billes peuvent causer des courts-circuits. Il est important de nettoyer votre carte après chaque soudure.

**Mauvais alignement des composants**
Un mauvais alignement des composants, surtout ceux avec plusieurs pattes, peut empêcher une soudure correcte ou rendre le circuit inutilisable.

**Soudure sèche (ou froide)**
Ce type de soudure survient quand la température est trop basse ou que la technique est mal appliquée. L'étain ne fait pas une bonne liaison avec le pad, ce qui peut entraîner des défaillances électriques prématurées.

**Contamination**
La saleté, la poussière ou les résidus de flux peuvent nuire à une bonne adhérence et créer des problèmes de conduction. Il est donc important de garder les cartes propres.

**Soudure sur plan de masse (GND)**
Quand une carte possède un large plan de masse, il faut plus de temps pour le chauffer correctement. Sinon, l’étain ne fondra pas ou la soudure ne tiendra pas bien. Prenez le temps de bien chauffer la zone.

---
## Exercice de soudure

Ajouter un exercice de soudure du premier PCB du tuto Altium.


---
## Conclusion

La soudure est une compétence essentielle pour tout membre du club, surtout ceux impliqués dans l’électronique. Même si ce n’est pas enseigné formellement à l’ÉTS, c’est un savoir qui vous servira toute votre carrière.

N’hésitez pas à vous exercer régulièrement avec le matériel du club, à poser des questions aux membres plus expérimentés.

---
## Ressources utiles

- 

---
**Corentin Coueron – 2025-07-10**