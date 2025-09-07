Ce guide vise à exposer les différentes démarches à effectuer une fois le schéma ou le PCB terminé, afin de nous assurer que tout a été fait correctement et d’éviter les erreurs bêtes pouvant entraîner la fabrication d'une nouvelle version de PCB et le rachat de composants.

## Validation du schema

Project->Validate PCB Project xxx
- Verfier toutes les erreurs pressente dans le panel message

View->Panel->Navigator
- Verfier dans la liste des Net qu'il n'y a pas d'erreur du type VBAT et VABTT (genre d'erreur de frappe qui peut coser des probleme)

## Revue du schema

PXXX - Checklists et Revue
- Ajoute le fichier de checklist dans le dossier du projet.

> La il faut ajouter les etapes de verifcation de shematics

## Bill of Materials

Verification des composant de la BOM
- Regarder les duplication de coposant
- Reduire au maximum le nombre de composant differents
- uniformiser la taille des composant (0603)

Choisir les composant generiaue (resitance, condo ect...)
- Cliquer sur le composant, Ajouter digikey en premier (ou mouseur)
- mettre le composant en 5 etoile pour le selectionner
- le logo a droite du tableau devrais se mettre en clear= (vert) pour valider le choix correct

Choisr un composant non generiaue (IC, microcontroler...0)
- cliauer sur sont copomsoant
- cliauer sur add Solution
- cliauer sur edit part choice 
- cliauer sur add
- mettre sont composant trouver par e part number puis ajouter avec OK
- Ensuiteselctionner le fournisseur (preference pour digikey puis mouseur)
- Puis mettre 5 etoile

## Layout

Design->Import change to .PcbDoc
- On verifei au'on a rien oublier d'inmporter

Design->Layer Stack Manager
- On verifie aue sont layer stack est correctement mis de la bonne taille

Place->Dimension->Lineare
- On vine mettre les dimension de la carte sur la couchemechanical 1

Tools->Polygon pour->polygone manager
- On viens verifier si tout nos polygone sont correct qu'il on bine leur nets correct et qu'il ne sont pas shelve

tools->via stinching/shelding->Add stiching to net
- On viens rajouter le via stitching on peut garder les pqrqmetre de bqse
> Verififier si on garde les parametre de base car tout les altium on peut etre pas les meme partametre

Clique droit sur un pad->find similare object->Shape (all layers)
	->selectionne Rectangular
	->selectionne Same
	->Apply puis OK
- Ca va venir selectionner tout les pad aui sont rectangulaire.
	->Panel->proprieter->Pad stack
	->on change le shape pour Rounded rectangulare
	->et on change le raduis pour 10%

Verification des proprieter des pad thermorelif
- Verifier aue les pad aui non pas de thermal relifs sont bien voulus

Tools->Teardrop
- Ajouter des teardrop sur les pad pour avoir une meilleur connexion

Remplir le document de verification du layout et faire faire une revue



