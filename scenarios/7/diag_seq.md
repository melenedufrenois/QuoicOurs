```mermaid
sequenceDiagram
    participant M as Membre
    participant S as Site Web
    M->>S: Recherche une œuvre à louer
    M->>S: Sélectionne et voit les conditions
    M->>S: Accepte et paie la location
    S->>M: Confirme la location
