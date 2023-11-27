```mermaid
sequenceDiagram
    participant U as Utilisateur
    participant S as Site Web
    U->>S: Accède à la page d'inscription
    U->>S: Remplit et soumet le formulaire
    S->>S: Vérifie les informations
    S->>U: Crée le compte et envoie confirmation
