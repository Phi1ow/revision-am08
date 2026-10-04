# Révision AM08 · Fluides en mouvement

Outil de révision interactif pour AM08 (mécanique des fluides incompressibles) : hydrostatique, efforts sur les parois et Archimède, Bernoulli (Torricelli, Venturi, Pitot, pompes et turbines), pertes de charge, formulaire, et entraînement sur les 19 exercices du TD et les médians A22 à A25 avec corrections.

Ouvrir `index.html` dans un navigateur, ou utiliser la version en ligne (GitHub Pages) : <https://phi1ow.github.io/revision-am08/>. Le pendant AM11 (éléments finis) est ici : <https://phi1ow.github.io/revision/>.

## Ce que la page sait faire

- **Labos animés** : chaque idée du cours (loi hydrostatique, tube en U, parois planes et courbes, Archimède, Euler, budget de pression, Torricelli, Venturi, Pitot, pompes, pertes de charge) a une animation dont tu changes les paramètres. Les calculs retrouvent les valeurs des diapos.
- **Entraînement** : les 19 fiches du TD et les médians A22, A23, A24 et A25, avec figure et correction à dévoiler question par question. Chaque correction est détaillée pas à pas (hypothèses, points choisis, équations justifiées, expression littérale encadrée, application numérique, commentaire et piège) et accompagnée d'un schéma animé qui suit le raisonnement : ligne de courant, bilan de charge en barres, chemin dans le manomètre, forces et équilibre, courbes… Le schéma suit aussi la question dans les cartes mémoire.
- **Progression** : sous chaque correction, marque la question *Acquis* ou *À revoir*. Le panneau en tête de la partie F montre la barre d'avancement, filtre ce qui reste, et retrouve le dernier exercice travaillé.
- **Cartes mémoire** (fin du formulaire) : formules, pièges, gestes de la méthode, les quatre pressions et les ordres de grandeur deviennent des cartes à répétition espacée (4 boîtes : une carte ratée revient tout de suite, une carte sue revient dans 1, 3 puis 7 jours). Le paquet *Exercices* ajoute toutes les questions des TD et médians. Au dos de chaque carte de formule, de piège ou de méthode, un schéma animé montre l'idée (budget de pression qui s'échange le long d'une ligne de courant, centre de poussée qui glisse sous G, ligne de charge, cavitation…) ; une carte d'exercice affiche la figure et le rappel de l'énoncé. Un petit schéma animé explique le passage d'une boîte à l'autre.
- **Chrono d'examen** (icône ⏱ dans la barre) : médian de 1 h 30, ou une durée au choix ; le temps restant s'affiche dans la barre et dans l'onglet, la page sonne à la fin, et le chrono survit à un rechargement.
- **Recherche** (loupe, `/` ou `Ctrl+K`) : chapitres, labos, formules, pièges, exercices et questions ; la cible s'ouvre et se surligne.
- **Thème** clair / sombre (icône lune / soleil, ou touche `t`), mémorisé.
- **Impression** : le bouton *Imprimer le formulaire* sort formules et pièges seuls sur une à deux pages A4, le brouillon de la page recto manuscrite autorisée au médian ; `Ctrl+P` imprime toute la page avec les corrections dépliées.
- **Liens profonds** : chaque question a une ancre (`#ex-td9-q2` par exemple), utile pour retrouver un point précis.

## Raccourcis clavier

| Touche | Action |
| --- | --- |
| `/` ou `Ctrl+K` | Rechercher |
| `t` | Changer de thème |
| `Espace` | Retourner la carte affichée |
| `→` / `←` | Carte sue / carte à revoir |
| `Échap` | Fermer la fenêtre ouverte |

## Données

Progression, cartes, thème et chrono sont enregistrés dans le `localStorage` du navigateur (clés préfixées `am08:`). Rien ne quitte ta machine ; un autre navigateur ou une fenêtre privée repart de zéro. Les boutons *Réinitialiser* du panneau de progression et des cartes effacent ces données.

## Structure

Un seul fichier, `index.html` : styles, contenu, solveurs et animations. Le « kit de révision » (progression, cartes, chrono, recherche, impression) est un bloc CSS et un script indépendants ajoutés à la fin du fichier ; il lit la page telle qu'elle est, donc ajouter un exercice ou un piège suffit pour qu'il apparaisse dans la recherche, la progression et les cartes.
