En accédant à l'URL

on remarque que le formulaire Login envoie les identifiants via une requête GET, ce qui expose directement les paramètres dans l’URL :
?page=signin&username=ADMIN&password=xxxx&Login=Login#


Ce fonctionnement rend les tests automatisés très faciles.

J’ai donc préparé une wordlist puis un script Python qui envoie des requêtes GET pour tester différentes valeurs.

Après lancement du script, la page réagit en fonction des identifiants testés.

flag: B3A6E43DDF8B4BBB4125E5E7D23040433827759D4DE1C04EA63907479A80A6B2

<img width="336" height="362" alt="Image" src="https://github.com/user-attachments/assets/923e1c22-b667-47ed-9d47-f378ee56ecd8" />
<img width="159" height="148" alt="Image" src="https://github.com/user-attachments/assets/7acbf462-118e-4ae2-a5fb-65a308ab5f03" />
<img width="858" height="278" alt="Image" src="https://github.com/user-attachments/assets/10560c20-6da5-4f3d-ba75-e55303063a46" />
<img width="1042" height="168" alt="Image" src="https://github.com/user-attachments/assets/e7751784-b49c-41b2-aa70-29050003170a" />
