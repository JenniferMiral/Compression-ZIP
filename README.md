Si ça marche, on va pouvoir faire quelque chose

Coder les images.
Parmi les contenus multimédias, comment les images sont-elles codées dans un ordi ?

Rappels : En parlant de création et de manipulation d'images numériques on fait appel à un domaine particulier de l'informatique = l'infographie.
En termes de communication entre les différents constituants d'un ordi, le processeur envoie les infos qui définissent l'image, de la mémoire vive vers la carte graphique qui convertir les données pour les afficher à l'écran.
Différence entre images numériques et images analogiques : les premières peuvent être décrites par un ensemble fini de valeurs entières = "code génétique" de l'image alors que les deuxièmes sont liées à un support matériel.
Si on prend exemple d'une photographie noir et blanc : un point donné sur une photographie argentique peut prendre n'importe quelle nuance entre le noir et le blanc, sa valeur est continue. Alors que dans une image numérique, un point ne peut prendre d'un nombre fini de valeurs entre le noir et le blanc. Ces valeurs = niveaux de gris.
=> Avantage indéniable des images numériques car possibilité de créer de nombreuses répliques identiques (sans dégradation) et facilité de transmission et de stockage TOUTEFOIS  l'apparence finale dépend beaucoup des logiciels et matériels utilisés (écrans, imprimantes) qui vont interpréter le code de l'image : code identique mais rendus différents.

Il existe deux catégories de codage d'images différenciées par le fait que l'image vectorielle accepte les "étirements" alors que l'image matricielle subie une dégradation => respectivement codage vectoriel (JPEG) avec un ensemble de formules mathématiques et codage Bitmap ou matriciel (RLE, LZW) comme un tableau de points. Cette opération (passage entre image continue à grille de pixels est appelée échantillonage.

Quels sont alors les paramètres pour définir une image matricielle ?
- le nombre de colonnes
- le nombre de lignes
la multiplication des deux constituant la définition d'une image
- le nombre de couleurs / pixel

Ainsi, à un pixel associé à une case du tableau correspond une valeur.

Selon le nombre de couleurs autorisées, la valeur est stockée sur un certain nombre de bits ; on a donc plusieurs formats :
- bitmap noir et blanc : 0 ou 1 = image binaire CF. TABLEAU
- bitmap 16 couleurs : 2⁴ possibilités
- bitmap 256 couleurs : 2⁸ possibilités
- True Color : RVB soit 2²⁴ possibilités soit plus de 16 millions de possibilités

Le choix du nombre de niveaux de gris ou de couleurs a des conséquences sur la qualité de l'image même si généralement 256. On peut aller au-delà ppour plus de précisions mais :

Taille en octets d'une image bitmap = Nbr de colonnes * Nbr de lignes * Nbr de bits par pixel / 8
Plus la résolution baisse, plus le nombre de pixels dans l'image diminue et plus la qualité de l'image se dégrade.
=> Important pour des question de stockage et de durée de chargement sur une page Web. => Pour choisir bonne résolution, bien identifier utilisation de l'image.

Le codage Bitmap "carte de bits" = description point par point ou pixel par pixel = façon la plus simple de coder une image MAIS pixels peuvent être petits et nombreux et donc une image bitmap est lourde.

=> Necessité de compression.

Pour diminuer l'impact de ces problèmes, compression des images :
- Compression RLE (Run Length Encoding) : images .bmp ; vise à repérer séquences comportants des répétitions d'un même élément (à partir de 3) ; images avec larges parties uniformes.
- Compression LZW (Lempel-Ziv-Welch) : .gif et .tiff ; repérer séquences mais en parallèle construction d'un dictionnaire qui attribue indice ; idem et images géométriques.
- Compression JPEG (Joint Photographic Expert Group) : .jpg ; atténuer les détails en éliminant certaines composantes de haute fréquence grâce à formules mathématiques complexes ; perte d'informations...


