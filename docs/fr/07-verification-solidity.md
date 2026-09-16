# 7. Vérification dans les contrats Solidity

Le package contracts expose Semaphore sous forme de contrats Solidity. Leur rôle est de relier une racine de groupe, un message, un scope et un nullifier à un vérificateur de preuve.

Le contrat ne connaît pas le secret de l’utilisateur. Il reçoit une preuve et les valeurs publiques nécessaires, puis délègue le contrôle cryptographique au vérificateur associé au circuit.

Après validation, il doit contrôler le contexte métier : racine acceptée, nullifier non consommé et paramètres cohérents avec l’action. La preuve ZK établit une relation mathématique ; elle ne décide pas seule de la politique applicative.

Les interfaces ISemaphore, ISemaphoreGroups et ISemaphoreVerifier rendent ces frontières explicites. Une intégration sérieuse doit suivre les événements et les erreurs du contrat plutôt que supposer qu’une preuve valide suffit à autoriser n’importe quelle opération.

Suite : [limites et périmètre](08-limites-et-perimetre.md).
