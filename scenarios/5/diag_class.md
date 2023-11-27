classDiagram
    class Administrateur {
      +String nom: "Admin"
    }
    class SiteWeb {
      +afficherPropositions()
    }
    class Oeuvre {
      +String titre: "Nouveau Roman"
    }

    Administrateur --> SiteWeb : consulte
    SiteWeb --> Oeuvre : montre
