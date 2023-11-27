classDiagram
    class InterfaceUtilisateur {
      +Page Recherche Location
      +Détails Location
    }
    class ServeurWeb {
      +API Location Oeuvre
    }
    class BaseDeDonnees {
      +Oeuvres
      +Locations
    }
    class Oeuvre {
      +String titre
      +String auteur
    }
    class Location {
      +Date dateLocation
      +Date dateFin
    }

    InterfaceUtilisateur --> ServeurWeb : demande location oeuvre
    ServeurWeb --> BaseDeDonnees : enregistre location
    BaseDeDonnees --> Oeuvre : renvoie informations
    BaseDeDonnees --> Location : crée enregistrement de location
