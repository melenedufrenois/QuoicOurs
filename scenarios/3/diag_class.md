classDiagram
    class Utilisateur {
      +String nom: "Luc"
      +String email: "luc@email.com"
    }
    class SiteWeb {
      +authentifier()
    }
    class Compte {
      +String identifiant: "luc456"
    }

    Utilisateur --> SiteWeb : se connecte
    SiteWeb --> Compte : authentifie
