---
title: Site LoWeb
---
## Low-Web

### Introduction

Internet est un grand réseau de câbles reliant des ordinateurs entre eux, chaque interaction que l'on réalise sur le net est un flux de données envoyé à travers ces câbles vers un autre ordinateur qui interprète le signal pour avoir un retour.

Dans un monde qui dépend de plus en plus d'internet, où les usages sont de plus en plus libres et les outils se multiplient, se pose la question du coût d'une telle technologie.

Les billions d'octets de données qui transitent à travers les baies serveurs consomment de l’électricité pour le refroidissement et le traitement tandis que l'augmentation de la demande créée des pénuries de matières premières.

En effet depuis des années, les consommations à travers les sites internet ont grandement augmenté. L'arrivée de plateforme comme Netflix (qui représente 15% de la consommation mondiale de data à lui seul) et les framework tels que REACT qui font fi de leur impact écologique nous ont habitué à un usage débridé des services proposés.
Ajoutons à cela les autres évolutions technologiques qui interfèrent sur la consommation du web :

* Images de meilleure qualité, donc plus lourdes ;
* Animations graphiques consommatrices de ressources ;
* Intégration vidéo de plus en plus fréquente ;
* Coût d'accès au matériel informatique réduit.

Ce florilège d'évolutions technologiques n'a pas que du bon, une étude sur les consommations énergétiques de 3 milliards d'usagers sur une année nous a permis d'avoir des statistiques. L’empreinte annuelle, au niveau mondial, serait de :

* 1 037 TWh d’énergie, soit 40 centrales nucléaires ou 140 millions de français pendant 1 an ;
* 608 millions de tonnes de gaz à effet de serre, soit l’équivalent de 86 millions de français(e)s ;
* 8,7 milliards de m3 d’eau, soit la consommation annuelle de 160 millions de français.

> « Ce qui coûte très cher à l’environnement aujourd’hui, c’est le flux de données, beaucoup plus que le stock  »
> > -Bela Loto, formatrice-consultante et fondatrice de la Maison de l’informatique responsable.

Face à ces problématiques, des intéressés ont cherché des moyens de lutter contre ces chiffres alarmants. Les usagers représentant 50% des émissions carbone d'internet, et pourtant nous n'avons que peu de contrôle sur la manière d'accéder au web ou ce que l'on peut y trouver.

Le low web est une initiative des usagers du web qui comprennent les limites techniques qu'imposent les nouvelles technologies déployées sur leurs sites afin de réduire cet impact, sans rogner sur le confort de tout un chacun lorsque l'on utilise internet.

Cette solution s'illustre sous le nom de "Low Web" en référence au Low Tech, combiné au web, et correspond à toute pratique visant à l'économie de ressources en ligne.

Cet article vise à vous présenter le Low-Web, définir ses avantages et limites afin de déterminer si c'est une technologie fiable pour répondre aux problématiques d'aujourd'hui.

### Low-Web, Qu'est-ce ?

Le low web (Fusion de Low-Tech et Web) est un ensemble de pratiques qui permettent d'alléger une page web au maximum.
Elles concernent les développeurs qui, lors de la mise en place du site internet, cherchent à créer un site léger, rapide, facilement réplicable.
On y retrouve les conditions suivantes pour correspondre a l'idée d'un site low-web:

* Le site ne doit être construit qu'à travers les langages basiques du web : HTML et CSS. Les scripts coté client ou serveur sont à éviter le plus possible.
* Un code propre et épuré, avec une architecture structurée sans page inutile.
* Un design simple, sans animations, avec un contenu accessible facilement.
* Garder un éditeur de site Web (CMS) qui respecte ces contraintes pour votre site.
* Un minimum d'image, et sinon les alléger pour ne pas faire charger d'image haute définition à l'usager. Favoriser les images Svg.

Ainsi un site low tech n'est pas différent d'un site standard, il est simplement optimisé et créé avec ces pratiques et dépossédé de ses fioritures.

Exemple de site Low-Web : Low <- Tech Magazine:

![LowTechMag](/images/uploads/image-1621431870221.png "Low-Tech_Magazine")

*Le site au dessus est un modèle pour le low-web: en plus d'avoir une page qui pèse seulement 584.15Ko, toutes les images sont traitées et décolorées, les textes sont en police "par défaut" du navigateur, leur site est statique... Le magazine s'est donné la peine de réfléchir a chaque point de son site pour économiser un maximum de ressource.*

Toutes ces pratiques ne semblent pas avoir d'impact pour un utilisateur et semblent même retirer certaines fonctionnalités ajoutées par les dernières évolutions technologiques.

En fait, une page issue des pratiques low web est 5 à 10 fois plus légère qu'une page standard, et donc se charge proportionnellement plus vite pour l'usager. De plus, le fait d'utiliser un code clair et simple favorise la compatibilité entre les navigateurs ainsi que la maintenance.

Le concept s’oppose au high-tech et peut faire appel à des solutions techniques tombées (plus ou moins récemment) en désuétude, mais remises au goût du jour à travers de nouveaux outils.

Par exemple, il existe des générateurs de sites statiques. Ces derniers ont, par leur structure et leur fonctionnement, intégrés par défaut les pratiques low-tech et il suffit de quelques attentions pour que le site généré soit tout a fait acceptable par les normes low-web.

Pour prendre un exemple, le moteur de génération de site Hugo, développé en Go, communautaire et open-source, est un outil qui permet de gérer son contenu en fichiers écrits en MarkDown et l'archiver selon une architecture définie soi-même puis de mettre en place ces textes en fichiers HTML grâce a des modèles.
Tout ces fichiers sont analysés pour créer un site statique.

Lorsque vous parcourez un site statique, votre navigateur demande à accéder à un fichier HTML sur le serveur dudit site, le serveur lui renvoie, le navigateur le lit, la page s’affiche. Ainsi, pour 1, 100, 1000 visiteurs, le fichier n’a été généré qu’1 fois et se contente d'être consulté.

A l'inverse, un site dynamique demande au serveur de générer à la demande la ressource, en allant récupérer dans les bases de données les textes, images et autres contenus souhaités. Il les traite / formate, génère la page, la renvoie, le navigateur la lit, la page s’affiche. Pour 1, 100, 1000 visiteurs, elle aura donc été généré 1, 100 ou 1000 fois.

Et malgré son appellation péjorative par rapport aux sites dynamiques, un site statique peut garder tout d'un site moderne. La preuve avec ce site, uniquement réalisé en CSS et HTML.

Ici, on voit que le site se permet d'afficher des images et d'utiliser une police spéciale.
Ces images sont, tout comme celles du Low<-Tech Magazine, réduites en taille, en qualité, décolorés afin de les rendre plus légère et rester compréhensibles.

La police va être téléchargée à la première arrivée sur le site, elle est ensuite stockée dans le cache du navigateur et ne sera plus chargée aux prochaines visites du site.

Il existe d'autres moteurs comme Hugo : Jekyll et Pelican pour ne citer que les plus connus.

### Adapté à tout type de projet ?

Les pratiques Low-Web n'ont pas cette prétention.

En effet, malgré tout les bienfaits de ce système alternatif, il reste certains cas qu'il ne peux pas traiter.

Par exemple, beaucoup de site internets croisent des sources de données qui sont stockées à travers des bases de données qui dépendent d'acteurs multiples. On ne peut pas accéder à la base de données et donc aux fonctionnalités du site en son intégralité si on s'en tient au site statique, on doit insérer des scripts et des requêtes dans la page.

Ou encore si votre site repose sur des données fournies entièrement par l'usager, il n'est pas possible de traiter ces données sans un script.

Enfin, les entreprises de communication et graphistes rechignent beaucoup a l'idée de simplifier les sites, de les rendre plus faciles d'accès et d'utiliser le moins de fonctions possibles.
En effet, la première crainte est portée sur la concurrence à qui cela laisse le champ libre d'exploiter ces artifices.
D'autres ne veulent pas se séparer des analyses, des publicités et des cookies.

Il y a aussi la barrière technique. En effet on entre aujourd'hui dans un essor des site-builders, logiciels a destination des usagers lambda pour mettre en place leur site marchand "basique". Cela accentue une mystique autour du développement, du web et de l'informatique en générale qui pousse les gens à se désintéresser du moyen au profit du but.

En effet pour comprendre l’intérêt du low-web il faut avoir connaissance de la technique derrière un site web. De plus, ces pratiques, plus récentes, sont moins lissées et, comme dit précédemment, ne prodiguent pas le même confort dû aux sacrifices faits pour obtenir un site low-tech.

Mais la principale raison du manque de popularité des site low-web et statiques vient surtout du manque de visibilité et de connaissance du grand public et des web-designers.

### Peut-on s’appuyer sur ces pratiques pour le web de demain ?

On pense souvent à un futur qui tend vers sa destruction pour l'humanité, et pourtant voilà un exemple d'auto-préservation d'une technologie et la mise en place des moyens nécessaires pour un "passage" vers un web moins lourd, plus facile a gérer.

Plutôt que s'imposer comme nouvelle norme, beaucoup de partisans du low-tech pensent que cette solution se présentera d'elle-même lors d’éventuelles limites d'accès à l’énergie et/ou une censure plus pesante.

Un site statique, low-tech, se détache des systèmes classiques pour le stockage des données.
Le fait de manipuler des fichiers textes simples, sans requête, IDs et autre éléments relatifs aux bases de données, rend les données facile à exporter, à cloner, à filtrer, à traiter. Cela rend le développement et l'intégration continue plus accessibles et simples à gérer.

Dans une ère de consommateurs de plus en plus éco-responsables, où l'information est accessible comme jamais et une nouvelle habitude peut se répandre comme une trainée de poudre, l'existence des pratiques low-web complémente le kit internet.

Il ne manque peut être que quelques memes sur le low-web pour que la pratique se popularise, en espérant qu'il ne faille pas attendre un crise mondiale pour que les développeurs adoptent ces pratiques, même partiellement.

![](/images/uploads/maybe-low-tech-is-the-new-high-tech.jpg)


Ce type de pratique est un exemple d'une communauté qui s'empare d'un problème et développe une solution. C'est un exemple pour les industries qui cherchent à faire de l'éco-marketing plutôt que de l'écologie.

Sources:

* [https://usbeketrica.com](https://usbeketrica.com)
* [https://lowtechlab.org/fr/actualites-blog/faire-un-site-low-tech](https://lowtechlab.org/fr/actualites-blog/faire-un-site-low-tech)
* [https://www.greenit.fr/2015/05/12/quelle-est-l-empreinte-environnementale-du-web/](https://www.greenit.fr/2015/05/12/quelle-est-l-empreinte-environnementale-du-web)

Exemples de site low-web :

Types blog :

* [https://www.pikselkraft.com/en/](https://www.pikselkraft.com/en/)
* [https://ecoweb.noema.design/index.html](https://ecoweb.noema.design/index.html)
* [https://low.plopcom.fr/](https://low.plopcom.fr)
* [https://lafun.fr/](https://lafun.fr/)
* [https://lowimpact.organicbasics.com/eur](https://lowimpact.organicbasics.com/eur)

Types applicatifs :

* [https://godottutorials.com/courses]( https://godottutorials.com/courses)
* [https://www.bypasscensorship.org/#tools]( https://www.bypasscensorship.org/#tools)

(auteur de l'article : martin gasque)