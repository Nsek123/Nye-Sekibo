Sur la page /survey, chaque sujet possède un bouton qui envoie automatiquement une note en POST grâce à this.form.submit().
Le formulaire transmet simplement deux champs : sujet (ID) et valeur (note).
Comme aucune vérification n’est faite, j’ai rejoué la requête avec curl en mettant une note impossible, 9999.
Le serveur l’a acceptée et a renvoyé le flag.

flag: 03a944b434d5baff05f46c4bed5e5792551a2595574bcafc9a6e25f67c382ccaa
<img width="569" height="830" alt="Image" src="https://github.com/user-attachments/assets/d6215bd8-c055-4e78-b53c-bce7e6e44361" />
