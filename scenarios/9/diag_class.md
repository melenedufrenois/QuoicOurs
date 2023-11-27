```mermaid
classDiagram
    class Utilisateur {
      +String nom: "Alex"
      +String email: "alex@email.com"
    }
    class SiteWeb {
      +redirigerVersOeuvre()
    }
    class Oeuvre {
      +String titre: "Le Petit Prince"
    }

    Utilisateur --> SiteWeb : accède à l'historique
    SiteWeb --> Oeuvre : redirige

```
