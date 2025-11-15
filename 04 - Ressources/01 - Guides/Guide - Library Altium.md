
---
## Introduction

Ce document a pour objectif d’expliquer comment utiliser la librairie Altium : comment créer des composants, les utiliser, organiser correctement la librairie, ainsi que comprendre comment elle a été conçue et dans quel but.

La librairie de nos composants est sensible à la casse. Pour que le développement de nos PCB se déroule au mieux et que tout reste correctement organisé, nous vous demandons de faire preuve de rigueur lors de son utilisation. Si vous n’êtes pas certain de ce que vous faites, ne modifiez rien et demandez l’avis du responsable électrique.

**Sommaire**

- [[#Étape 1]]
- [[#Étape 2]]
- [[#Étape 3]]
- [[#Étape 4]]
- [[#Conclusion]]
- [[#Ressources utiles]]]

**Historique de Version**

| Version | Auteur           | Date       | Description      |
| ------- | ---------------- | ---------- | ---------------- |
| 1       | Corentin Coueron | 2025-10-01 | Version Initiale |
|         |                  |            |                  |

**Materiel Requis :**
- Odinateur
- Altium
- Obsidian

---
## Organisation de la library

Quand on developper des carte et des circuit electronqiue avoir acces a une liberary prorpre est ce qu'il y a de mieux et de plus agreable. Nous avon sdonc developper une library de compossantes complete afin de pourvour les utiliser facument.

Notre maniere de penser est simple, eviter au mximum de devoir importer une composante durant la conception.

Car pour faire monter les composant sur nos carte par une entrperise tels que JLCPCB nous avons besoin que la conception de nos carte soit bine unifirme et corresponde au standar attendu et dans les composant ajouter par internet directement les standar sont souvent pas respecter et donc on doit les modifier a la maij ce qui augemente le nombre d'erreur possible.

Pour celq nous avons developper une gamme tres complette des standare d'emprinte et de symbole de composant afin que vous ayer directemetn des models a prendre durant cotre conception et ne pas a avoir a importer des composante.

Voic i l'organisation des fichier dans altium : (rubrique Explorer)

SONIA Components
- Components templates (template generique utiliser pour la creation des composants)
- Generics Components
	- Generic Fooprint (enpreinte pcb)
	- Generic Symbol (desin shematics)
	- Generics Components Templates (les composant en entier)
- Specifics Components 
- la y'a des truc arjouter niomralement

Components template :
C'est une template de composant generique tel que tout les composant de type resitance condo induct . Cq sert a quand je va cree un nouveau model ou composant tu va pouvoir utliser ce template generic et il va te mettre correctemnt les bon parametred





Description de la première étape. Essayez de détailler le plus possible ce que vous voulez expliquer. Il y a rarement **trop** d’explications.  

Dites-vous que ce que vous allez écrire sera probablement lu par quelqu’un dans plusieurs années, et il faudra que cette personne comprenne clairement ce que vous avez fait.

Exemple de tableau :

| Numéro des PCB | Tension 1 | Tension 2 | Tension 3 |
|----------------|-----------|-----------|-----------|
| PCB1           | 24V       | 12V       | 9V        |
| PCB2           | 24V       | 12V       | 9V        |
| PCB3           | 24V       | 12V       | 9V        |

> Vous pouvez aussi ajouter des notes pour apporter plus de précision.

---
## Cree la library

Ci dessous vous aller retoeuver les differente etpape que nious avons fait pour cree la library, il est a but purrament informatif et aussi si on veux faire une modification ca nous permet de nous rappler comment nous l'avons fait.





N’hésitez pas à ajouter des bouts de code si nécessaire, mais pensez à les formater pour une meilleure lisibilité.

```c
#include <stdio.h>

int main() {

    printf("Hello World");

    return 0;

}
```

Et si vous utilisez des commandes Linux ou Windows, utilisez également des blocs de code pour permettre au lecteur de faire un simple copier-coller.

```bash
sudo apt update
```

Cela peut aussi servir à mettre en évidence des noms particuliers.  
Par exemple, il est important d’avoir toujours une fonction `main` dans un projet de programmation.

---
## Étape 3

Lors de vos expérimentations, n’hésitez pas à inclure les calculs nécessaires : résistance de LED, diviseur de tension dans un schéma, puissance d’un moteur, etc.

$$

R = \frac{U - V_{LED}}{I}

$$

Si vous souhaitez faire référence à un autre fichier dans vos notes, vous pouvez insérer un lien Obsidian comme ceci :  

[[Nom du fichier de référence]]

---
## Étape 4

Vous pouvez également faire des listes ou des démarches étape par étape avec un format lisible.

Dans **Apple** :
- Réglages > Informations Système > Supprimer l’OS.
- Ensuite, soyez heureux.

Voilà comment faire une bonne action.

---
## Conclusion

Terminez par une belle conclusion, et n’oubliez pas de mettre votre nom et la date pour garder une trace de qui a écrit quoi.  

Cela peut être important pour l’historique.

Enfin, une fois votre guide terminé, **n’oubliez pas de faire un push vers le serveur pour bien sauvegarder votre travail.**


---
## Ressources utiles

- [Loi d’Ohm – Wikipédia](https://fr.wikipedia.org/wiki/Loi_d%27Ohm)
- [Code des couleurs des résistances (outil)](https://www.digikey.fr/en/resources/conversion-calculators/conversion-calculator-resistor-color-code)

---
**Auteur – Date**