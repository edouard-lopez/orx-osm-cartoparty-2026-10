---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
# background: https://cover.sli.dev
background: /background.jpg
# some information about your slides (markdown enabled)
title: Presentation d'OSM (OpenStreetMap)
info: |
  ## Presentation d'OSM (OpenStreetMap)
  OpenstreetMap (OSM) est une carte collaborative et libre

  [En savoir plus sur OpenStreetMap](https://www.openstreetmap.org/)
# apply UnoCSS classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/a`nimations.html#slide-transitions
transition: slide-left
# enable Comark Syntax: https://comark.dev/syntax/markdown
comark: true
# duration of the presentation
duration: 30min
---

# OpenStreetMap

## Carte collaborative et libre

Présentation pour la cartopartie du 24 octbre 2026
  <br>
<small>Par Édouard Lopez / Groupe Mapadour</small>

<div @click="$slidev.nav.next" class="mt-12 py-1" hover:bg="white op-10">
  [Space] <carbon:arrow-right />
</div>

<div class="abs-br m-6 text-xl">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="slidev-icon-btn">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->
---
hideInToc: true
---

# Sommaire

<Toc minDepth="1" maxDepth="1" />


---
layout: two-cols
---

# Contexte de l'événement

* Orx: village nature et nourricier
* Inclus Kfé: café associatif, inclusion et lieu de rencontre
* Mapadour: groupe local de contributeurs OSM sur le Pays-Basque et le Sud des landes
* Édouard: Ingénieur logiciel et contributeur des communs (OSM, Wiki, Jardin Partagé)


::right::

![Lào Map](/lào-map.svg)


---
layout: two-cols
---

# Historique

La France a une longue tradition de la cartographie !

## Cartographie en France

* XVIII<sup>e</sup> siècle : [Carte de Cassini][cassini] par [triangulation][triangulation]
* XIX<sup>e</sup> siècle : Carte d'état major
* XX<sup>e</sup> siècle : Cartes topographiques de l'[IGN][ign]
* XXI<sup>e</sup> siècle : [cartes numériques et collaboratives][osm].

::right::

<div class="flex flex-col items-center gap-8 align-center">
  <figure class="flex flex-col items-center">
    <img src="/histoire-carte-cassini-1783.JPG" alt="Carte de France de 1783 (partie Nord-Ouest)." width="250vh" >
    <figcaption class="text-center text-sm">
      <i>Par Cassini de Thury</i>
      <!-- — Planche de l'ouvrage de J.J. Levallois Mesurer la Terre., Domaine public, https://commons.wikimedia.org/w/index.php?curid=41009875 -->
    </figcaption>
  </figure>

  <figure class="flex flex-col items-center">
    <img src="/histoire-planchette_2_1751.jpg" alt="Carte de France de 1783 (partie Nord-Est)." width="125vh" >
    <figcaption class="text-center text-sm">
      <i>Levé à la planchette</i>
      <!-- Par de Marinoni — BnF, Gallica, ETH-Bibliothek Zürich, De re ichnographica, accès en ligne, voir p. 49., Domaine public, https://commons.wikimedia.org/w/index.php?curid=43339156 -->
    </figcaption>
  </figure>
</div>

[triangulation]: https://www.youtube.com/watch?v=8mbmY8kYp5g "La cartographie au fil du temps – de 1667 aux années 2000"
[cassini]: https://fr.wikipedia.org/wiki/Carte_de_Cassini
[ign]: https://fr.wikipedia.org/wiki/Institut_national_de_l%27information_g%C3%A9ographique_et_foresti%C3%A8re
[osm]: https://openstreetmap.org


---
layout: two-cols
---

# OpenStreetMap

Projet **collaboratif** de cartographie en ligne qui vise à constituer une **base de données géographiques libre** du monde

Créé en 2004 par Steve Coast à l'University College de Londres.

* Principe collaboratif comme Wikipédia
* Base de données géographiques au Monde.
  * 1 point = plusieurs informations
* Libre d'utilisation (licence _Open Database License_)
  * Les données peuvent être utilisées, modifiées et partagées librement
* En évolution permanente
* Réactive <abbr title="Humanitarian OpenStreetMap Team"> [HOT][HOT] </abbr>

[HOT]: https://www.hotosm.org/en/
::right::

<div class="flex flex-col items-center gap-8 align-center">

![logo OSM](/logo-osm.png)

</div>


---
layout: two-cols
---

# Participatif

OpenStreetMap, c’est l’équivalent de Wikipédia pour les cartes

Vous connaissez bien le quartier dans lequel vous vivez? Quelques choses à changer ? C'est l'occasion de contribuer

## 🌪💥 Lors de crises

OpenStreetMap permet de [cartographier rapidement les zones touchées][crisis-mapping] pour faciliter l'aide et la coordination des secours.

ex. Lors du passage à  [Mayotte de la tempête Chido : cartographie des dommages des bâtiments][mayotte-chido]

[crisis-mapping]: https://doi.org/10.1111/1468-5973.12330
[mayotte-chido]: https://forum.openstreetmap.fr/t/mayotte-chido-cartographie-des-dommages-des-batiments/31722

::right::


# Communautés
  * Fondation (monde) 2006
  * Association OSM-France 2011
  * Mapadour: Sud-Landes Pays-Basque

<style>
  .slidev-layout {
    gap: 3rem;

    div.col-right, ul {
      margin-left: 2rem;
    }
  }

</style>

---

## Mondial

* OpenStreetMap est la plus grande base libre de données géographiques au Monde.
* +10 millions de contributeur-ices dans le monde entier (chiffres de 2025) ;

> Nous cartographions le globe, rue après rue, chemin après chemin, tout simplement.



---
layout: two-cols-header
---

# Libre

Vous êtes libre d’utiliser, télécharger et remixer toutes nos données, et ce même dans un but commercial. Les données sont publiées sous licence ouverte.

> Nous croyons en un monde où les données cartographiques sont libres et ouvertes.

<br>

::left::

À quoi ça sert ? Il y a déjà l’IGN et Google Maps ?

<!-- [ya-google-map]: https://www.palabritudes.net/2024/08/15/quinze-ans-contribution-osm.html -->

* Les rendus des cartes sont souvent
  * figés et non personnalisable
  * orientées publicités
* màj surtout sur les zones urbaines
* les données ne sont pas libres

::right::

<div class="flex flex-col items-center gap-4">

  <figure class="flex flex-row items-center">
  <img src="/StreetComplete-logo.svg" alt="streetcomplete logo">
  <figcaption class="text-center text-sm">

  [StreetComplete](https://streetcomplete.app/)

  </figcaption>
  </figure>

  <figure class="flex flex-row items-center">
  <img src="/logo-osm.png" alt="OSM logo" width="80vh" >
  <figcaption class="text-center text-sm">

  l'[Éditeur web d'OSM](https://www.openstreetmap.org)

  </figcaption>
  </figure>

  <figure class="flex flex-row items-center">
  <img src="/Panoramax_logo.svg" alt="Panoramax logo" width="80vh">
  <figcaption class="text-center text-sm">

  [Panoramax](https://panoramax.openstreetmap.fr)

  </figcaption>
  </figure>
</div>

---
layout: two-cols
---

# Des données de qualité

Des données basées sur les connaissances du terrain, collectées par des contributeur-ices du monde entier.

La qualité des données motive les institutions à collaborer avec OSM:
* Base Adresses Nationale
* Projet leader mondial ([Panoramax][panoramax])
* Situation de crise
* Création d'entreprise (ex. Géovélo)

[panoramax]: https://panoramax.openstreetmap.fr

::right::

# Mise à jour en continue

Constamment mises à jour par des contributeur-ices du monde entier et mise à disposition à la volée.

* [Pifomètre][pifometre]: rapprocher les données OpenStreetMap, le fichier Topo (ex-Fantoir), le cadastre et la BAN pour favoriser l'enrichissement
* Utilisation par les villes pour du suivi des infrastructures et de l'urbanisme

[pifometre]: https://www.palabritudes.net/2024/08/15/quinze-ans-contribution-osm.html

---

## Utilisez par… !

De nombreux acteurs s’appuient sur l’écosystème OpenStreetMap, ses données, ses cartes ou encore ses services. Nous y retrouvons des citoyennes et des citoyens, des collectivités, des associations et des entreprises de toutes tailles:

* Entreprises: Amazon, Apple, Baidu Maps, Facebook, Microsoft, Wikipedia, Pinterest etc.
* Gouvernements: 🇫🇷 Gendarmerie et Police, 🇧🇷 Brésil, France Base des adresses nationales, 🇮🇹 Italie, 🇱🇸 Lesotho, 🇱🇹 Lithuania, 🇵🇱 Pologne, 🇨🇦 Canada, etc.
* Entreprises du TransporT: SNCF, Air France, Uber, Deutsche Bahn, etc.
* Associations: MSF (Médecins Sans Frontières), ONU (Organisation des Nations Unies), Croix Rouge, etc.
* Universités: Cambridge
* Media: BBC, Wall Street Journal, etc.

[Qui l'utilise ?][qui-utilise]

[qui-utilise]: https://welcome.openstreetmap.org/about-osm-community/consumers/

---
layout: two-cols
---
# StreetComplete

Application pour contribuer à la base OpenStreetMap au travers d'un système de questions simples sur les éléments environnants incomplètement renseignés

* iOS & Android

  <figure class="flex flex-col items-center">
  <img src="/StreetComplete-logo.svg" alt="streetcomplete logo">
  <figcaption class="text-center text-sm">

  [StreetComplete](https://streetcomplete.app/)

  </figcaption>
  </figure>

::right::

![les quetes dans streetcomplete](/streetcomplete-quetes.jpeg)


---
layout: two-cols
---
# L'Éditeur web d'OSM iD

Permet l'édition avancée des données (point, polygone, ligne, etc) avec différentes sources de photos aériennes comme fond de carte.

Fonctionnalités:
* Ajouter/Modifier/Supprimer des <abbr title="Point d'intérêt">POI</abbr>s ;
* Ajouter un chemin ;
* Modifier des formes ;
* Modifier les propriétés des objets OSM existants ;
* Modifier les relations ;
* Voir/Modifier  les notes ;
* Travailler hors-ligne ;

<figure class="flex flex-col items-center margin-bottom-xs">
  <img src="/logo-osm.png" alt="OSM logo" width="80vh" class="margin-bottom-xs">
  <figcaption class="text-center text-sm">
 <a href="https://www.openstreetmap.org/edit">
  OSM iD
 </a>
  </figcaption>
</figure>

::right::

<div class="flex flex-col items-center gap-8 align-center">

<figure class="flex flex-col items-center">
  <img src="/OpenStreetMap_data_primitives_in_iD.png" alt="OpenStreetMap logo" width="50%">
  <figcaption class="text-center text-sm">
  <i>Primitives de données OSM (nœuds, tracés et relations)</i>
  <!-- By CactiStaccingCrane  - Own work, CC BY 4.0, https://commons.wikimedia.org/w/index.php?curid=127205850 -->
  </figcaption>
</figure>


<figure class="flex flex-col items-center">
  <img src="/osm-id-editor.png" alt="OSM logo" width="80%" >
  <figcaption class="text-center text-sm">
  <i>Aperçu de l'éditeur OSM iD sur Orx</i>
  </figcaption>
</figure>

</div>


---
layout: two-cols
---

# Panoramax

Commun numérique, collaboratif, libre et ouvert de vues immersives. <br>Alternative libre à Google Street View.

<!-- En 2020, le rachat par Meta, la maison-mère de Facebook, d’un des seuls vrais concurrents de Google Street View  -->

* Création: 2022 par l'IGN + OpenStreetMap France
* [Stats oct. 2026][panoramax-stats]
  * Contributeur-ces: ~2 700,
  * Kilomètres parcourus: ~1 100 000 km
  * Photos: 122 000 000
  * Instances: 🇫🇷 🇹🇼 🇧🇪 🇦🇷 🇨🇿 🇨🇦 🇭🇷 🇪🇸 🇳🇱 🏴󠁧󠁢󠁷󠁬󠁳󠁿 …

Usage: le SDIS repère les bornes incendies 🧑‍🚒

<!--
autres usage:
surveiller l'état de la voirie et du mobilier urbain.
vérifier le respect de la réglementation sur l'affichage publicitaire

Sources:
* Comment les usages de Panoramax se dessinent dans les territoires : https://www.banquedesterritoires.fr/
* Avec ses vues 3D, Val Parisis agglo ajuste sa carte au territoire (95) : https://www.banquedesterritoires.fr/experience/avec-ses-vues-3d-val-parisis-agglo-ajuste-sa-carte-au-territoire-95
* Panoramax, l'alternative libre et souveraine à Street View : https://www.europe1.fr/emissions/initiative-a-impact/panoramax-lalternative-libre-et-souveraine-a-street-view-4229690#about
*  Panoramax : le projet citoyen initié par l'Institut national de l'information géographique et forestière (IGN) pour ne plus dépendre de Google Street View : https://www.franceinfo.fr/replay-radio/nouveau-monde/panoramax-le-projet-citoyen-initie-par-l-institut-national-de-l-information-geographique-et-forestiere-ign-pour-ne-plus-dependre-de-google-street-view_6754240.html
 -->

  <figure class="flex flex-col items-center">
  <img src="/Panoramax_logo.svg" alt="Panoramax logo" width="80vh">
  <figcaption class="text-center text-sm">

  [Panoramax](https://panoramax.openstreetmap.fr)

  </figcaption>
  </figure>

::right::

<figure>
  <img src="/panoramax-preview.jpg" alt="panoramax preview">
  <figcaption class="text-center text-sm">

  Panoramax Preview

  </figcaption>
</figure>
<figure>
  <img src="/panoramax-orx.png" alt="panoramax orx">
  <figcaption class="text-center text-sm">

  Jardin partagé d'Orx

  </figcaption>
</figure>

[panoramax-stats]: https://panoramax.fr/stats/


---

# Fonctionnalités
  * Exploration
  * Calcul d'itinéraire
  * Affichage spécifique
  * Édition collaborative

---

# Cartopartie

 * Il s'agit d'un événement communautaire convivial,

<!-- ouvert à tous, et bien que certains puissent être des experts, les nouveaux venus sont toujours les bienvenus. C'est un très bon moyen d'en savoir plus sur le projet, et si vous n'avez jamais eu à récolter des informations pour mettre à jour OpenStreetMap, c'est une bonne façon d'apprendre à le faire. Cependant, certaines mapping parties peuvent être plus spécifiquement dédiées à la formation de nouveaux utilisateurs. Dans d'autres cas, les organisateurs peuvent fournir des récepteurs GPS de manière à jouer avec des gadgets (bien que l'utilisation de GPS ne soit pas nécessaire pour réaliser des ajouts sur OpenStreetMap). -->

* L'organisation d'une mapping party peut prendre diverses formes,

<!-- par exemple il peut simplement s'agir de se donner rendez-vous dans un bar après avoir cartographié une zone, mais en général un événement plus ambitieux peut nécessiter une rencontre préalable pour discuter des actions à mener et pour mettre en place des équipes de participants. Ensuite, il peut être utile de mettre à disposition des ordinateurs connectés à internet, pour réaliser l'import des données récoltées dans la journée, mais cela n'st pas indispensable (dans le cas de mapping parties plus simples, les participants repartent avec leurs données et les saisissent plus tard à leur rythme). -->

* Pour former des débutants il peut être utile de disposer d'au moins un ordinateur/téléphone,
<!-- pour pouvoir effectuer des démonstrations de saisie de données. Soyez prêts à utiliser les fonctionalités de saisie de JOSM en mode non connecté (téléchargez et enregistrez un fichier .osm au préalable) dans le cas où l'accès à internet ne serait pas possible. Si l'utilisation de GPS est prévue, il peut être pratique d'exporter les données de l'appareil pour les besoins de la démonstration, et parce qu'il s'agit d'une opération un peu complexe que des débutants pourraient ne pas arriver à réaliser seuls une fois de retour chez eux. Ainsi, vous pourrez mettre leur fichier en ligne pour eux. -->

* Une fois que les opérations de cartographie sont terminées, les participants partagent nourriture et boissons

<!-- les participants partagent nourriture et boissons, et prennent du plaisir à être ensemble. Après tout, il s'agit d'une fête ! En fait il n'est pas obligatoire de cartographier lors d'une mapping party. Parfois, il s'agit juste de faire la fête ! -->

Liste des [Événement en cours](https://wiki.openstreetmap.org/wiki/Current_events)

<figure class="flex flex-col items-center">
  <img src='/cartoparty-london.jpg' alt='Cartoparty à Londres' width='40%'>
  <figcaption class="text-center text-sm">
  Cartoparty à Londres
  </figcaption>
</figure>

