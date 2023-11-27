classDiagram
    class InterfaceUtilisateur {
      +Page Historique Lecture
    }
    class ServeurWeb {
      +API Historique Lecture
    }
    class BaseDeDonnees {
      +HistoriqueLectures
    }
    class HistoriqueLecture {
      +List oeuvresLues
    }

    InterfaceUtilisateur --> ServeurWeb : demande historique lecture
    ServeurWeb --> BaseDeDonnees : récupère historique
    BaseDeDonnees --> HistoriqueLecture : renvoie historique
