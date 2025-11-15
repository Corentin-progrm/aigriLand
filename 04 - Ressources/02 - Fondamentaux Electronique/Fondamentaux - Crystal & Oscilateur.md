**Difference entre les deux**
Un oscillateur à cristal est un circuit électronique qui utilise un cristal de quartz pour générer une fréquence précise et stable, tandis qu'un cristal n'est que le composant de cristal de quartz lui-même, nécessitant un circuit oscillateur externe pour fonctionner.

on va dire au'on prefere large les crystale car tu as rien a rajuter en plus

**Crysltal**
A regarder :
- Frequence
- y'en a d'autre mais je me souvients plus

Les caracteristiaue du crystale depende de ce aue demande la chip dans la data sheet, ensuite il faut calculer les condo dont a besoin le crystale

https://blog.adafruit.com/2012/01/24/choosing-the-right-crystal-and-caps-for-your-design/

pour calculer on eut utiliser le logicile saturn pcb design
dans PPM-XTAL calculator 
- load capacitance, c'est celui du crystal
- stry capacitance c'est la capaticter de ta trace donc on peut mettre environs 3pf
- C1/C2 value c'est la valur des condo aue tu doit mettre
- based on C1/C2 c'est ce quer t uqs grqce au condo aue tu as mis
qund tu fait solve tu doit faire en sorte que la load capacitence soit egal a la based on C1/C2 donc change la valeur des condo aui doivent etre identiaue pour avoirt le bon resutlat

![[Pasted image 20250728140938.png]]