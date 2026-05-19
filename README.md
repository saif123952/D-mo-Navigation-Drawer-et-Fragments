# D-mo-Navigation-Drawer-et-FragmentsCompte Rendu TP Android : Interface Multi-Fragments avec Drawer Menu

📌 Présentation du Travail

Dans ce TP, nous avons réalisé une application Android composée de plusieurs interfaces reliées par un menu coulissant latéral.
L’idée principale était de créer une navigation simple permettant de passer d’un écran à un autre sans ouvrir plusieurs activités.

Le projet a été développé sous Android Studio en utilisant Java et les composants standards d’Android.

⚙️ Fonctionnement Général de l’Application

L’application démarre sur une activité principale contenant :

une barre supérieure (Toolbar) ;
un menu latéral affichable par glissement ;
une zone centrale qui change selon le fragment sélectionné.

Chaque option du menu ouvre un fragment différent.

📂 Composants Réalisés
🔹 Activité Principale

Le fichier MainActivity.java contrôle toute la navigation dans l’application.

Ses rôles principaux :

ouvrir et fermer le Drawer ;
détecter les clics du menu ;
charger le fragment demandé ;
afficher le titre correspondant dans la Toolbar.
🔹 Premier Écran

Le premier fragment sert d’écran d’accueil.
Il contient un texte de bienvenue et un arrière-plan personnalisé.

Couleur utilisée : vert foncé.

🔹 Deuxième Écran

Le second fragment possède une interface différente avec une autre palette graphique.

Couleur utilisée : orange clair.

Ce fragment permet surtout de tester le changement dynamique d’interface.

🔹 Fragment Liste

Le dernier écran affiche une liste simple d’éléments statiques.

Exemples affichés :

Android
Java
XML
Fragment
Navigation Drawer

L’affichage a été réalisé avec ListFragment.

🧩 Organisation XML

Le layout principal utilise :

DrawerLayout
NavigationView
FrameLayout

Le FrameLayout joue le rôle de conteneur principal pour les fragments.

🖥️ Exemple du Menu XML
<menu xmlns:android="http://schemas.android.com/apk/res/android">

    <item
        android:id="@+id/nav_home"
        android:title="Accueil"
        android:icon="@android:drawable/ic_menu_compass"/>

    <item
        android:id="@+id/nav_second"
        android:title="Interface 2"
        android:icon="@android:drawable/ic_menu_manage"/>

    <item
        android:id="@+id/nav_data"
        android:title="Données"
        android:icon="@android:drawable/ic_menu_sort_by_size"/>

</menu>
🔧 Techniques Utilisées

Pendant la réalisation du projet, plusieurs concepts Android ont été appliqués :

Élément	Utilisation
FragmentManager	Gestion des transitions
NavigationView	Création du menu
Toolbar	Barre supérieure
ListFragment	Affichage de listes
DrawerLayout	Menu coulissant
🎨 Modifications Personnelles Effectuées

Pour personnaliser davantage l’application, plusieurs changements ont été ajoutés :

changement total des noms des fragments ;
nouvelles couleurs et nouveaux thèmes ;
modification des titres du menu ;
ajout d’icônes différentes ;
structure de code réorganisée ;
commentaires simplifiés ;
design plus minimaliste.
📱 Résultat Final

L’application obtenue permet :

✅ une navigation rapide
✅ une interface propre
✅ une bonne séparation des composants
✅ une meilleure compréhension des Fragments Android

📝 Conclusion

Ce TP nous a aidés à maîtriser la navigation avec les fragments et la création d’interfaces dynamiques dans Android.
Nous avons également appris à organiser un projet Android de manière plus professionnelle tout en améliorant l’expérience utilisateur grâce au menu latéral.
