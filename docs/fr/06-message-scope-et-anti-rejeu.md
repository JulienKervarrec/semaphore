# 6. Message, scope et anti-rejeu

Semaphore ne prouve pas seulement qu’un membre existe : il lie la preuve à un message et à un scope. Le message porte l’action autorisée, tandis que le scope identifie le contexte dans lequel cette autorisation peut être consommée.

Cette liaison empêche qu’une preuve créée pour un vote soit réutilisée pour une autre action ou qu’une preuve destinée à une application soit acceptée par une application voisine. Le contrat doit transmettre exactement les mêmes valeurs au vérificateur que celles utilisées lors de la génération.

Le scope peut représenter un scrutin, une campagne, un groupe logique ou une instance applicative. Il doit être stable pendant la durée de l’action, suffisamment spécifique pour éviter les collisions et conçu avec soin pour ne pas créer de corrélations inutiles.

Le contrôle cryptographique et la mémoire des nullifiers forment ensemble la défense contre le rejeu. Oublier l’un des deux réduit la sécurité du parcours.

Suite : [vérification dans les contrats](07-verification-solidity.md).
