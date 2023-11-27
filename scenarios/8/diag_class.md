classDiagram
    class Utilisateur {
      +String nom: "Emma"
      +String email: "emma@email.com"
    }
    class SiteWeb {
      +afficherHistorique()
    }
    class HistoriqueLecture {
      +List oeuvresLues: ["Les Misérables", "1984"]
    }

    Utilisateur --> SiteWeb : consulte
    SiteWeb --> HistoriqueLecture : affiche
