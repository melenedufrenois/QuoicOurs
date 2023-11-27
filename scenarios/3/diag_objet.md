```mermaid
classDiagram
    class InterfaceUtilisateur {
      +Page Connexion
      +Formulaire Connexion
    }
    class ServeurWeb {
      +API Authentification
    }
    class BaseDeDonnees {
      +Utilisateurs
    }
    class Utilisateur {
      +String email
      +String motDePasse
    }

    InterfaceUtilisateur --> ServeurWeb : envoie identifiants
    ServeurWeb --> BaseDeDonnees : vérifie identifiants
    BaseDeDonnees --> Utilisateur : valide connexion
