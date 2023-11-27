classDiagram
    class InterfaceAdministrateur {
      +Page Modération
      +Liste Propositions
    }
    class ServeurWeb {
      +API Gestion Propositions
    }
    class BaseDeDonnees {
      +Propositions Oeuvres
    }
    class Oeuvre {
      +String titre
      +String auteur
    }

    InterfaceAdministrateur --> ServeurWeb : demande propositions
    ServeurWeb --> BaseDeDonnees : récupère propositions
    BaseDeDonnees --> Oeuvre : envoie informations
