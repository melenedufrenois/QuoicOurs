```mermaid
sequenceDiagram
    participant M as Membre
    participant S as Site Web
    M->>S: Recherche une œuvre
    M->>S: Sélectionne l'œuvre
    S->>S: Vérifie la disponibilité
    S->>M: Enregistre la demande d'emprunt
