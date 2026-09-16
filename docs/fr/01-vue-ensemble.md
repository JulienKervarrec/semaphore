# 1. Semaphore, une couche de confidentialité

Semaphore permet de prouver qu’un utilisateur appartient à un groupe sans révéler quelle identité du groupe il contrôle. Le protocole s’appuie sur des preuves à divulgation nulle de connaissance et peut transmettre un message hors chaîne ou à un contrat compatible EVM.

L’identité réelle n’est donc pas publiée dans le message. Le vérificateur reçoit seulement les éléments nécessaires pour contrôler trois propriétés : l’appartenance au groupe, l’autorisation du message et l’absence de réutilisation de la même preuve.

Le dépôt organise cette chaîne en plusieurs briques : circuits ZK, contrats Solidity et bibliothèques TypeScript. Les packages identity, group et proof décrivent respectivement l’identité, l’arbre de membres et la génération ou vérification des preuves.

Le parcours suivra ces briques dans cet ordre. Il s’agit d’une lecture du code et de la documentation du dépôt ; aucune installation, compilation ni exécution de test n’est réalisée.

Suite : [identité et secret utilisateur](02-identite-et-secret.md).
