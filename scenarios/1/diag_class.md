```mermaid
classDiagram
    class Utilisateur {
      +String nom: "Jean"
      +String email: "jean@email.com"
      +String motDePasse
      +bool estAuthentifie()
      +void changerMotDePasse(String nouveauMotDePasse)
    }
    class Role {
      +String nom
    }
    class UtilisateurRole {
      +Utilisateur utilisateur
      +Role role
    }
    class SiteWeb {
      +rechercher()
      +afficherDetails()
      +bool verifierAutorisation(Utilisateur utilisateur, String roleRequis)
      +void enregistrerActivite(Utilisateur utilisateur, String activite)
    }
    class Oeuvre {
      +String titre: "Les Misérables"
      +String auteur: "Victor Hugo"
    }

    Utilisateur --> UtilisateurRole : a
    Role --> UtilisateurRole : a
    UtilisateurRole --> Utilisateur : contient
    UtilisateurRole --> Role : contient
    UtilisateurRole --> SiteWeb : utilise
    SiteWeb --> Oeuvre : affiche
```
