sequenceDiagram
    participant U as Utilisateur
    participant S as Site Web
    U->>S: Accède à la page de connexion
    U->>S: Saisit email et mot de passe
    S->>S: Vérifie les informations
    S->>U: Authentifie et redirige vers le compte
