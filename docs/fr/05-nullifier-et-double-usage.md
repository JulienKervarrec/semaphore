# 5. Nullifier et prévention du double usage

La confidentialité ne suffit pas si un membre peut utiliser la même autorisation plusieurs fois. Semaphore ajoute donc un nullifier, une valeur dérivée de l’identité et du scope de l’action.

Le nullifier ne révèle pas l’identité du membre, mais il devient un identifiant public stable pour ce contexte précis. Le vérificateur ou le contrat peut mémoriser les nullifiers déjà consommés et refuser une seconde utilisation.

Le scope est essentiel : une même identité peut agir dans plusieurs groupes, applications ou scrutins sans produire un identifiant globalement corrélable. À l’inverse, un scope mal choisi peut autoriser un rejeu ou créer une corrélation involontaire entre des actions.

La prévention du double usage est donc une propriété applicative autant que cryptographique. Le contrat doit vérifier le nullifier au moment de l’action et l’enregistrer seulement lorsque l’opération est acceptée.

Suite : [message, scope et anti-rejeu](06-message-scope-et-anti-rejeu.md).
