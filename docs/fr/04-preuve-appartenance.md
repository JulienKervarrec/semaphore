# 4. Prouver l’appartenance sans révéler le membre

Pour produire une preuve, l’utilisateur fournit localement son identité, le groupe visé, la racine de Merkle et le message à autoriser. Le package proof assemble ces données et les transmet au circuit, sans envoyer le secret au vérificateur.

La preuve démontre que le commitment contrôlé par l’utilisateur se trouve bien dans l’arbre correspondant à la racine annoncée. Elle démontre aussi que le prouveur connaît le secret associé, sans révéler ce secret ni la position exacte du membre dans l’arbre.

Le message fait partie du contexte cryptographique. Une preuve générée pour un message ne doit donc pas être traitée comme une autorisation générale : modifier le message modifie le domaine de la preuve.

Le résultat est vérifiable par une bibliothèque ou par le contrat Semaphore. Cette vérification ne reconstitue pas l’identité ; elle contrôle seulement les contraintes publiques prévues par le circuit.

Suite : [nullifier et prévention du double usage](05-nullifier-et-double-usage.md).
