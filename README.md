Si vous voulez faire un blog en une seule langue, Dotclear le fait très bien par
défaut. Si vous voulez mélanger des articles dans une langue et dans une autre,
sans effort particulier de traduction, c'est également très bien géré. Si vous
voulez faire un blog avec des articles en deux langues, tous traduits
intégralement, vous pouvez (encore une fois par défaut) utiliser les capacités
multi-blogs de Dotclear et faire simplement deux blogs distincts.

Mais si vous voulez réellement faire du contenu bilingue (petit à petit ou tout
d'un coup), avec une réelle correspondance entre les articles, en en traduisant
certains mais pas tous, en permettant aux lecteurs bilingues de sauter d'une
traduction à l'autre, en mettant le maximum d'éléments dans la langue du
visiteur (la navigation tout d'abord, et si un article existe en plusieurs
versions, celle qui est préférée par le lecteur) tout en laissant accès au
reste, bref, pour faire un réel site multilingue, cette extension dctranslations
est pour vous.

Installation
============

Utilisez le fichier zippé fourni sur Dotaddict.org . La zone
d'administration est dans Blog > Traductions. La langue du blog doit être mise
à une valeur vide (c'est fait automatiquement lorsqu'on se rend sur les
paramètres du blog et qu'on les sauve ; il est important d'aller ensuite dans la
zone d'administration des traductions pour régler les langues visibles et la
langue de dernier recours). Le fonctionnement du plugin n'est pas correct tant
que le paramètre de langue n'est pas vide (on peut vérifier dans Extensions >
about:config).

Cette extension rajoute un panneau de commande pour choisir les langues
utilisables par les lecteurs pour naviguer sur le site, une interface pour
traduire les billets, les pages statiques ou des petits éléments de navigation.
La traduction des widgets ou des descriptions de catégories sont
laissées à d'autres extensions (mentionnées plus loin).

Ce plugin requiert l'usage du plugin stacker[3], en version au moins 0.4.

Cette extension redéfinissant des codes internes standards de Dotclear, il est
recommandé après l'avoir installé d'aller dans le tableau de bord et de faire
Extensions -> Maintenance -> Vider le cache des templates.

L'extension autolocale joue un rôle similaire à cette extension pour ce qui est
de présenter le blog en changeant la langue de navigation automatiquement selon
les préférences de l'utilisateur, mais aucun contrôle plus fin n'est permis (et
pas de traduction de billets). Pour un système multilingue complet, il est
recommandé d'installer la dernière version du plugin translatedwidgets[1], ainsi
que le plugin kezako[2].

Cette extension est sous la licence [4]GPL version 2.0.

Utilisation
===========

Simple utilisateur
------------------

Lorsque vous naviguez sur un blog muni de cette extension, Dotclear choisit
votre langue préférée (soit la dernière que vous aviez choisie manuellement,
soit celle qui est indiquée dans votre navigateur). En dernier recours, une
langue a été choisie par l'auteur du blog (si aucune de vos langues indiquées ne
convient).

Pour indiquer une langue à votre navigateur, il s'agit presque toujours d'une
préférence que vous pouvez modifier.

Lorsqu'un billet ou une page est disponible en plusieurs langues, la langue
préférée est présentée par défaut. Un widget (qui peut avoir été ajouté au site)
permet de choisir une autre traduction (si un locuteur multilingue désire voir
une autre version).

Simple auteur
-------------

Lorsque vous composez (ou éditez) une page ou un billet, apparaît en dessous de
la zone usuelle de saisie une zone pour saisir une nouvelle traduction à chaque
clic sur le bouton « nouvelle traduction », ainsi qu'une zone pour chaque
traduction déjà entrée. Chaque zone comporte cinq indications: titre, langue,
extrait, contenu, URL (la signification de chacun de ces cinq champs est la même
que pour la langue d'origine). La zone peut être masquée partiellement, laissant
alors apparaître seulement langue et titre.

Pour effacer une traduction déjà entrée, une case permet de le faire. La
traduction n'est pas effacée tant qu'une sauvegarde n'a pas été faite.

L'URL sera déterminée automatiquement à partir du titre traduit, sauf si elle
est modifiée manuellement. L'URL d'un billet est :
  * ...nomdusite/tpost/lang/url-de-la-traduction (billet traduit)
  * ...nomdusite/opost/lang/url-du-billet (billet dans la langue d'origine)
  * ...nomdusite/post/url-du-billet (prend automatiquement la langue préférée du
lecteur)

Chargé de traduction
--------------------

Parce que tout n'est pas parfait, il est parfois nécessaire d'entrer à la main
des éléments de traduction. Par exemple, la traduction des mots-clefs (tags),
des titres de widgets (lorsque ce n'est pas le titre par défaut), etc. Le
panneau d'administration (Blog > Traductions) permet d'entrer des traductions
qui, ajoutées aux traductions déjà livrées avec Dotclear, servent à traduire les
éléments visibles.

Le panneau d'administration comporte deux parties, une pour les réglages
multi-lingues du blog, et une autre sur les éléments de traduction. Le réglage
du blog se fait de deux façons extrêmement simples: il y a une liste de langages
autorisés (disponibles pour la navigation). La valeur par défaut est « en,fr »
ce qui autorise à naviguer en anglais ou en français (les deux langues les mieux
traduites pour Dotclear). La deuxième valeur est la langue de dernier recours
(qui doit être une des langues autorisées pour la navigation) qui est la langue
utilisée si un lecteur vient naviguer sur le site et que son navigateur
n'accepte aucune des langues autorisées. L'anglais est utilisé par défaut.

La deuxième partie sert à ajouter les éléments de traduction. Pour traduire un
élément, il suffit que le terme tel que rentré dans l'interface soit dans la
première colonne (« Chaîne »), et que la traduction correspondante soit la
colonne correspondant à la langue.

Par exemple, si j'ai un mot-clé « calendar », je peux ajouter sa traduction
française « agenda » dans la colonne « Français » et sa traduction allemande
dans la colonne « Deutsch ». Je laisse la traduction anglaise vide, puisqu'il
n'y a rien à traduire. J'aurais aussi pu choisir que le terme à rentrer était «
agenda » et le traduire respectivement en anglais et allemand par « calendar »
et « Kalendar ».

Pour ajouter une nouvelle entrée, il y a toujours une ligne vide dans la page 1
(les traductions sont présentées 16 par 16). Un petit menu à cliquer permet de
faire apparaître automatiquement des lignes pour tous les titres de catégories
et tous les titres de tags (la liste complète des termes sans traduction est
alors affichée aussi en dessous).

Pour supprimer une traduction, il faut laisser la première colonne « Chaîne » et
supprimer toutes les traductions. Une meilleure interface sera proposée dans
l'avenir.

L'effet est normalement visible immédiatement en zone publique.

Administrateur
--------------

Comme précisé plus haut, il faut s'assurer que toutes les extensions requises
sont présentes (et celles qui sont recommandées aussi), et que la langue du blog
est réglée sur la chaîne vide. Il faut aussi remplacer les widgets déjà présents
par les widgets équivalents traduits (de translatedwidgets). Par ailleurs, la
permission « editor » doit être conférée aux utilisateurs autorisés à s'occuper
de la traduction de l'interface (pas des billets; par exemple, traduire les
mots-clés et autres éléments graphiques du thème qui ne seraient pas traduits
par défaut -- titres de widgets différents du titre par défaut, par exemple).
Les administrateurs d'un blog n'ont pas besoin de cette permission.

Trois widgets sont disponibles et à ajouter aux endroits adéquats. Le premier,
actif uniquement sur une page de billet ou une page statique, permet de lister
toutes les traductions existantes du billet.

Le deuxième, « langue de navigation », permet de choisir sa langue de navigation
(elle devient alors la langue préférée pour ce site) sans passer par les
préférences de son navigateur (toutefois, il peut être indispensable de
recharger la page en « outrepassant » le mécanisme de cache, souvent par
shift-F5, ou en quittant son navigateur). Il est assez important de le mettre,
car beaucoup d'utilisateurs ne paramètrent pas correctement leur navigateur.

Le troisième, enfin, permet de remplacer le widget de choix des langues en
sélectionnant les articles par leur langue s'ils existent dans la langue en
question, pas seulement par leur langue d'origine. Il est appelé « Montrer
seulement les billets en ... ». L'autre widget est gardé pour des raisons
historiques, mais remplit moins de services (et s'appelle toujours « Langues du
blog »).

Références

   1. http://plugins.dotaddict.org/dc2/details/translatedwidgets
   2. http://plugins.dotaddict.org/dc2/details/kezako
   3. http://plugins.dotaddict.org/dc2/details/stacker
   4. http://www.gnu.org/licenses/gpl-2.0.html
