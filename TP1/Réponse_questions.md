## Suite des questions
#### Liam Boudadi & Chloé Varin

### 4. Donnez la forme de la matrice Q s'il fallait appliquer le Q-Learning à l'environnement MoutainCar.

Pour appliquer un algorithme de Q learning sur le problème de la mountain on doit définir les états possibles. On a 2 observations :

- La position de la voiture, généralement entre $-1.2$ et $0.6$
- La vitesse de la voiture entre $-0.7$ et $0.7$
  On peut diviser ces deux intervalles pa exemple en 20 groupes de valeurs chacun ce qui nous donne 20x20, 400 états possibles

Peu importe l'état, la voiture ne peut effectuer q'une des 3 actions suivantes : accélerer à gauche, ne pas accélérer, accélerer à droite.

Une Q-table pour le problème de la moutain car pourrait avoir 400 lignes pour les états possibles avec chacune 3 colonnes pour les actions possibles.

### Expliquez ce qu'est le Deep Q-Learning.

Le Deep Q-learning est une variante du Q-Learning qui va associer l'algorithme à un réseau de neurones l'intérêt étant de s'attaquer à des espaces d'états de plus grande taille où le réseau de neurone va approximer la valeur de la Q-function. Le réseau va être mis à jour avec des combinaisons d'itérations et de stratégies d'exploration.

### 5. Les algorithmes de type QLearning tâtonnent, les algorithmes de types A* sont guidés vers l'objectif par une heuristique. Pourquoi et quand est-il plus intéressant d'utiliser le Q-Learning ?

L'algorithme de Q-learning est un algorithme de renforcement, il est plus utilisé lorsqu'on ne connait pas la structure de l'environnement car il va explorer activement pour découvrir les informations. Il est efficace dans les problèmes ou des séquences d'actions doivent être prise, sachant que chaque action à des conséquences sur l'avenir, c'est le cas des problèmes de contrôle comme le FrozenLake ou le Mountain Cart étudis précedemment dans ce TP. Quant à l'algorithme A*, c'est un algorithme de recherche qui peut être appliqué dans les tous les espaces qui peuvent être représentés sous forme de graphe où les noeuds sont des positions et les arêtes ont un coût. Il est intéressant de l'utiliser dans les problèmes de recherche de chemin dans les environnements satiques, ou bien dans les environnements déterministes où chaque action a un résultat prévisible et fixe.

### 6. Citez des exemples réels d'applications industrielles, commerciales du Q-Learning
L'intelligence artificielle étant de plus en plus utilisée dans les industries, on trouve facilement des exemple d'entreprises qui utilisent l'algorithme de Q-learning pour différentes applications par exemple: 
- *Ubisoft* utilise l'apprentissage par renforcement pour améliorer l'IA des PNJ dans leurs jeux, rendant les interactions plus réalistes et engageantes
- *Walmart* utilise des techniques d'apprentissage par renforcement pour optimiser les routes de livraison et la gestion des stocks, contribuant ainsi à des économies significatives et à une meilleure satisfaction client.
- *Netflix* utilise des algorithmes d'apprentissage par renforcement pour personnaliser les recommandations de films et séries, améliorant ainsi la satisfaction et la rétention des utilisateurs.