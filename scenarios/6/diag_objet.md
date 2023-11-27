```mermaid
classDiagram
    class InterfaceUtilisateur {
      +Page Recherche Oeuvre
      +Détails Oeuvre
    }
    class ServeurWeb {
      +API Emprunt Oeuvre
    }
    class BaseDeDonnees {
      +Oeuvres
      +Emprunts
    }
    class Oeuvre {
      +String titre
      +String auteur
    }
    class Emprunt {
      +Date dateEmprunt
      +Date dateRetour
    }

    InterfaceUtilisateur --> ServeurWeb : sélectionne oeuvre pour emprunt
    ServeurWeb --> BaseDeDonnees : vérifie disponibilité et enregistre emprunt
    BaseDeDonnees --> Oeuvre : renvoie détails oeuvre
    BaseDeDonnees --> Emprunt : crée enregistrement d'emprunt
