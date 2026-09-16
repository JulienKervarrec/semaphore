# 3. Groupes et arbre de Merkle

Un groupe Semaphore est un ensemble de commitments représentant les membres autorisés. La bibliothèque group gère l’ajout, la suppression et la construction de la structure authentifiée utilisée par le circuit.

Les commitments sont placés dans un arbre de Merkle. Sa racine résume l’état du groupe : le vérificateur n’a pas besoin de recevoir toute la liste des membres, seulement la racine et le chemin qui relie le membre prouvé à cette racine.

Chaque modification du groupe peut donc changer la racine. Une preuve doit référencer une racine acceptée par le contrat ou par le destinataire ; une preuve correcte associée à une ancienne racine peut être refusée si le contexte n’est plus valide.

La racine est publique, mais elle ne révèle pas quel membre sera utilisé dans une preuve. La confidentialité vient de la combinaison entre chemin de Merkle et circuit ZK, pas de l’arbre seul.

Suite : [preuve d’appartenance](04-preuve-appartenance.md).
