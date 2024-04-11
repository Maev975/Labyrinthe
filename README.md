EVA Maxence
HERGOTT Aymeric
S2E

Un descriptif expliquant comment lancer votre application :

Pour lancer notre jeu, il vous suffit de vous rendre dans un terminal, éventuellement compiler tous les fichiers si ce n'est pas déjà fait, lancer le main avec la commande "java mainLaby". Un jeu se lancera. Dans ce jeu, vous devez taper une action qui permettra au personnage de se déplacer (vous pouvez soit entrer gauche, droit, haut ou bas). Vous pouvez aussi taper "exit" pour sortir du jeu. Si l'action n'est pas possible, le personnage ne bougera pas et le terminal vous demandera d'entrer une nouvelle commande ou action. S'il n'est pas arrêté manuellement par l'utilisateur, le jeu continue jusqu'à ce que le personnage atteigne la sortie.

Un résumé des résultats de vos tests (ce qui réussit / échoue éventuellement) :

Tous les tests fonctionnent (testGetSuivant, testDeplacerPerso, testGetChat(), testEtreFini() et testChargerLabyrinthe) à l'exception d'un (testToString). Pour tous les tests, la difficulté principale rencontrée était d'appeler un des labyrinthes créés précédemment, mais ce problème a vite été résolu à l'aide du cours et de nos recherches. Pour le test "testToString", nous ne comprenons pas l'erreur, elle est sans doute due à une faute dans le document txt puisque avec un "System.out.println" on observe que le labyrinthe obtenu est exactement le même que le labyrinthe attendu :
Labyrinthe obtenu :
XXXXXXXXXX
X.....XX.X
X.XS.....X
X......X.X
X........X
X..XXP...X
XXXXXXXXXX

Labyrinthe attendu :
XXXXXXXXXX
X.....XX.X
X.XS.....X
X......X.X
X........X
X..XXP...X
XXXXXXXXXX"
Nous supposons aussi que le problème pourrait être lié aux "\n" que nous avons utilisés pour revenir à la ligne, qui sont présents dans le test mais pas dans le fichier .txt.
