classDiagram
    class Utilisateur {
      +String nom: "Paul"
      +String email: "paul@email.com"
    }
    class SiteWeb {
      +verifierDisponibilite()
      +enregistrerEmprunt()
    }
    class Oeuvre {
      +String titre: "L'Iliade"
      +String auteur: "Homère"
    }

    Utilisateur --> SiteWeb : demande emprunt
    SiteWeb --> Oeuvre : vérifie et enregistre
