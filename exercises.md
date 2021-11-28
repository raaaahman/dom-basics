# Javascript - l'API du DOM

## Exercice 1

### Le thème sombre (1ère partie)

Vous souhaitez donner la possibilité aux visiteurs de votre blog personnel d'opter pour un thème sombre au lieu d'un thème clair (un peu comme sur un éditeur de texte). Pour ce faire, vous devez trouver comment changer en javascript les propriétés suivantes:

1. Changer la couleur du fond d'écran pour du noir et le texte pour du blanc (Utiliser la cascade CSS).
2. Changer l'image de fond du `#site-header` pour `code-dark.jpg` (dans le dossier `img`).
3. Changer également les crédits photographiques du `footer` pour l'URL `https://unsplash.com/@baciutudor?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText` et le nom *Tudor Baciu* (Vous pouvez créer des constantes ou des variables pour vous aider).
4. Changer la couleur de fond des champs du formulaire, par exemple en utilisant la couleur `darkgrey` ou la classe `bg-dark` de Bootstrap (vous pouvez créer une boucle, ou changer les éléments un par un).
5. Changer la couleur des liens pour une plus claire, par exemple la couleur `lightblue`, ou la classe `link-info` de Bootstrap (vous aurez besoin d'une boucle).

### Bonus: Changer le thème pour les exemples de code

Le blog utilise la bibliothèque *Prism.js* pour afficher une coloration syntaxique sur ces exemples de code. Ces couleurs proviennent de la feuille de style `https://cdnjs.cloudflare.com/ajax/libs/prism/1.25.0/themes/prism.min.css`.

1. Changer la feuille de style pour `https://cdnjs.cloudflare.com/ajax/libs/prism/1.25.0/themes/prism-dark.min.css` (vous aurez besoin d'utiliser un sélecteur d'attribut)
    - Si vous n'arrivez pas à utiliser le sélecteur d'attribut, ajoutez un `id` sur le `link` à la place
2. Créer une fonction permettant de changer la feuille de style pour utiliser n'importe lequel des thèmes suivants (passé en paramètre):
    - https://cdnjs.cloudflare.com/ajax/libs/prism/1.25.0/themes/prism-coy.min.css
    - https://cdnjs.cloudflare.com/ajax/libs/prism/1.25.0/themes/prism-dark.min.css
    - https://cdnjs.cloudflare.com/ajax/libs/prism/1.25.0/themes/prism-funky.min.css
    - https://cdnjs.cloudflare.com/ajax/libs/prism/1.25.0/themes/prism-okaidia.min.css
    - https://cdnjs.cloudflare.com/ajax/libs/prism/1.25.0/themes/prism-solarizedlight.min.css
    - https://cdnjs.cloudflare.com/ajax/libs/prism/1.25.0/themes/prism-tomorrow.min.css
    - https://cdnjs.cloudflare.com/ajax/libs/prism/1.25.0/themes/prism-twilight.min.css

Appeler la fonction dans la console pour tester si elle... fonctionne.

## Exercice 2

### Les commentaires (1ère partie)

On veut que les visteurs puissent ajouter des commentaires sur la page. Vous devez pour cela trouver un myen de les ajouter en javascript.

1. Supprimer le commentaire de M. Callaghan (le dernier).
2. Ajouter un paragraphe au commentaire de Georges Abitbol (le premier).
3. Ajouter un commentaire entier (attention, c'est long).
4. Créer la fonction `addComment` qui permet d'ajouter un commentaire dans la liste, en prenant en paramètre le nom de la personne et son message (et éventuellement une date).

### Bonus: Les commentaires

1. Générer la date grâce à un objet `Date`: [Date, Objets Globaux, Référence Javascript, Mozilla Developers Network](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Date)

## Exercice 3

### Le thème sombre (2ème partie)

1. Changer le thème pour un thème sombre lorsque l'on appuie sur le bouton `#theme-switcher` (réutiliser le code de l'exercice 1).
2. Lorsque l'on clique sur le bouton `#theme-switcher`, si l'on est déjà en thème sombre, on doit retourner en thème clair. Changer aussi le texte du bouton, pour qu'il affiche "Thème Clair" ou "Thème Sombre".
3. Lorsque l'on clique sur le bouton `#like-btn`, on doit augmenter le nombre affiché dans ce bouton.
4. Lorsque l'on envoie le formulaire, le commentaire doit être ajouté à la suite des autres commentaires. Ce commentaire doit utiliser le nom et le message renseigné dans le formulaire. Le formulaire doit être réinitialisé **après** que le commentaire aie été ajouté.

### Bonus

1. Un visiteur peut ajouter autant de "likes" qu'il veut au compteur, arriverez-vous à limiter l'ajout à un seul "like"?
2. Changer le thème des exemples de code en utilisant les valeurs du menu déroulant `#code-theme-switcher` (il faut trouver un nouvel événement).
3. On veut pouvoir afficher la progression de la lecture de l'article dans l'élément `progress`, pouvez-vous remplir cette barre au fur et à mesure que l'utilisateur fait défiler la page? (nouvel événement, il va aussi falloir utiliser des propriétés de l'objet [window](https://developer.mozilla.org/fr/docs/Web/API/Window)).
4. Ajouter un bouton permettant de modifier un commentaire déjà publié.