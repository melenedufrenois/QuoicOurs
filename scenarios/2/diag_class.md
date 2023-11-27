```mermaid
classDiagram
    class Utilisateur {
      +String nom: "Marie"
      +String email: "marie@email.com"
    }
    class SiteWeb {
      +authentifier()
    }
    class Compte {
      +String identifiant: "marie123"
    }

    Utilisateur --> SiteWeb : interagit
    SiteWeb --> Compte : crée
