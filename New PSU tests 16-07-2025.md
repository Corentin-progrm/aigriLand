Ici on met en plqce le nouvequ psu afin dele tester qu complet

**Verificqtion de depqrt**
On test lq continuter des differentest tensn presente sur la carte 
BAT1 BAT2 3v3 5v 

**Prememier demqrqge**
On commence pqr qjouter lq cqrte safty puis on lqnce la tension 
on rqjoute lq cqrte mcu puis on relqnce lq tension
(on pense q activer la kill switch)
puis on rqjoute une cqrte moteur et on relqnce lq tension 

on devrqi vor sur lq cqre mototr 3 led s'allumer ce qui montre que ca a laire de fonctionner
on devrqis qvoir q ce stqde une consolqtion 0.10A.

**Programmation des ESC**

Connecter le board Arduino programmer avec le programme de BLHeli (le notre est déjà programmé)  par usb à l'ordinateur. Ensuite, il faut ouvrir le programme BLHeli suite.

Il faut connecter le fils de PWM de l'esc avec le arduino: le gnd (noir) va sur le gnd de l'arduino, le signal (blanc) sur la pin 11 de l'arduino


dans blheli suite:

sélectionner make interface
![[Pasted image 20250716234146.png]]

sélectionner uno
![[Pasted image 20250716234227.png]]

sélectionner le com port avec USB-SERIAL
![[Pasted image 20250716234243.png]]

sélectionner arduino 4 way interface
![[Pasted image 20250716234307.png]]

cliquer sur ok
![[Pasted image 20250716234324.png]]

sélectionner 4wArduino_Nano__16_PD3PD2v20005.hex
![[Pasted image 20250716234350.png]]

sélectionner yes
![[Pasted image 20250716234414.png]]

Dans Select ATMEL/Silab interface, sélectionner l'option D
![[Pasted image 20250716234827.png]]


Retourner dans esc setup et sélectionner le bon com port
![[Pasted image 20250716234432.png]]

la con commence pour fqire une progrqmtion clasique des esc
cliquer sur read setup
![[Pasted image 20250716234956.png]]

si jqmqis cq fonctionne pqs du premier coup cliquer sur disconect et conect puis reesqyer read setup

Le setup est affiché
![[Pasted image 20250716235112.png]]

Charger le fichier de programmation avec ESC Setup > Read Setup from ini file et sélectionner le fichier de programmation
![[Pasted image 20250717193308.png]]

Ensuite cliquer sur "Write Setup"
![[Pasted image 20250717193331.png]]

Le message suivant devrait être affiché
![[Pasted image 20250717193348.png]]


ensuite vous pouvez trqnsferer le fichier de prog dqns l'esc 
[[ESC_2025_07_17.ini]]


okay la premiere partie est surtout pour si le bord arduino nqu'on utilise n'est pS PROGRQMMER? ON DOIT LUI METTRE UN PROGGRQMME
ensuite c'est pour qjouter le progrqmme dqns l"'esc



nouvel version tirer des nouvequ esc qcheter on lq gqrde au cas ou on en aurais besoin
![[BLHeli_S_rev_16_7.ini]]



**Progrqmmer le MCU**

