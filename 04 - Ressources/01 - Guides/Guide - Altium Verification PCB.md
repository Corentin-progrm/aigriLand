
Avant de commencer

|                                                                                                            |                                                                  |
| ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
| Vérification des capacités de manufacture minimum pour les largeur de traces (width/clearance) et les vias | voir comment on fait pour savoir ca et le mettree dans les rules |
| Vérification des capacités de manufacture des vias et des "Annular ring"                                   | pareil voir comment on fait pour verif ca avant                  |

PLacement

|                                                                                                                                                              |                                                                                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Verifier l'Aspect visuel du placement et l'alignement des composants                                                                                         | essayer de faire auelaue chose de relativement beau                                                                                                        |
| Optimisation du placement des composants pour obtenir des pistes les plus courtes                                                                            |                                                                                                                                                            |
| Verifier présence de zone libre autour de chaque IC pour faciliter l'assemblage automatisé, le controle et la réparation.                                    |                                                                                                                                                            |
| Vérifier zone libre autour et sous connecteurs                                                                                                               |                                                                                                                                                            |
| Veirifer zone libre autour des trous mécaniques (par défaut, 2.5mm)                                                                                          |                                                                                                                                                            |
| Les condensateurs de découplage sont-ils placés au plus près des alimentations des circuits intégrés ?                                                       |                                                                                                                                                            |
| Es ce que les conneceur de communication avec la carte sont bine placer et ne pose pas de probme mecaniaue                                                   | faire attention au connecteur JTAG et tout les autre connecteur, ne pas oublier que la mianiere dont il se connecte peut poser certsain probleme mecaniaue |
| Valider aue les element de visulaisation comme des led ou un ecarant sdont bine visible par l'utilisateur                                                    | du gnere pas cacher par un connecteur                                                                                                                      |
| Valider aue les hauterus des composant les plus grand ne vienne pas en interference mecaniaue avec d'autre coposant ou carte qui pour etre localiser a coter |                                                                                                                                                            |
|                                                                                                                                                              |                                                                                                                                                            |

Routage 

|                                                                                                                     |                                                                            |
| ------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| Pas d'angles 90º                                                                                                    |                                                                            |
| Absence de fentes ou d'angle aigu                                                                                   |                                                                            |
| appliquer le teardrop                                                                                               | tools>therdrop>objects (selewct all)>ok                                    |
| Absence de zone isolée (islands, dead copper)                                                                       |                                                                            |
| Controle des longueur des pistes (verifier au'il n'y a rie nd'aberant par rapport a la taille du PCB)               | Panels>PCB>Nets (trier par longueur)                                       |
| Afin d’éviter tout couplage capacitif ou par induction, vérifier les traces qui se longent sur de longues distances | On est surtout pour des signaux sensible comme du spi                      |
| Paires différentielles avec le moins de via possible                                                                |                                                                            |
| Matcher les longueurs de traces sur une paire différentielle (ex. USB ou chaque canal de MIPI)                      | Panels>PCB>Nets (trier par nom) on doit avoir une difference de longeur de |
| Matcher les longueurs des paires différentielles multiples (ex. MIPI)  - ajouter accordéons                         |                                                                            |
| Multiplication des « vias » de masse entre plans de masse?                                                          | tools>via stitching>add stitching to net                                   |
|                                                                                                                     |                                                                            |
Indistrualisations et testabiliter

|                                                                           |                                                                                     |
| ------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| Controle de la présence de Test Point et Regroupement sur une seule face. | les test point doivent etre des via de tel taille pour y mettre des crochet de test |
|                                                                           |                                                                                     |
Mécanique et Layout

|                                                                                           |                                                 |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------- |
| Le pinout des connecteurs est bien identifié sur le silkcreen et visible le plus possible | ex: VBAT, GND                                   |
| Marquage silkcreen                                                                        | ex: sérigraphie, Version, logo client et motsai |
|                                                                                           |                                                 |
