# 2. Identité et secret utilisateur

Une identité Semaphore ne se résume pas à une adresse Ethereum. La bibliothèque identity construit une paire de valeurs à partir d’un secret conservé par l’utilisateur. Ce secret constitue la donnée sensible : il ne doit pas être publié ni envoyé au vérificateur.

Le protocole dérive de cette identité un commitment, c’est-à-dire une représentation publique qui peut être insérée dans un groupe. Le commitment permet de reconnaître l’appartenance cryptographique sans permettre de retrouver le secret à partir de la valeur publiée.

Cette séparation donne deux propriétés importantes. Le même utilisateur peut prouver son appartenance à plusieurs groupes, tandis que chaque groupe ne voit qu’un membre représenté par son commitment. La perte ou la réutilisation du secret reste toutefois une responsabilité critique du portefeuille ou de l’application.

Les types et fonctions de la bibliothèque doivent donc être lus avec une frontière claire : identité et secret côté utilisateur, commitment côté registre de groupe, preuve côté circuit.

Suite : [groupes et arbre de Merkle](03-groupes-et-arbre.md).
