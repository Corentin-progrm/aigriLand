### Definition Theorique
Une diode électroluminescente ( DEL ) est un dispositif  semi-conducteur qui émet de la lumière lorsqu'il est traversé par un Courant électrique. Les électrons du semi-conducteur se recombinent avec les trous d'électrons , libérant de l'énergie sous forme de photons.


$$
R = (Vs-Vled) / Iled
$$

#### Parametres a regarder

| Prametre Name                | Description                   | Valeur typique |
| ---------------------------- | ----------------------------- | -------------- |
| Voltage - Forward (Vf) (Typ) | Tension de drop de la led     | 2V             |
| Current - Test               | Consomation typique de la led | 20mA           |
Vous pouvez aussi regarder le package, la couleur et autre mais ces 2 parametre la sont les plus important dans la conceptions.
### Exemple Pratique
**Contexte :** On a une alimentation de 3V3 et on souhaite ajouter la led LTST-C190KFKT.
Qud on analyse la datasheet on contate que sont Voltage - Forward est de 2V et que ca consomation typiaue est de 20mA.

Etant donner que nous avons une alimentation de 3V3 il nous reste 1V3 (3V3 -3V) que nlus devons enlever grace par exemple a une resistance. En nous basant sur la calcult theoriaue

### Utilisation dans Altium

**Dans le Shematic :**

**Dans le PCB :**



```

```





on veux brancher une led sns info 

multimetre en mode diuode on mesure d'un coter open et de lÉ'autre la tension de drop 
la plus par du tps on veux que la led eclaire a 5ma amp c'est bine pas trop fort mais bine 
donc on clacul la resisance, ici 
![[Pasted image 20250623103956.png]]