
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
## Étape 2 - Setup Git

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
git branch -M main
git push -u origin main
```

Vous pouvez ensuite qller verifier que sur votre github vous avez bine voptre proejt avec le fichoer readme qui a bien ete ajouter.

---
## Commandes classique

**Commande Versionage**
```bash
git add .
git commit -m "nomducommit"
git push
```



---
## Probleme Classique

**Ajout de fichier .vs**
Si vous avex un projet avec visdual studio il est possible que vous ayerz des fichier avec un .vs
Pour egler ce genre de probleme il faut ignorer les fichiers 

Exemple de probleme
```bash
$ git add .
error: open("P002-Finance-Software/.vs/P002-Finance-Software/FileContentIndex/8677dbd9-7e80-424f-b092-052ffe7e4bbb.vsidx"): Permission denied
error: unable to index file 'P002-Finance-Software/.vs/P002-Finance-Software/FileContentIndex/8677dbd9-7e80-424f-b092-052ffe7e4bbb.vsidx'
fatal: adding files failed
```

vous pouvez faire ca pour fixer votre projet

```bash
cd votreprojet
touch .gitignore
```

ouvre et ajoute
```bash
.vs/
*.user
*.suo
*.tmp
*.log
```

3. Sauvegarde `.gitignore`.
4. Supprime les fichiers déjà indexés par Git (s’ils ont été ajoutés avant) :
```bash
git rm -r --cached .vs
```

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