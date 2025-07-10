## Introduction

Ce guide vise a connaitre la materile de soudure, comrndre theoriament ce qu'est qu'une soudure puis commnet s'exercer de maniere praitaue.

Nous sommes conciens aue certain de nos memebre sortie du cegep n'on roboable;ent jmais fait ou tres peut de soudure et malheureusement il y a tres peut de contexte ou vous pourrez l'apprendre a l'ets. Pourtant cette aspect techniaue est importanmt a avoir maitriser, en effet emem en tant aue ingenieur et surtout dans le dommine de l'electroniaue, il va vous arriver reguliere de de voir modifier des carte ou des prototype par vous meme pour faire des test par exemple. Il faut donc aue vous conniassiez les base de la soudure.

**Sommaire**

- [[#Materiels Utilises]]
- [[#Differents Type de soudure]]
- [[#Les erreus de soudures]]
- [[#Conclusion]]
- [[#Ressources utiles]]]

**Historique de Version**

| Version | Auteur           | Date       | Description      |
| ------- | ---------------- | ---------- | ---------------- |
| 1       | Corentin Coueron | 2025-07-10 | Version Initiale |
|         |                  |            |                  |

**Materiel Requis :**
- Boot ELE
- PCB
- Composantes electronique

---
## Materiels Utilises

Vous aller retouver ici la liste des outils aue nous utilisons mjoritairement pour faire de la soudure avec un petit explications de leur utilisations

Liste du materils

| Nom            | Description                                                                                           | Digikey Part Number |
| -------------- | ----------------------------------------------------------------------------------------------------- | ------------------- |
| Poste a souder | Appareil qui permet de chauffer le fer a souder a la temperature souhaiter                            | FM203-01            |
| Fer a souder   | Sous forme d'une tige ne metale, elle permet de faire fondre l'etein pour souder les composant        | T0058770715         |
| Pince          | Outils qui permet de manipuler les composant avec prescision                                          |                     |
| Brass coil     | Laine de laiton qui permet de netoyer votre fer a souder                                              | AOREF98B            |
| Etein          | Metale aui permet de souder les composant entre eux                                                   |                     |
| Flux           | Produit chimique permettant de faciliter la soudure                                                   |                     |
| Alchool 99.9%  | Alcholl blanc presaue pur qui permet de nethoyer les carte apres une soudire                          |                     |
| Pate a brser   | Melange chimiaue de flux et d'etind. sous forme de pate elepermet de souder les composant via un four |                     |
> Le digikey part number est present pour donner une illustration du produit

---
## Differents Type de soudure

Il existe diffeentes maniere de souder des composant sur un pcb, elle ontoute des point fort et des point faible

**Soudure par refusion**
sur une carte vierge, on y depose de la pates a souder, (malnge d'etein et de flux) sur les emperinte des composant, ensuite on y depose les composant dessus puis on chuaffe la carte soit a l'ai 'un four soit avec un fer a air chaud
Un fois la temperature atteinte on va pouvoir voir la pate a souder se mettre en fusion et soude le pad au composant juste au dessus.

**Soudure au fer a souder**
La soudure au fer a souder est la techniaue la plus classiaue. Il s'agit dd'utiliser le fer a souder pur deposer de l'etain en fusion sur les pad u composant et ensuite d'apporter a la main le composant sur sont pad et d'utiliser le fer pour mettre ne fusion l'einte , position le composant et enlever son fer pour aue l'etain refroidisse


---
## Les erreus de soudures

**Court-circuits et ponts de soudure**
C,es lorsque il y a une connexion entre 2 pate  ou deux composant, cela peut cree un court circuit dnas votre circuit et donc cree des dommage.

**Soudure insuffisante**
Une quantité de soudure trop faible peut entraîner des joints faibles ou incomplets, causant des problèmes de connexion électrique. 

**Billes de soudure**
Lorsaue vous souder, des petite bille de soudure peuvent etre eclbousser sur le PCB et creee involontairement des court cirtcuit, pour eviter cela il faut prendre le temps de netoyer ca carte

**Mauvais alignement des composants**
Lorsaue vous souder des composant actigf avec plusieurs pates, il y a une risaue que si vous n'alligner pas correctement le composant il peut y avoir un defaut de soudure 

**Soudure sèche ou froide**
Des joints de soudure poreux ou mal formés peuvent résulter de températures incorrectes ou de techniques de soudure inappropriées. Cela peut provoquer des sudure briser prematureement.  

**Contamination**
Des impuretés comme la saleté ou la poussière peuvent empêcher une bonne soudure et causer des problèmes électriques.  

**Soudure de GND**
Si votre carte possede un GND tres grand, il peut rendre la soudure du composant tres compliauer il faut donc bine prendre le temps de bien chauffer sa carte pour aue la fusion se fasse correctement.

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
**Corentin Coueron – 2025-07-10**