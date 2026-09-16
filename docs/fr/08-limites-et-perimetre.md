# 8. Limites et périmètre

Semaphore fournit une primitive de preuve d’appartenance privée ; il ne transforme pas automatiquement une application en système anonyme complet. Les métadonnées réseau, les horaires, les adresses de relais et le contenu des messages peuvent encore révéler des informations.

La sécurité dépend aussi du choix du hash, du circuit, des clés de vérification, de la gestion des racines et de la conservation du secret utilisateur. Une mauvaise intégration peut réintroduire rejeu, corrélation ou divulgation malgré une preuve mathématiquement valide.

Ce parcours couvre l’identité, les groupes, l’arbre de Merkle, les preuves, les nullifiers, le scope et la vérification Solidity. Il ne remplace ni un audit cryptographique, ni une revue de contrat, ni une validation des paramètres de production.

Le dépôt contient une suite de tests pour les bibliothèques et les contrats, ainsi que les scripts de compilation et de documentation. Ils constituent la suite naturelle pour vérifier le comportement, mais aucune installation, compilation ou exécution n’a été réalisée dans ce parcours documentaire.

Retour : [vue d’ensemble](01-vue-ensemble.md).
