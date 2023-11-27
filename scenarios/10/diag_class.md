```mermaid
classDiagram
    class Utilisateur {
      +String nom: "Hugo"
      +String email: "hugo@email.com"
    }
    class SiteWeb {
      +ajouterAuxFavoris()
    }
    class Favoris {
      +List oeuvresFavorites: ["Les Misérables"]
    }
    class Oeuvre {
      +String titre: "Le Comte de Monte-Cristo"
    }

    Utilisateur --> SiteWeb : sélectionne œuvre
    SiteWeb --> Oeuvre : ajoute aux favoris
    Oeuvre --> Favoris : est ajoutée
