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
