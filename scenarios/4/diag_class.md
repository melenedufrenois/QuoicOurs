```mermaid
classDiagram
    class Utilisateur {
      +String nom: "Sophie"
      +String email: "sophie@email.com"
    }
    class SiteWeb {
      +recevoirProposition()
    }
    class Oeuvre {
      +String titre: "Nouveau Roman"
      +String auteur: "Sophie Auteur"
    }

    Utilisateur --> SiteWeb : propose
    SiteWeb --> Oeuvre : enregistre
