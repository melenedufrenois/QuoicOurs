classDiagram
    class Utilisateur {
      +String nom: "Clara"
      +String email: "clara@email.com"
    }
    class SiteWeb {
      +afficherConditionsLocation()
      +confirmerLocation()
    }
    class Oeuvre {
      +String titre: "1984"
      +String auteur: "George Orwell"
    }

    Utilisateur --> SiteWeb : demande location
    SiteWeb --> Oeuvre : traite demande
