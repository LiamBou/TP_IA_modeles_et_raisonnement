### 4. Donnez la forme de la matrice Q s'il fallait appliquer le Q-Learning à l'environnement MoutainCar.

Pour appliquer un algorithme de Q learning sur le problème de la mountain on doit définir les états possibles. On a 2 observations :

- La position de la voiture, généralement entre $-1.2$ et $0.6$
- La vitesse de la voiture entre $-0.7$ et $0.7$
  On peut diviser ces deux intervalles pa exemple en 20 groupes de valeurs chacun ce qui nous donne 20x20, 400 états possibles

Peu importe l'état, la voiture ne peut effectuer q'une des 3 actions suivantes : accélerer à gauche, ne pas accélérer, accélerer à droite.

Une Q-table pour le problème de la moutain car pourrait avoir 400 lignes pour les états possibles avec chacune 3 colonnes pour les actions possibles.

### Expliquez ce qu'est le Deep Q-Learning.

Le Deep Q-learning est une variante du Q-Learning qui va associer l'algorithme à un réseau de neurones l'intérêt étant de s'attaquer à des espaces d'états de plus grande taille où le réseau de neurone va approximer la valeur de la Q-function. Le réseau va être mis à jour avec des combinaisons d'itérations et de stratégies d'exploration.
