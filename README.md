# Mixt3nUm
Trier trois  nombres sans conditions 
Dans cet exercice, il fallait penser un peu plus à la solution car il était interdit d'utiliser les structures conditionnelles.

Pour résoudre ce problème, nous commençons par trouver le nombre le plus petit et le nombre le plus grand entre les trois variables a, b et c grâce aux fonctions min et max.

Cela nous donne donc la variable a1 et la variable a3 :

    a1 = min(a, b, c)
    a3 = max(a, b, c)

Puisque nous ne pouvons pas savoir d'avance quelles variables parmi a, b et c vont correspondre à la valeur la plus petite et la valeur la plus grande, il nous faut faire un peu d'arithmétique pour trouver la valeur du milieu.

Pour se faire, nous additionnons les trois valeurs ensemble (a, b et c) puis nous soustrayons les deux variables précédemment trouvées avec la fonction min et max :

    a2 = (a + b + c) - a1 - a3
