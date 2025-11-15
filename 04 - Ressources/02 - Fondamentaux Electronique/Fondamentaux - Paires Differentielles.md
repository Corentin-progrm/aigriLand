### Definition
Une paire différentielle, dans la conception de PCB, est une paire de pistes ou de fils qui transportent des signaux égaux mais opposés, souvent utilisés pour transmettre des données à haute vitesse et améliorer la résistance au bruit
Les paires différentielles émettent des champs magnétiques égaux et opposés qui se neutralisent mutuellement et peuvent produire une diaphonie inductive plus faible qu'un signal asymétrique.

#### Parametres d'une paire differentielle
Il existen un grqnd nombre de pare differenteille (USB, Ethernet, HDMI...), mais chcune a une particulariter en fonction de son utiliter et des infor;ation donner dans la datacheet de composant qui l4utilise.

Grace cette informations omn peut donc connaitre les caracteristiaue a prendre en compte de la paire differentielle sur un PCB.
- La resistance de differenteille (trouvable dans datasheet)
- La largeur de la trace. (W)
- L'espace entre les trace differentielle (S)
- L'espace entre la trace et un plan (de masse ou autre) (H)

![[Pasted image 20250605092834.png]]
Poure calculer toutes ses caracteristiaue, je vous conseille d'utiliser le logicielle [SaturnPCB](https://saturnpcb.com/saturn-pcb-toolkit/) dans la rubrique "Differential Pairs / XTALK".
#### Utilisation avec Altium
##### Dans le Shematics
Pour declarer une paire differentielle dans le shematics altium, les layer s concerner doivent etre renomer avec ce format : 
```
NOM_DE_VOTRE_PAIRE_N
NOM_DE_VOTRE_PAIRE_P
```
Ensuite vous devez y rajouter le symbole de la paire differentielle (Place>Directives>Deffirential Paires), cela permet de valider pour altium que ce sont bine des paire differentielle.

![[Pasted image 20250605100953.png]]

##### Dans le PCB

pour parametrer les caracteristiaue des paire diff, design>rules
Design rules>Routing>Differential Paire routing>DiffPaire_USB

exemple d'uen rules pour une paire de usbc2.0 avec 90ohm de resitance
![[Pasted image 20250605101249.png]]
