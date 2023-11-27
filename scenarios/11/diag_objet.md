classDiagram
class InterfaceUtilisateur {
+Page Profil
+Formulaire Mise à Jour Profil
}
class ServeurWeb {
+API Mise à Jour Profil
}
class BaseDeDonnees {
+Utilisateurs
}
class Utilisateur {
+String nom
+String email
+String motDePasse
}

    InterfaceUtilisateur --> ServeurWeb : soumet mise à jour profil
    ServeurWeb --> BaseDeDonnees : met à jour informations utilisateur
    BaseDeDonnees --> Utilisateur : stocke nouvelles informations
