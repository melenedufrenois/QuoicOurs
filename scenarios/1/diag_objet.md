classDiagram
    class InterfaceUtilisateur {
      +Page d'Accueil
      +Page de Recherche
      +Page de Détails
    }
    class ServeurWeb {
      +API de Recherche
      +API de Détails
    }
    class BaseDeDonnees {
      +Oeuvres
    }
    class Oeuvre {
      +String titre: "Les Misérables"
      +String auteur: "Victor Hugo"
    }

    InterfaceUtilisateur --> ServeurWeb : requêtes API
    ServeurWeb --> BaseDeDonnees : requêtes SQL
    BaseDeDonnees --> Oeuvre : renvoie données
    Oeuvre --> InterfaceUtilisateur : affiche informations