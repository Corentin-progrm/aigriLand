en gros tu peut faire une ligne SCL SDA et y mettre plein de capteur i2c, et il faut juste aue tout les capteur est une adresse differente

pour mettre une adresse soit utas le choix et tu peut mettre la pin adresse au gnd ou vcc ou sda ou scl ou alors tu peut pas choisir et faut voirtdnas la datasheet quelle adresse a ete donne

si jamais tu a besoin de mettre 2 fois la meme adresse et bien il te faut un multiplexer pour pouvoir avoir 2 ligne de i2c

il faut mettre des pullup en debut de ligne de data et clk moi je met 5k1 car j'en ai souvent dans le coin


