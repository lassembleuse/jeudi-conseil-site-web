# Je veux faire mon site web moi-même ! - Programme

Se créer un site en ligne rapidement avec github pages

## Préambule

### C'est quoi un site statique ?

Site simple, HTML, CSS et éventuellement du javascript. Toutes les pages sont générées au moment du déploiement, et non pas générées dynamiquement pendant qu'on navigue sur le site.

### C'est quoi git et github ?

- [GitHub Pour les Nuls : Pas de Panique, Lancez-Vous !](https://www.christopheducamp.com/2013/12/15/github-pour-nuls-partie-1/)

## Tutoriel

### Un site tout simple avec un thème

- rendez-vous sur [https://github.com](https://github.com), et créez un compte gratuit
- Créez un nouveau `repository`, et l'initialiser avec un fichier `read.me`
- Aller dans `settings` -> Github pages -> sélectionner `master branch` comme source et sauver.
- Se rendre sur son site en ligne :)
- Modifier le `read.me` et constater le changement !
- Choisir un thème dans `settings`
- Attendre quelques instants et constater le changement sur son site en ligne !

> Mais d'où vient cette magie ?
> Derrière github pages mouline [Jekyll](https://jekyllrb.com/), un **générateur de sites statiques**. Quelques fichiers sont cachés par github et permettent derrière le rideau de faire tourner la machine. Les fichiers d'un site statique basique fait avec Jekyll ressemblent à ça : [site jekyll vierge](https://github.com/lassembleuse/blank-jekyll-starter)
> Quelques ressources pour en savoir plus : 
> - [Générateur de site statique, un modèle alternatif](https://www.quaternum.net/2016/01/09/generateur-de-site-statique-un-modele-alternatif/)
> - [Les générateurs de site statique](https://bertrandkeller.info/generateur-site-statique/)

## Personnaliser son site

### Personnaliser le CSS de votre thème Jekyll

1. Créez un fichier appelé `/assets/css/style.scss` à la racine du dépôt de votre site.

2. Ajoutez le contenu suivant en haut du fichier, exactement comme indiqué :
  
```
---
---

@import "{{{site.theme}}}" ;
```

3. Ajoutez du CSS personnalisé comme vous souhaitez immédiatement après la ligne `@import`.

### Personnalisation de la mise en page HTML de votre thème Jekyll

1. Naviguez jusqu'au fichier `_layouts/default.html` du dépôt de votre thème Jekyll. Par exemple, accédez à `https://github.com/pages-themes/THEME_NAME/blob/master/_layouts/default.html` et remplacez `THEME_NAME` par le nom de votre thème Jekyll.

Liste de tous les dépôts des thèmes : [https://github.com/pages-themes](https://github.com/pages-themes)

2. Copiez le contenu de `default.html`.

> Astuce : Cliquez sur Raw dans le coin supérieur droit de la page pour modifier l'affichage du fichier afin de faciliter la copie.

3. Créez un fichier appelé `/_layouts/default.html` dans le dépôt de votre site.

4. Collez le contenu de la mise en page par défaut copié à l'étape 2 dans le nouveau fichier `/_layouts/default.html` du dépôt de votre site.

5. Personnalisez la mise en page comme vous le souhaitez.


- [Customizing CSS and HTML in your Jekyll theme](https://help.github.com/en/articles/customizing-css-and-html-in-your-jekyll-theme)

# Aller plus loin 

- installer git sur son ordinateur pour pouvoir éditer son site depuis son ordinateur
- installer ruby et jekyll pour pouvoir éditer tous les fichiers de son site

## Ressources pour les participants

- [https://gitlab.com/pages?page=1](https://gitlab.com/pages?page=1) : exemple de sites générés sur gitlab pages avec différents générateurs de sites statiques

# Quelques liens utiles

- ⚙️ Assemblage avec Jekyll : [https://jekyllrb.com/docs/](https://jekyllrb.com/docs/)
  - Variables : [https://jekyllrb.com/docs/variables/](https://jekyllrb.com/docs/variables/)
  - Filtres de données : [https://jekyllrb.com/docs/liquid/filters/](https://jekyllrb.com/docs/liquid/filters/)
  - Gabarits : [https://jekyllrb.com/docs/layouts/](https://jekyllrb.com/docs/layouts/)
  - Inclusions : [https://jekyllrb.com/docs/includes/](https://jekyllrb.com/docs/includes/)
- 📝 Syntaxe Markdown (`.md`) : [https://fr.wikipedia.org/wiki/Markdown#Quelques_exemples](https://fr.wikipedia.org/wiki/Markdown#Quelques_exemples)
- 🎨 Présentation avec CSS : [https://developer.mozilla.org/fr/docs/Web/CSS/Reference](https://developer.mozilla.org/fr/docs/Web/CSS/Reference)
- 🏷 Structure avec HTML : [https://developer.mozilla.org/fr/docs/Web/HTML/Element](https://developer.mozilla.org/fr/docs/Web/HTML/Element)



## Ressources et inspirations pour cet atelier
- https://github.com/daktary-team/maquillage : pour les explications + captures d'écran de comment créer un site avec github pages.
- https://github.com/oncletom/demo.usinevivante.org
- https://github.com/oncletom/enssib-m2-pn#pr%C3%A9-requis
- https://github.com/oncletom/m2-transfo-num

- [https://putaindecode.io/articles/creer-un-site-web-gratuitement-avec-github-pages/](https://putaindecode.io/articles/creer-un-site-web-gratuitement-avec-github-pages/)
- [https://www.christopheducamp.com/2013/12/21/demarrer-avec-pages-github/](https://www.christopheducamp.com/2013/12/21/demarrer-avec-pages-github/)
- [https://pages.github.com/](https://pages.github.com/)
- [https://guides.github.com/features/pages/](https://guides.github.com/features/pages/)