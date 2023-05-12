# Challenge n°1 : FTP - Authentification
## Sujet 
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(225).png)

## Etape I :
1. Faire du click droite sur le bouton `Démarer le challenge` puis clicker sur `copie le lien de`
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(227).png)
2. Ouvrir un nouvel ongel et coller `l'adresse` puis `entrer` et il téléchargera automatiquement le fichier `wireshark`.
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(228).png)

##  Etape II :
1. Ouvrir le fichier `wireshark` puis chercher le packet contenant le mot de passe dans les differents packet capturer.
2. Lorsqu'on a trouver le `packet`, faire du `click droite` après passer le curseur sur `suivre` enfin sur `Flux TCP` et les données dans le packet affichera.
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(229).png)
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(231).png)

## Etape III :
Il suffit de copier le `mot de passe` trouver sur le packet dans la barre de validation sur rootMe et envoyer.

# Challenge n°2 : TELNET - Authentification
## Sujet 
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(224).png)

## Etape I :
Même étape que les étapes précedantes

## Etape II :
1. Ouvrir le fichier `wireshark` puis chercher le packet contenant le mot de passe dans les differents packet capturer.
2. Lorsqu'on a trouver le `packet`, faire du `click droite` après passer le curseur sur `suivre` enfin sur `Flux TCP` et les données dans le packet affichera.
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(232).png)
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(233).png)

## Etape III :
Il suffit de copier le `mot de passe` trouver sur le packet dans la barre de validation sur rootMe et envoyer.

# Challenge n°3 : ETHERNET - trame
## Sujet
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(223).png)

## Etape I :
De même que l'étape préccedente mais cette fois ci après le collage de l'adresse du lien il n'y aura pas de téléchagement mais il va afficher `des nombres hexadécimales` donc pour trouver les données normalement `confidentielles` contenues dans cette trame il faut les convertir en language humain.  
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(226).png)

## Etape II : Convertion
1. Puisque ce sont des `nombres hexadécimales`, on devrai le convertir en `Texte`. Pour celà on devrai utiliser des sites ou d'autre chose qui pourra le convertir, dans cette sujet j'ai utiliser le site `unit-conversion-info` pour la convertion
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(234).png)
## NB :
Ceci n'est pas encore en texte humaine, c'est encore a `Base64` parcequ'il se termine par des `=`.
2. Il faut decoder pour voir le contenue, pour celà j'ai utiliser le site `base64decode.org`
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(235).png) 

## Etape III :
Il suffit de copier le text décodé sur la barre d'envoie !

# Challenge n°4 : Authentification twiter
## Sujet
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(222).png)

## Etape I :
De même que l'étape I des Challenge préccedente.

## Etape II :
1. Ouvrir le packet télécharger sur `wireshark` puis le suivre pour obtenir les données
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(236).png)
2. Le mot de passe est ecris à `base64` donc il suffit de le décoder:
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(237).png)
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(239).png)

## Etape III :
`copier` le mote de passe obtenue dans rootMe

# Challenge n°5 : Bluetooth - Fichier inconnu
## Sujet
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(221).png)

## Etape
De même que la 1ère étape de chaque Challenges préccedente.

## Etape II :
1. Ouvrir `wireshark` manuellement après avoire télécharger le fichier cacher, puis dans wireshark faire `CTRL + O` pour ouvrir le fichier cacher.
2. Puis dans la barre des options sur wireshark, clicker sur `wireless` après sur `Equipements Bluetooth` et il affichera l'appareil détécter.
3. Pour trouver le mot de passe on nous propose que la reponse est le `hash SHA1` de la concatenation de l'adresse MAC et du nom du téléphone, donc il suffit de convertir ces derniers en `hash SHA1`.
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(240).png)
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(241).png)
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(242).png)
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(243).png)
![](Image/Capture%20d%E2%80%99%C3%A9cran%20(244).png)

## Etape III :
Copier le mot de passe obtenue dans `rootMe`