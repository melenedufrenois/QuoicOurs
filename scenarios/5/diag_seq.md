```mermaid
sequenceDiagram
    participant A as Administrateurs
    participant S as Site Web
    A->>S: Se connectent et accèdent à la modération
    S->>A: Affiche les propositions en attente
    A->>S: Examinent et décident sur chaque proposition
