# Framwork CSS

## Qu'est ce qu'un framwork ?

Les frameworks facilitent le travail du concepteur en fournissant plusieurs services:

-   Simplification des positionnements complexes
-   Amélioration du rendu visuel
-   Gestion de la compatibilité entre les navigateurs.

Comme pour d'autres langages, à partir du moment ou l'on se répète on peut créer un outil (ici le framwork) qui permet d'aller plus vite dans la conception d'une page HTML, le style d'une page, d'un formulaire etc.

## L'interet d'un framwork

Son intéret est simplement de développer plus vite. Que ce soit des sites vitrines, des applications web des jeux etc.
Par exemple, ils incluts quasiment tous un reset CSS qui permet de ne pas avoir le CSS par défaut du navigateur et ainsi de personnaliser nos css à nous.
Vous developpez des styles qui mis bout à bout, ou en groupe permette de créer des composants qui seront réutilisables à l'infini.

## Listes des frameworks CSS

Voici une liste non exhaustives des framewoks CSS

-   [Bootstrap][bootstrap]
-   [TailwindCSS][tailwind]
-   [MaterializeCSS](https://materializecss.com/)
-   [Semantic UI](https://semantic-ui.com/)

[tailwind]: https://tailwindcss.com/
[bootstrap]: https://getbootstrap.com/docs/5.0/getting-started/introduction/

Nous allons nous intéresser sut TailwindCSS.

⚠️ Nous allons voir TailwindCSS mais vous pouvez tester les autres frameworks par curiosité, comme ça, vous pouvez vous faire votre avis et ainsi choisir celui avec lequel vous êtes le plus à l'aise.

## TailwindCSS

Tailwind Css est un framework CSS complètement personnalisable, basé sur le principe de classes utilitaires. Sur le site officiel [ici][tailwind] nous pouvons voir une démo de comment ce construit la page HTML.

## Comment ça fonctionne ?

Avec les frameworks CSS, généralement, tout est une question de classe. On appel ça des 'classe utilitaire'.

Une classe utilitaire est une classe CSS qui a un seul et unique but.
Exemple `.bg-white`. Cette classe a pour but de donner un `background-color: white;` à l’élément.

Prenons un exemple avec [Bootstrap][bootstrap] qui sur le principe fonctionne de la même manière que TailwindCSS mais sur la forme pas du tout !

## Et la sémantique dans tout ça ?

Comme vous avez pu le constater avec vos TP ou vos propre création, la sémantique n'est pas "vraiment" respécté ici. Et oui, on nous demande de faire la page HTML avec les `id` les `class` adéquat et la, quand on regarde la documentation, on ne respect plus réellement cette structure sémantique. Et bien [Adam Wathan](https://adamwathan.me/) à expliqué dans un article que justement, imposer ça (classe css sémantique) été l'un des freins majeurs pour un projet à long terme.

Voici un [site](https://builtwithtailwind.com/) qui enregistre les sites développer avec TailwindCSS

## Exemple entre Bootstrap & Tailwind

Ici, nous avons le code CSS pour générer un bouton avec bootstrap. [ICI](https://codepen.io/gorski_anthony/pen/ExNEqMw)

Et la, la même chose mais pour Tailwind CSS. [ICI](https://codepen.io/gorski_anthony/pen/GRNdKRa?editors=1010)

🤔 Quel est la différence ?

Comme vous l'avez remarqué, sur bootstrap, nous utilisons des classes préfabriqués. `.btn`, `.btn-primary`, etc.

Alors que pour Tailwind, nous avons la possibilitée de personnaliser assez profondement chacun de nos élements car nous ne sommes pas limité aux classes prefabriqué comme bootstrap.

De plus ce lui ci inclut énormément de choses que ne sont la majoritairement pas utilisé.

⚠️ L'avantage de bootstrap.

Pour les gros projets, boiotstrap est un alié car permet à l'ensemble de la team de développeur d'avoir une syntaxe similaire et donc d'avoir les mêmes choses partout, à l'inverse, tailwind est tellement personnalisable que nous devons passer un certain temps à définir la syntaxe à aborder etc.

## La personnalisation

Ok, on a beaucoup parlé de Tailwind, mais ça donne quoi en vrai ?

[Tailwind][tailwind] a mis à disposition un éditeur de code qui permet de tester celui ci directement !

Allons faire un tour et découvrire ce qu'il propose.

## Le background

Voilà la syntaxe pour le changer le background.

`.bg-COULEUR-NUANCE`

⚠️ Il y a des exception evidente pour les couleurs suivante

-   .bg-transparent
-   .bg-current
-   .bg-black
-   .bg-white

Les couleurs citées ci dessus n'ont pas de nuance.

Pour les autres², les nuances vont de

-   50 \> 100 \> 200 \> 300 \> 400 \> 500 \> 600 \> 700 \> 800 \> 900

50 étant la nuance la plus claire et 900 la plus foncée.

Les autres couleurs :

-   gray
-   red
-   yellow
-   green
-   blue
-   indigo
-   purple
-   pink

![color](/images/bg-color.png)

👨‍🎓 TP - Arc en ciel

Créer sur le site de Tailwind, un arc-en-ciel de couleur !
Pour cela, vous allez utiliser la classe background-color de tailwind et ajouter le style suivant `style="height: 20px;"` pour voir le résultat.

ex: ![t1](/images/t1.png)

👨‍🏫 Correction : [ici](https://play.tailwindcss.com/oG0073qRTl)

## Width et Height

Voilà la syntaxe pour modifier la taille.

**width**

`w-VALEUR`

**height**

`h-VALEUR`

Voilà les valeurs disponibles, ici ce sont les valeurs en unité rem:

### Détail des ranges

<details>
 <summary>Cliquez ici</summary>

| Valeur    | Rendu                     |
| --------- | ------------------------- |
| `w/h`-0   | `width/height`: 0px;      |
| `w/h`-0.5 | `width/height`: 0.125rem; |
| `w/h`-1   | `width/height`: 0.25rem;  |
| `w/h`-1.5 | `width/height`: 0.375rem; |
| `w/h`-2   | `width/height`: 0.5rem;   |
| `w/h`-2.5 | `width/height`: 0.625rem; |
| `w/h`-3   | `width/height`: 0.75rem;  |
| `w/h`-3.5 | `width/height`: 0.875rem; |
| `w/h`-4   | `width/height`: 1rem;     |
| `w/h`-5   | `width/height`: 1.25rem;  |
| `w/h`-6   | `width/height`: 1.5rem;   |
| `w/h`-7   | `width/height`: 1.75rem;  |
| `w/h`-8   | `width/height`: 2rem;     |
| `w/h`-9   | `width/height`: 2.25rem;  |
| `w/h`-10  | `width/height`: 2.5rem;   |
| `w/h`-11  | `width/height`: 2.75rem;  |
| `w/h`-12  | `width/height`: 3rem;     |
| `w/h`-14  | `width/height`: 3.5rem;   |
| `w/h`-16  | `width/height`: 4rem;     |
| `w/h`-20  | `width/height`: 5rem;     |
| `w/h`-24  | `width/height`: 6rem;     |
| `w/h`-28  | `width/height`: 7rem;     |
| `w/h`-32  | `width/height`: 8rem;     |
| `w/h`-36  | `width/height`: 9rem;     |
| `w/h`-40  | `width/height`: 10rem;    |
| `w/h`-44  | `width/height`: 11rem;    |
| `w/h`-48  | `width/height`: 12rem;    |
| `w/h`-52  | `width/height`: 13rem;    |
| `w/h`-56  | `width/height`: 14rem;    |
| `w/h`-60  | `width/height`: 15rem;    |
| `w/h`-64  | `width/height`: 16rem;    |
| `w/h`-72  | `width/height`: 18rem;    |
| `w/h`-80  | `width/height`: 20rem;    |
| `w/h`-96  | `width/height`: 24rem;    |

---

Valeur particulière

---

| Valeur       | Rendu                        |
| ------------ | ---------------------------- |
| `w/h`-auto   | `width/height`: auto;        |
| `w/h`-px     | `width/height`: 1px;         |
| `w/h`-full   | `width/height`: 100%;        |
| `w/h`-screen | `width/height`: 100vw;       |
| `w/h`-min    | `width/height`: min-content; |
| `w/h`-max    | `width/height`: max-content; |

---

Valeur pourcentage

---

| Valeur      | Rendu                       |
| ----------- | --------------------------- |
| `w/h`-1/2   | `width/height`: 50%;        |
| `w/h`-1/3   | `width/height`: 33.333333%; |
| `w/h`-2/3   | `width/height`: 66.666667%; |
| `w/h`-1/4   | `width/height`: 25%;        |
| `w/h`-2/4   | `width/height`: 50%;        |
| `w/h`-3/4   | `width/height`: 75%;        |
| `w/h`-1/5   | `width/height`: 20%;        |
| `w/h`-2/5   | `width/height`: 40%;        |
| `w/h`-3/5   | `width/height`: 60%;        |
| `w/h`-4/5   | `width/height`: 80%;        |
| `w/h`-1/6   | `width/height`: 16.666667%; |
| `w/h`-2/6   | `width/height`: 33.333333%; |
| `w/h`-3/6   | `width/height`: 50%;        |
| `w/h`-4/6   | `width/height`: 66.666667%; |
| `w/h`-5/6   | `width/height`: 83.333333%; |
| `w/h`-1/12  | `width/height`: 8.333333%;  |
| `w/h`-2/12  | `width/height`: 16.666667%; |
| `w/h`-3/12  | `width/height`: 25%;        |
| `w/h`-4/12  | `width/height`: 33.333333%; |
| `w/h`-5/12  | `width/height`: 41.666667%; |
| `w/h`-6/12  | `width/height`: 50%;        |
| `w/h`-7/12  | `width/height`: 58.333333%; |
| `w/h`-8/12  | `width/height`: 66.666667%; |
| `w/h`-9/12  | `width/height`: 75%;        |
| `w/h`-10/12 | `width/height`: 83.333333%; |
| `w/h`-11/12 | `width/height`: 91.666667%; |

</details>

---

![size](/images/size.png)

👨‍🎓 TP - Arc en ciel

On va évoluer notre vue en rajouter la width et height. Vous pouvez le faire comme vous voulez.

ex: ![t2](/images/t2.png)

👨‍🏫 Correction : [ici](https://play.tailwindcss.com/oJimUS5j3f)

## Font size

Voilà la syntaxe pour la taille de police.

`.text-TAILLE`

| Class     | Propriété                                  |
| --------- | ------------------------------------------ |
| text-xs   | font-size: 0.75rem; line-height: 1rem;     |
| text-sm   | font-size: 0.875rem; line-height: 1.25rem; |
| text-base | font-size: 1rem; line-height: 1.5rem;      |
| text-lg   | font-size: 1.125rem; line-height: 1.75rem; |
| text-xl   | font-size: 1.25rem; line-height: 1.75rem;  |
| text-2xl  | font-size: 1.5rem; line-height: 2rem;      |
| text-3xl  | font-size: 1.875rem; ine-height: 2.25rem;  |
| text-4xl  | font-size: 2.25rem; line-height: 2.5rem;   |
| text-5xl  | font-size: 3rem; line-height: 1;           |
| text-6xl  | font-size: 3.75rem; line-height: 1;        |
| text-7xl  | font-size: 4.5rem;line-height: 1;          |
| text-8xl  | font-size: 6rem; line-height: 1;           |
| text-9xl  | font-size: 8rem; line-height: 1;           |

![taille](/images/taille.png)

## Padding et Margin

Concernant le padding / margin

`.p{t/r/b/l}-VALEUR`

### Détail des ranges

<details>
 <summary>Cliquez ici</summary>

| Valeur                 | Rendu                       |
| ---------------------- | --------------------------- |
| `p-m{t/r/b/l/y/x}`-0   | `padding/margin`: 0px;      |
| `p-m{t/r/b/l/y/x}`-0.5 | `padding/margin`: 0.125rem; |
| `p-m{t/r/b/l/y/x}`-1   | `padding/margin`: 0.25rem;  |
| `p-m{t/r/b/l/y/x}`-1.5 | `padding/margin`: 0.375rem; |
| `p-m{t/r/b/l/y/x}`-2   | `padding/margin`: 0.5rem;   |
| `p-m{t/r/b/l/y/x}`-2.5 | `padding/margin`: 0.625rem; |
| `p-m{t/r/b/l/y/x}`-3   | `padding/margin`: 0.75rem;  |
| `p-m{t/r/b/l/y/x}`-3.5 | `padding/margin`: 0.875rem; |
| `p-m{t/r/b/l/y/x}`-4   | `padding/margin`: 1rem;     |
| `p-m{t/r/b/l/y/x}`-5   | `padding/margin`: 1.25rem;  |
| `p-m{t/r/b/l/y/x}`-6   | `padding/margin`: 1.5rem;   |
| `p-m{t/r/b/l/y/x}`-7   | `padding/margin`: 1.75rem;  |
| `p-m{t/r/b/l/y/x}`-8   | `padding/margin`: 2rem;     |
| `p-m{t/r/b/l/y/x}`-9   | `padding/margin`: 2.25rem;  |
| `p-m{t/r/b/l/y/x}`-10  | `padding/margin`: 2.5rem;   |
| `p-m{t/r/b/l/y/x}`-11  | `padding/margin`: 2.75rem;  |
| `p-m{t/r/b/l/y/x}`-12  | `padding/margin`: 3rem;     |
| `p-m{t/r/b/l/y/x}`-14  | `padding/margin`: 3.5rem;   |
| `p-m{t/r/b/l/y/x}`-16  | `padding/margin`: 4rem;     |
| `p-m{t/r/b/l/y/x}`-20  | `padding/margin`: 5rem;     |
| `p-m{t/r/b/l/y/x}`-24  | `padding/margin`: 6rem;     |
| `p-m{t/r/b/l/y/x}`-28  | `padding/margin`: 7rem;     |
| `p-m{t/r/b/l/y/x}`-32  | `padding/margin`: 8rem;     |
| `p-m{t/r/b/l/y/x}`-36  | `padding/margin`: 9rem;     |
| `p-m{t/r/b/l/y/x}`-40  | `padding/margin`: 10rem;    |
| `p-m{t/r/b/l/y/x}`-44  | `padding/margin`: 11rem;    |
| `p-m{t/r/b/l/y/x}`-48  | `padding/margin`: 12rem;    |
| `p-m{t/r/b/l/y/x}`-52  | `padding/margin`: 13rem;    |
| `p-m{t/r/b/l/y/x}`-56  | `padding/margin`: 14rem;    |
| `p-m{t/r/b/l/y/x}`-60  | `padding/margin`: 15rem;    |
| `p-m{t/r/b/l/y/x}`-64  | `padding/margin`: 16rem;    |
| `p-m{t/r/b/l/y/x}`-72  | `padding/margin`: 18rem;    |
| `p-m{t/r/b/l/y/x}`-80  | `padding/margin`: 20rem;    |
| `p-m{t/r/b/l/y/x}`-96  | `padding/margin`: 24rem;    |

---

Valeur particulière

---

| Valeur                    | Rendu                          |
| ------------------------- | ------------------------------ |
| `p-m{t/r/b/l/y/x}`-auto   | `padding/margin`: auto;        |
| `p-m{t/r/b/l/y/x}`-px     | `padding/margin`: 1px;         |
| `p-m{t/r/b/l/y/x}`-full   | `padding/margin`: 100%;        |
| `p-m{t/r/b/l/y/x}`-screen | `padding/margin`: 100vw;       |
| `p-m{t/r/b/l/y/x}`-min    | `padding/margin`: min-content; |
| `p-m{t/r/b/l/y/x}`-max    | `padding/margin`: max-content; |

---

Valeur pourcentage

---

| Valeur                   | Rendu                         |
| ------------------------ | ----------------------------- |
| `p-m{t/r/b/l/y/x}`-1/2   | `padding/margin`: 50%;        |
| `p-m{t/r/b/l/y/x}`-1/3   | `padding/margin`: 33.333333%; |
| `p-m{t/r/b/l/y/x}`-2/3   | `padding/margin`: 66.666667%; |
| `p-m{t/r/b/l/y/x}`-1/4   | `padding/margin`: 25%;        |
| `p-m{t/r/b/l/y/x}`-2/4   | `padding/margin`: 50%;        |
| `p-m{t/r/b/l/y/x}`-3/4   | `padding/margin`: 75%;        |
| `p-m{t/r/b/l/y/x}`-1/5   | `padding/margin`: 20%;        |
| `p-m{t/r/b/l/y/x}`-2/5   | `padding/margin`: 40%;        |
| `p-m{t/r/b/l/y/x}`-3/5   | `padding/margin`: 60%;        |
| `p-m{t/r/b/l/y/x}`-4/5   | `padding/margin`: 80%;        |
| `p-m{t/r/b/l/y/x}`-1/6   | `padding/margin`: 16.666667%; |
| `p-m{t/r/b/l/y/x}`-2/6   | `padding/margin`: 33.333333%; |
| `p-m{t/r/b/l/y/x}`-3/6   | `padding/margin`: 50%;        |
| `p-m{t/r/b/l/y/x}`-4/6   | `padding/margin`: 66.666667%; |
| `p-m{t/r/b/l/y/x}`-5/6   | `padding/margin`: 83.333333%; |
| `p-m{t/r/b/l/y/x}`-1/12  | `padding/margin`: 8.333333%;  |
| `p-m{t/r/b/l/y/x}`-2/12  | `padding/margin`: 16.666667%; |
| `p-m{t/r/b/l/y/x}`-3/12  | `padding/margin`: 25%;        |
| `p-m{t/r/b/l/y/x}`-4/12  | `padding/margin`: 33.333333%; |
| `p-m{t/r/b/l/y/x}`-5/12  | `padding/margin`: 41.666667%; |
| `p-m{t/r/b/l/y/x}`-6/12  | `padding/margin`: 50%;        |
| `p-m{t/r/b/l/y/x}`-7/12  | `padding/margin`: 58.333333%; |
| `p-m{t/r/b/l/y/x}`-8/12  | `padding/margin`: 66.666667%; |
| `p-m{t/r/b/l/y/x}`-9/12  | `padding/margin`: 75%;        |
| `p-m{t/r/b/l/y/x}`-10/12 | `padding/margin`: 83.333333%; |
| `p-m{t/r/b/l/y/x}`-11/12 | `padding/margin`: 91.666667%; |

</details>

---

Padding

---

![padding](/images/p-all.png)
![padding](/images/p.png)
![padding](/images/py.png)
![padding](/images/px.png)

---

Margin

---

![margin](/images/m-all.png)
![margin](/images/m.png)
![margin](/images/my.png)
![margin](/images/mx.png)

👨‍🎓 TP - Arc en ciel

Inserer un margin sur chaque couleurs de notre arc en ciel pour faire un effet acordéon

Ex :
![aec](/images/t3.png)

👨‍🏫 Correction : [ici](https://play.tailwindcss.com/Q7YK7HKTxx)

## Textes

Ok, c'est sympa notre arc en ciel mais on ne fait pas encore réellement de CSS, avec du texte, du style etc.

Concernant le texte, c'est comme le background-color. C'est à dire que nous avons les mêmes couleurs (voir la section bg)

👨‍🎓 TP - Texte

Ecrire 3 paragraphes ([lorem ipsum](https://www.lipsum.com/) suffit !) avec le background qui possède une couleur de nuance 100 et le texte la nuance 600 de la même couleur. N'hésitez pas à aérer vos div avec un padding ou margin.

Ex:
![bg and text](/images/bg-text.png)

👨‍🏫 Correction : [ici](https://play.tailwindcss.com/p9rWwOnPWk)

## Le hover

Pour ajouter du css sur le hover, Tailwind à mis à disposition une classe dédié qui est `hover:`

Et, sur le même principe que pour le texte ou le background. J'ai les mêmes couleur à chaque fois.

👨‍🎓 TP - Hover

J'indique que sur le hover, je souhaite inverser les couleurs de mon backgroud-color et mon texte.

Ex:
![hover](/images/hover.png)

👨‍🏫 Correction : [ici](https://play.tailwindcss.com/3N4oujOzrW)

## Les gradiants

Pour insérer un gradient avec tailwind il faut utiliser la propriété

-   `bg-gradient-to-`{valeur}
-   `from-`blue-600. On commence à (from)
-   `via-`purple-60. Si on souhaite une couleur intermédiaire
-   `to-`blue-30. On fini à (to)

Les propriétés de `bg-gradient-to-` sont les suivantes :

| valeur | css          |
| ------ | ------------ |
| `t`    | top          |
| `b`    | bottom       |
| `r`    | right        |
| `l`    | left         |
| `tr`   | top-right    |
| `tl`   | top-left     |
| `br`   | bottom-right |
| `bl`   | bottom-left  |

## Texte Gradient

Pour le texte gradient, nous allons faire un bg-gradient avec la direction.
Ensuite on indique les 2 classes suivantes :

-   `text-transparent`
-   `bg-clip-text`

![text gradient](/images/text-gradient.png)

👨‍🏫 Correction : [ici](https://play.tailwindcss.com/EKCqKJpVwX)

## Responsive

Tailwind est conçu pour être “mobile first”.

C'est à dire que le CSS qu'on écrit est prévu de base pour les mobiles, ensuite, nous allons écrire le CSS pour les medias superieurs (Tablette, Desktop, TV)

👨‍🏫 Correction : [ici](https://play.tailwindcss.com/2aC5fqyz1u)

![responsive](/images/responsive.png)

## Grid

Nous allons manipuler les grilles sur tailwind pour comprendre comment il fonctionne 😁

Voilà déjà la documentation concernant les grilles : 

![grid](/images/grid.png)

Mais ça veut dire quoi ça ?

Si nous faisons un tour sur leur éditeur !

[Ici](https://play.tailwindcss.com/aQksJUCIsc) par exemple ! 

Analysons la ligne suivante 

```html
<ul class="grid grid-cols-1 gap-4 sm:grid-cols-2 md:grid-cols-3 md:gap-8">
```

Déjà, nous avons la classe : `grid` qui indique que ce qui suit sera sous forme de grille

Ensuite `grid-cols-1`, ne l'oublions pas, tailwind est `mobile-first` donc, c'est le comportement par défaut si nous rajoutons rien !

- `gap-4` c'est l'espace que doit avoir les éléments entre eux.

- `sm:grid-cols-2` on vient de rajouter un média query ici qui comprend les écrans de petite taille (640px). On indique que pour les écrans qui ont au minimum 640px, ils auront 2 colonnes.

donc, nos dis auront 2 comportements 
  - 1 pour les écrans petit
  - 1 pour les media qui ont au minimum 640px

- `md:grid-cols-3` sur le même principe que ci-dessus

- `md:gap-8` ce style sera appliqué que si l'écran et de taille md soit au minimum 768px.

Ensuite, ce sont des divs 'classique'.

Amusons nous maintenant avec les tailles !

👨‍🎓 TP Grid

Créer une grille de 1 colonne pour les mobiles, 3 colonnes pour les petits écrans et 6 colonnes pour les écrans moyens.

👨‍🏫 Correction : [ici](https://play.tailwindcss.com/EFf1uqQNSF)

⚠️ Pour la suite, on va tous partir du code suivant pour avoir la même base :

```html
<div class="h-screen flex items-center bg-gradient-to-b from-blue-600 to-purple-600">
  <div class="flex-1 p-10">
    <ul class="grid grid-cols-6 gap-8">
      <li class="bg-white rounded-lg shadow-xl"><div class="h-24"></div></li>
      <li class="bg-white rounded-lg shadow-xl"><div class="h-24"></div></li>
      <li class="bg-white rounded-lg shadow-xl"><div class="h-24"></div></li>
      <li class="bg-white rounded-lg shadow-xl"><div class="h-24"></div></li>
      <li class="bg-white rounded-lg shadow-xl"><div class="h-24"></div></li>
      <li class="bg-white rounded-lg shadow-xl"><div class="h-24"></div></li>
      <li class="bg-white rounded-lg shadow-xl"><div class="h-24"></div></li>
      <li class="bg-white rounded-lg shadow-xl"><div class="h-24"></div></li>
      <li class="bg-white rounded-lg shadow-xl"><div class="h-24"></div></li>
      <li class="bg-white rounded-lg shadow-xl"><div class="h-24"></div></li>
      <li class="bg-white rounded-lg shadow-xl"><div class="h-24"></div></li>
      <li class="bg-white rounded-lg shadow-xl"><div class="h-24"></div></li>
    </ul>
  </div>
</div>
```

Pour changer la taille d'une colonne, nous allons utiliser la propriété CSS de tailwind qui est `col-span-{n}`. La [doc](https://tailwindcss.com/docs/grid-column) ici !

{n} vaut un nombre entre 1 et 12, il existe 2 valeurs qui ne possède pas de chiffre, `auto` et `full`.

Mais ça veut dire quoi ? Enfaite, ça veut dire que nous allons prendre {n} place dans notre grid !

👨‍🎓 TP Span

Jouer avec la taille des éléments pour que ça ressemble plus ou moins à ça :

![tp-span](/images/tp-span.png)

👨‍🏫 Correction : Voyons un exemple [ici](https://play.tailwindcss.com/DdPAdNFguH)

Ensuite, nous avons `col-{start/end}-{n}`. Ici, j'écris {start/end} car c'est la même choses pour le début et pour la fin. {n} on la vu plus haut mais sur les valeurs de {start/end} il y a le `13` en plus. Mais pourquoi 13 ? Si je fait 12 colonnes je suis censé allez jusqu'à 12 ? Et bien non ! Je t'invite à faire ce petit jeu sympa -> [grid garden](https://cssgridgarden.com/#fr) tu auras les bases pour comprendre le concept (après tu as la [doc](https://developer.mozilla.org/fr/docs/Web/CSS/CSS_Grid_Layout) mais c'est moins ludique !)


Ici, nous avons un exemple avec `col-start-4` : [exemple](https://play.tailwindcss.com/kI8VvXynLW)

Et le rendu avec l'affichage de la grille

![display grid](/images/col-start-grid.png)

Nous voyons bien qu'il commence à 4 comme indiqué ci dessus. Et vu que je ne lui ai pas donnée de l'argeur ni même de fin, alors il gared sa taille de base.

Maintenant je vais lui ajouter une fin avec `col-end-6`, [exemple](https://play.tailwindcss.com/B5spZTm7Qm)

![display grid](/images/col-end-grid.png)

Et si je ne met pas de start, mais que la fin alors ça resemble à [ça](https://play.tailwindcss.com/8i5T6ftt3T)

![display grid](/images/just-end-grid.png)

Et maintenant, je vais aussi ajouter un `col-span-4` combiné avec `col-end-6` ça donne ce [résultat](https://play.tailwindcss.com/gDWsleM0Oi) !

![display grid](/images/end-span-grid.png)

C'est super ! On comprend comment fonctionne tailwind avec les grids sur les colonnes ! Mais sur les lignes, les `row` c'est pareil ? **Oui, absolument**, ce qui est valable pour les `col`, est aussi valable pour les `row`, [regardons](https://play.tailwindcss.com/2sp6VQmZWC) !

![display grid](/images/row-grid.png)

👨‍🎓 TP start/end

Vous devez refaire la même chose que l'image ci dessous .

![tp-span](/images/tp-start.png)

👨‍🏫 Correction : Voyons une solution [ici](https://play.tailwindcss.com/kgH6NiFJGE)

## Flexbox

Concernant les flexbox, tailwind fait sensiblement la même chose que les grids.

En effet, nous devons indiquer sur la div parent que les éléments sont flex, et leur ajouter des classes pour quelles correspondent à ce que je veux. 

Voilà de la doc et voilà LA [doc](https://tailwindcss.com/docs/flex-direction) !


![display grid](/images/flex.png)
![display grid](/images/flex-direction.png)
![display grid](/images/flex-wrap.png)
![display grid](/images/flex-order.png)

Quelques petits exo avant un petit challenge !

**Utilisation du flex**

[Ici](https://play.tailwindcss.com/h4WGjlDnI1) nous allons manipuler le flex.

Comment je fais ? J'indique dans la div parent (la plus haute) que mes enfants soit flex.

Ensuite nous avons les directions :

**Justify-{alignement}**

| Alignement                                         | valeur par defaut |
| :------------------------------------------------- | :---------------- |
| [start](https://play.tailwindcss.com/o7LoIob0bp)   | [x]               |
| [center](https://play.tailwindcss.com/VQ6KvvMGO7)  |                   |
| [end](https://play.tailwindcss.com/2dS0W69tN0)     |                   |
| [between](https://play.tailwindcss.com/5tei7BnH9S) |                   |
| [around](https://play.tailwindcss.com/HBPBMmi8Vn)  |                   |

**items-{alignement}**

| Alignement                                         | valeur par defaut |
| :------------------------------------------------- | :---------------- |
| [stretch](https://play.tailwindcss.com/HozYVKJMLS) | [x]               |
| [start](https://play.tailwindcss.com/HozYVKJMLS)   |                   |
| [center](https://play.tailwindcss.com/NFQmRXuRM5)  |                   |
| [end](https://play.tailwindcss.com/3rfRwJeJXO)     |                   |


**flex-{wrapMode}**

| wrapMode                                                | valeur par defaut |
| :------------------------------------------------------ | :---------------- |
| [no-wrap](https://play.tailwindcss.com/N58nj06bJl)      | [x]               |
| [wrap](https://play.tailwindcss.com/PXHUV6PrBS)         |                   |
| [wrap-reverse](https://play.tailwindcss.com/E5x9EZdtEB) |                   |

👨‍🎓 Challenge

- Chaque cases doit occuper tout l'espace disponible 
- Une grille 3x3 distribuée uniformément 
- Les lettres doivent être centrées sur le carré 

La base du code

```html
<div>
  <div class="bg-green-100">A</div>
  <div class="bg-green-200">B</div>
  <div class="bg-green-300">C</div>
  <div class="bg-green-400">D</div>
  <div class="bg-green-500">E</div>
  <div class="bg-green-600">F</div>
  <div class="bg-green-700">G</div>
  <div class="bg-green-800">H</div>
  <div class="bg-green-900">I</div>
</div>
```

👨‍🏫 Correction : [ici](https://play.tailwindcss.com/GRPsQSgJAo)

<details>
  <summary>Les étapes de mon raisonnement</summary>

  1. Informer que mes enfants sont flex grâce à la classe `flex`
  2. J'indique que je dois avoir 3 lignes de 3 cases. Rappelons nous qu'il existe la classe `w-1/3` grâce à la [doc](https://tailwindcss.com/docs/width)
  3. C'est bien, mais maintenant il faut avertir que je souhaite retourner à la ligne si j'ai pas assez de place grâce à `flex-wrap`
  4. J'indique que ma div global est 100vh et sur tailwind, je le dis avec `h-screen`
  5. Pour centrer un élément on utilise le duo `justify-center` et `items-center`, mais pour que ça marche, il faut dire que chacun de mes éléments doit être `flex`
  
**Code final**

```html
<!-- Doit occuper tout l'espace disponible -->
<!-- Une grille 3x3 distribuée uniformément -->
<!-- Les lettres doivent être centrées sur le carré -->
<div class="h-screen flex flex-wrap">
  <div class="bg-green-100 w-1/3 flex justify-center items-center">A</div>
  <div class="bg-green-200 w-1/3 flex justify-center items-center">B</div>
  <div class="bg-green-300 w-1/3 flex justify-center items-center">C</div>
  <div class="bg-green-400 w-1/3 flex justify-center items-center">D</div>
  <div class="bg-green-500 w-1/3 flex justify-center items-center">E</div>
  <div class="bg-green-600 w-1/3 flex justify-center items-center">F</div>
  <div class="bg-green-700 w-1/3 flex justify-center items-center">G</div>
  <div class="bg-green-800 w-1/3 flex justify-center items-center">H</div>
  <div class="bg-green-900 w-1/3 flex justify-center items-center">I</div>
</div>

```
</details>

👨‍🎓 TP Form

Créer l'input suivant

![tp 5](/images/tp-5.png)

👨‍🏫 Correction : [ici](https://play.tailwindcss.com/KudpoSLnAC)

<details>
  <summary>Les étapes de mon raisonnement</summary>

  1. Je créer une div qui prend en hauteur 100vh (`h-screen`), elle est `flex`, puis j'indique la direction avec `flex-col` et je centre avec `justify-center items-center`
  2. Je créer un `label` un `input` et un `button` sans rien.
  3. Le label
     1. J'indique que le text est gray et en bold, je rajoute `select-none` comme ça je ne peux pas selectionner le label
  4. L'input
     1. Je met une marge top, un effet de shadow et les bords arrondies
     2. Je grossie sa taille grâce à `w-4/6` et je met des paddings
     3. Ensuite je met le texte en gris
     4. Un focus en blue
     5. et le placeholder en indigo
  5. Le button
     1. Marge top avec les paddings qui vont avec
     2. couleur bleu foncée 
     3. le texte en blanc 
     4. arrondie
  
**Code final**

```html
<div class="h-screen flex flex-col justify-center items-center">
  <label for="full_name" class="text-gray-700 text-sm font-bold select-none">Nom Prénom</label>
  <input id="full_name" placeholder="Bob l'éponge" class="mt-2 shadow border rounded-lg w-4/6 px-3 py-2 text-gray-700 focus:bg-blue-100 placeholder-indigo-300" />
  <button class="mt-2 px-3 py-2 bg-blue-900 text-blue-100 rounded-lg">Go!</button>
</div>
```
</details>

👨‍🎓 TP First card

Créer la carte suivante : 

![tp 8](/images/tp-8.png)

👨‍🏫 Correction : [ici](https://play.tailwindcss.com/548UviwQDq)

<details>
  <summary>Les étapes de mon raisonnement</summary>

  1. Je créer une div avec un padding et j'indique que pour les ecrans au dela de 768px la carte fait 33%
  2. Je met le bg et les paddings pour faire jolie
  3. Je met du style dans mes ecriture pour faire jolie (la [doc](https://tailwindcss.com/docs/font-family))
  
**Code final**

```html
<div class="p-4 md:w-1/3">
  <div class="bg-gray-100 px-8 pt-16 pb-24 rounded-lg text-center">
    <h2 class="tracking-widest text-xs font-medium text-gray-400 mb-1">CATEGORY</h2>
    <h1 class="sm:text-2xl text-xl font-medium text-gray-900 mb-3">Lorem ipsum</h1>
    <p class="leading-relaxed mb-3">Lorem ipsum dolor, sit amet consectetur adipisicing elit. At neque ullam magnam nemo eos, inventore doloremque ab omnis cumque minus soluta consectetur dicta!</p>
    <a class="text-green-500 items-center">Lorem Ipsum </a>
  </div>
</div>
```
</details>

👨‍🎓 TP Carte

Créer la carte suivante : 

![tp 6](/images/tp-6.png)

👨‍🏫 Correction : [ici](https://play.tailwindcss.com/w8OdBAMl6j)

👨‍🏫 Ici avec un exemple de responsive : [ici](https://play.tailwindcss.com/ELvcUE8AZJ)

<details>
  <summary>Les étapes de mon raisonnement</summary>

  1. J'indique que ma carte sera centré, nous avons l'habitude
     1. `flex flex-col h-screen justify-center items-center`
  2. Ensuite, j'indique que ma carte fera 33% de largeur 
  3. Je commence par dessiner la carte ensuite, dans l'ordre
     1. L'image (un peu de [doc](https://tailwindcss.com/docs/object-fit))
     2. Une div qui contiendra
        1. Une catégorie avec un style d'écriture [comme ça](https://tailwindcss.com/docs/letter-spacing#class-reference)
        2. Un titre
        3. Une description
        4. Et pour finir une div qui contiendra mon dernier lien
  
**Code final**

```html
<div class="flex flex-col h-screen justify-center items-center">
  <div class="w-1/3">
    <div class="border-2 border-gray-200 border-opacity-60 rounded-lg overflow-hidden">
      <img class="object-cover object-center" src="https://picsum.photos/720/400" alt="blog" />
      <div class="p-6">
        <h2 class="tracking-widest text-xs font-medium text-gray-400 uppercase mb-1">Lorem</h2>
        <h1 class="text-lg font-medium text-gray-900 mb-3">Lorem ipsum</h1>
        <p class="mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis harum omnis nobis quis officiis maxime cumque accusantium!</p>
        <div>
          <a class="text-indigo-500 inline-flex items-center md:mb-2 lg:mb-0">Encore plus !</a>
        </div>
      </div>
    </div>
  </div>
</div>
```
</details>

👨‍🎓 TP Citation

Créer la carte suivante : 

![tp 7](/images/tp-7.png)

le code SVG des quottes

```html
<svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="inline-block w-8 h-8 text-gray-400 mb-8" viewBox="0 0 975.036 975.036">
        <path d="M925.036 57.197h-304c-27.6 0-50 22.4-50 50v304c0 27.601 22.4 50 50 50h145.5c-1.9 79.601-20.4 143.3-55.4 191.2-27.6 37.8-69.399 69.1-125.3 93.8-25.7 11.3-36.8 41.7-24.8 67.101l36 76c11.6 24.399 40.3 35.1 65.1 24.399 66.2-28.6 122.101-64.8 167.7-108.8 55.601-53.7 93.7-114.3 114.3-181.9 20.601-67.6 30.9-159.8 30.9-276.8v-239c0-27.599-22.401-50-50-50zM106.036 913.497c65.4-28.5 121-64.699 166.9-108.6 56.1-53.7 94.4-114.1 115-181.2 20.6-67.1 30.899-159.6 30.899-277.5v-239c0-27.6-22.399-50-50-50h-304c-27.6 0-50 22.4-50 50v304c0 27.601 22.4 50 50 50h145.5c-1.9 79.601-20.4 143.3-55.4 191.2-27.6 37.8-69.4 69.1-125.3 93.8-25.7 11.3-36.8 41.7-24.8 67.101l35.9 75.8c11.601 24.399 40.501 35.2 65.301 24.399z"></path>
      </svg>
```

👨‍🏫 Correction : [ici](https://play.tailwindcss.com/bY5cPUNjLm)

<details>
  <summary>Les étapes de mon raisonnement</summary>

  1. J'indique que tout mon texte sera gris
  2. Je met du padding / margin
  3. J'importe le svg
  4. Je stylise un peu mon texte avec les infos fournie dans la [doc](https://tailwindcss.com/docs/line-height#class-reference)
  5. Je stylise une petite barre en mode `inline` sinon ça ne fonctionne pas
  6. Je fini avec le footer de l'auteur
  
**Code final**

```html
<div class="text-gray-600 body-font">
  <div class="px-5 py-24 mx-auto">
    <div class="w-full mx-auto text-center">
      <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="inline-block w-8 h-8 text-gray-400 mb-8" viewBox="0 0 975.036 975.036">
        <path d="M925.036 57.197h-304c-27.6 0-50 22.4-50 50v304c0 27.601 22.4 50 50 50h145.5c-1.9 79.601-20.4 143.3-55.4 191.2-27.6 37.8-69.399 69.1-125.3 93.8-25.7 11.3-36.8 41.7-24.8 67.101l36 76c11.6 24.399 40.3 35.1 65.1 24.399 66.2-28.6 122.101-64.8 167.7-108.8 55.601-53.7 93.7-114.3 114.3-181.9 20.601-67.6 30.9-159.8 30.9-276.8v-239c0-27.599-22.401-50-50-50zM106.036 913.497c65.4-28.5 121-64.699 166.9-108.6 56.1-53.7 94.4-114.1 115-181.2 20.6-67.1 30.899-159.6 30.899-277.5v-239c0-27.6-22.399-50-50-50h-304c-27.6 0-50 22.4-50 50v304c0 27.601 22.4 50 50 50h145.5c-1.9 79.601-20.4 143.3-55.4 191.2-27.6 37.8-69.4 69.1-125.3 93.8-25.7 11.3-36.8 41.7-24.8 67.101l35.9 75.8c11.601 24.399 40.501 35.2 65.301 24.399z"></path>
      </svg>
      <p class="leading-relaxed text-lg">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Consectetur deserunt ratione velit voluptatibus rem ducimus quasi totam harum necessitatibus autem? Consectetur deserunt libero animi dolores enim? Molestias modi officia ad.</p>
      <span class="inline-block h-1 w-10 rounded bg-yellow-500 mt-8 mb-6"></span>
      <h2 class="text-gray-900 font-medium tracking-wider text-sm uppercase">ANONYMOUS</h2>
      <p class="text-gray-500">A great anonymous person</p>
    </div>
  </div>
</div>
```
</details>


## Les images

Pas grand chose de plus à dire par rapport à la [doc](https://tailwindcss.com/docs/object-fit). Il faut essayer d'importer une photo et tenter de manipuler avec ça ! 

![obj fit](/images/object-fit.png)
![obj position](/images/object-position.png)

Et pour plus de fun, il y a un [visuel](https://play.tailwindcss.com/HIp9cTWl2I) qui va permettre de manipuler les images.