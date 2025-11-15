
---
## Introduction

Ce guide vise à expliquer, dans l'ordre, toutes les différentes étapes d'un projet, de sa création à sa finalisation.  
Nous vous demandons de suivre ce guide autant que possible afin d'assurer une certaine rigueur et une uniformisation dans l'ensemble de nos projets. Cela permet une meilleure transmission des connaissances au fil du temps.

Afin de mieux illustrer cette documentation, le projet **P001 - (mettre un nom)** sert d'exemple. C’est un projet de base assez simple, dont vous pouvez consulter les documents (sans les modifier). Il sert de référence à suivre pour le déroulement de votre propre projet.

**Sommaire**

- [[#Étape 1 - Specifications]]
- [[#Étape 2 - Synoptique]]
- [[#Étape 3 - Altium]]
- [[#Étape 4 - Checklists et Revues]]
- [[#Étape 5 - Inspection, Tests & ECO]]
- [[#Conclusion]]
- [[#Ressources utiles]]

**Historique de version**

|Version|Auteur|Date|Description|
|---|---|---|---|
|1.0|Corentin Coueron|2025-08-05|Version initiale|

**Matériel requis :**
- Ordinateur

---
## Étape 1 - Specifications

Les spécifications d'un projet représentent l'ensemble des différentes fonctions et caractéristiques que celui-ci doit remplir. Il ne s'agit pas uniquement des caractéristiques électroniques d'une carte, mais aussi des aspects physiques, comme la visibilité d'une LED, sa taille, ou encore son intégration mécanique, etc.

Par expérience, cette première phase peut sembler peu utile ou trop longue, mais elle est en réalité essentielle. Elle vous aidera non seulement dans la conception du schéma électrique, mais aussi dans les étapes de validation.  
Surtout, elle permet de clarifier les besoins de votre projet afin d'éviter les zones d’ombre avant de commencer la conception.

Pour cela, vous devez remplir la page **Specifications** du fichier Excel **Pxxx - Documentation**.

**Fonctionnement de la page :**

- **Bloc fonctionnel** : Permet de catégoriser les requis ; cela aide par la suite dans le développement du circuit électrique.

- **Numéro** : Numérotation des requis pour les identifier plus facilement.

- **Description** : Décrit simplement le besoin à remplir dans le cadre du projet.
    

Une fois cette page remplie, vous devez la faire relire par le responsable **ELE**, afin de vous assurer que tous les requis nécessaires à la conception de la carte sont présents et obtenir un avis extérieur.

> Je vous conseille d’aller consulter le projet exemple **P001 - (à nommer)** pour mieux vous faire une idée de ce que vous devez écrire.

---
## Étape 2 - Synoptique

Un _synoptique_ est un mot un peu compliqué pour désigner un schéma haut niveau de votre système.  
Pour faire simple : c’est un dessin avec tous les blocs fonctionnels de votre projet et les différentes connexions.  
Il s'agit d'un schéma général : ne rentrez pas trop dans les détails, l’objectif est qu’il soit compréhensible par quelqu’un qui ne connaît pas le projet.

Pour réaliser ce dessin, vous pouvez utiliser la fonction **Canvas** dans Obsidian, le sauvegarder, puis ranger le fichier dans le dossier de votre projet.

N’oubliez pas d’ajouter dans votre documentation un **lien vers le synoptique**, accompagné d’un petit texte explicatif. Un peu de contexte est toujours utile.

---
## Étape 3 - Altium

Le moment est venu de créer votre projet **Altium**. Vous pouvez suivre les étapes de création à l’aide de ce guide : _(mettre le lien du guide)_.  
Pensez à bien respecter les étapes pour partir sur une bonne base de projet.

_(Je n’ai rien d’autre à ajouter dans cette section pour le moment, mais on pourra la compléter au besoin.)_

---
## Étape 4 - Checklists et Revues

Dans le fichier Excel de votre projet, vous trouverez les pages **Checklists** et **Revues**, qui se composent de 4 sections :

- **Checklist de Conception** : Permet de vérifier que rien n’a été oublié dans le circuit électrique.

- **Revue de Conception** : Permet à votre relecteur de noter ses remarques.

- **Checklist de Layout** : Vérifie que vous n’avez rien oublié dans la phase de placement/routage.

- **Revue de Layout** : Permet au relecteur de commenter cette phase.


Ces documents vous servent à la fois de mémo pour ne pas oublier d'étapes importantes, et d'outil de communication avec votre relecteur, qui pourra y noter directement ses remarques ou suggestions.

Dans les checklists, vous n’avez qu’à cocher si une action a été réalisée ou non. Si elle ne s'applique pas, indiquez-le, avec une brève justification.

Dans les pages de revue, notez les erreurs détectées (sur les composants ou générales), et précisez si vous avez apporté une correction. Le relecteur pourra alors valider cette correction.

---
## Étape 5 - Inspection, Tests & ECO

Une fois que vous avez reçu vos PCB, vous pouvez passer à cette étape pour bien préparer la mise en route.  
Je vous conseille de préparer ces documents à l’avance — certains doivent être remplis avant même la fabrication.

Dans le fichier Excel, trois pages sont dédiées à cette phase :

- **Suivi** : Liste tous les PCB du projet, avec leurs versions et modifications.

- **Tests** : Détaille les différents tests réalisés lors de la mise en route.

- **ECO** (_Engineering Change Order_) : Documente les modifications à prévoir pour les versions suivantes.

**Suivi**
Indiquez tous les PCB liés au projet, leur version matérielle, les reworks effectués (modification de composants, etc.), la version firmware (si applicable), et précisez si la carte fonctionne comme prévu.

**Tests**
La mise en route nécessite de tester correctement votre carte pour valider son fonctionnement.  
Réalisez les tests prévus, et documentez-les dans la colonne "Notes" : précisez les points de test, les broches utilisées, les composants testés, etc. Cela permettra à une autre personne de reproduire et valider les mêmes vérifications.

**ECO**
Lors de la vérification de votre PCB, vous constaterez probablement des erreurs ou ajustements nécessaires.  
Dans la page ECO, pour chaque problème constaté, remplissez : le bug ou erreur rencontrée, le patch temporaire appliqué et le correctif définitif prévu pour la version suivante

N'oubliez pas de remplir les autres colonnes importantes (version, date, etc.).

> Il est important de compléter ces documents **au fur et à mesure** pour assurer un bon suivi du projet.

---
## Conclusion

Toutes ces étapes sont très importantes : elles permettent de créer des projets plus fiables et facilitent la transmission des informations.  
L’objectif est qu’un autre membre puisse reprendre, modifier, améliorer, tester ou simplement utiliser votre projet, même plusieurs mois ou années plus tard.

---
## Ressources utiles

- _(Ajouter le lien vers le dossier du projet P001)_

---
**Corentin Coueron – 2025-08-06**
