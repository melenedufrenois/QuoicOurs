```mermaid
classDiagram
    class InterfaceUtilisateur {
      +Page Inscription
      +Formulaire Inscription
    }
    class ServeurWeb {
      +API Création Compte
    }
    class BaseDeDonnees {
      +Utilisateurs
    }
    class Utilisateur {
      +String nom
      +String email
      +String motDePasse
    }

    InterfaceUtilisateur --> ServeurWeb : envoie données inscription
    ServeurWeb --> BaseDeDonnees : crée utilisateur
    BaseDeDonnees --> Utilisateur : stocke informations
