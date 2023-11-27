classDiagram
class Utilisateur {
+String nom: "Léa"
+String email: "lea@email.com"
}
class SiteWeb {
+mettreAJourProfil()
}
class Compte {
+String identifiant: "lea789"
}

    Utilisateur --> SiteWeb : modifie le profil
    SiteWeb --> Compte : enregistre les changements
