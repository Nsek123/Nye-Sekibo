La page :

/index.php?page=media&src=

réinjecte directement le contenu du paramètre src.

En testant l’URL on constate que la valeur passée apparaît telle quelle dans la page. Avec un schéma de type :
data:text/html;base64,BASE64_PAYLOAD

on voit clairement que la page affiche ce qui lui est fourni, ce qui confirme une XSS Reflected : le paramètre src est utilisé sans filtrage pour afficher un fichier ou du contenu.

flag: 928d819fc19405ae09921a2b71227bd9aba106f9d2d37ac412e9e5a750f1506d

<img width="1753" height="875" alt="Image" src="https://github.com/user-attachments/assets/e9f7edf3-2855-4bf5-96c1-3bebcff8f6fd" />
<img width="1176" height="411" alt="Image" src="https://github.com/user-attachments/assets/375c8d0c-c875-435a-8d40-4b2995fc5c8c" />
