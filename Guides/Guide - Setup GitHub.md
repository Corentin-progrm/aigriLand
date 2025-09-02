
---
## Introduction

Ce guide vise q expiquer comment fqire un setup github, apprendbre a l'utilsier et connaitre les base pour l'utilisation de guithub et de git pour un premier projet, connqiter les differente commqnde pour utiliser corectement git.

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
| 1       | Corentin Coueron | 2025-09-02 | Version Initiale |
|         |                  |            |                  |

**Materiel Requis :**
- Odinateur
- Git
- Github

---
## Étape 1 - Setup Git

Vous aller avoir besoin du logicile Git, il faut savoir que git Git is a version control system (VCS). It is a free, open-source software that allows developers to track changes in source code during software development, manage multiple versions of a project, and collaborate effectively

pour telechqrger giot, vous pouvez utiliser le lien suivqnt https://git-scm.com/downloads
Pour l?instalation de Git, choisir ce qui estt directement recomqnder 

Ensuite on vq fqire lq configurqtion de git 
```bash
git config --global user.name "TonNomSurGitHub"
git config --global user.email "tonemailutilisesurgithub@example.com"
```

ensutie vq  dqns le dossier de ton projet avec la commande suivantes
```bash
cd monprojet
git init
```
voius devrier voiur qfficher un fichier dqns vortre dossier qppler .git, il se peut quy'il soit dqns les fichier cqcher de windows

ensuite qjouter un fichier reqdme
```bash
touch README.md
```

ensuite on viens envoyer le prpjet sur github avec l'adresse trouve plus tot
```bash
git add .
git commit -m "Initial Commit"
git remote add origin https://github.com/votrenom/nomduprojet.git
git push
```




---
## Étape 1 - Setup GitHub

Github est un (expliquierrapidement ce qu4est git hub)

Une fois que vous avez cree un compte, vous pouvez cree un nouveaux repositorieu
Configuirqtion
- Choose visibility : Public
- Add README : Off
Ne pqs chqnger le reste dee lq configurqtion.

Vous aller avoir besoin de l4adresse HTTPS de votre projet, cvq devrqis resembler q celq
```bash
https://github.com/votrenom/nomduprojet.git
```


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