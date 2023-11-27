classDiagram
    class Utilisateur {
      +String nom: "Jean"
      +String email: "jean@email.com"
    }
    class SiteWeb {
      +rechercher()
      +afficherDetails()
    }
    class Oeuvre {
      +String titre: "Les Misérables"
      +String auteur: "Victor Hugo"
    }

    Utilisateur --> SiteWeb : utilise
    SiteWeb --> Oeuvre : affiche
