Sur la page: /index.php?page=searchimg

on peut faire une injection SQL pour extraire une donnée cachée.
On liste d’abord les tables avec une requête sur information_schema.tables, puis on récupère les commentaires de list_images.

On y trouve un hash MD5 : 1928e8083cf461a51303633093573c46

Ce hash correspond à albatroz.
Il suffit ensuite de générer le SHA-256 de “albatroz” en minuscules pour obtenir le flag.

flag: f2a29020ef3132e01dd61df97fd33ec8d7fcd1388cc9601e7db691d17d4d6188

<img width="712" height="459" alt="Image" src="https://github.com/user-attachments/assets/6e6eb797-ec36-4f15-bd1c-66ddf1a9674f" />
<img width="1222" height="264" alt="Image" src="https://github.com/user-attachments/assets/04fc7e2e-b385-45d9-9a13-4c698618e77f" />
