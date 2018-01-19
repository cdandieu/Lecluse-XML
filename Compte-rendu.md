# Quel est l'intérêt et le fonctionnement d'une chaîne XML ?
## Découverte d'un workflow complexe et abouti avec ENS Éditions


*Résumé :* Sophie Lecluse, éditrice chez **ENS Editions**, est venue ce mercredi 13 décembre 2017 nous présenter la chaîne de publication mise en place au sein de sa structure éditoriale. Le thème de la séance était donc assez technique, en voici la restitution synthétique.

*Mots-clés :* Publication scientifique ; édition numérique ; XML ; TEI ; chaîne de publication ; édition universitaire ; standards ; communauté scientifique


### Présentation d’ENS Éditions

ENS Éditions est une maison d’édition universitaire publique, qui publie de l’édition scientifique, environ une vingtaine d’ouvrages par an, en papier et en numérique. Les publications sont de domaines variés, il s’agit de textes complexes, aux structures élaborées contenant des notes, des références bibliographiques, des liens hypertextes, qui entraînent un autre usage et un autre mode de lecture, propre au domaine de la recherche scientifique. La particularité de l’édition scientifique rend difficile une publication exclusivement numérique, car le papier semble encore avoir une valeur de validation de l’information. Un des objectifs d’ENS Éditions est donc de proposer la même expertise en numérique que pour le papier.

A cette première caractéristique s’en ajoute une deuxième : leur statut d’éditeur publique leur donne le devoir de diffuser les résultats de la recherche aux chercheurs à l’international.
L’enjeu pour ENS Éditions est de trouver un équilibre entre leur mission, c’est-à-dire diffuser au plus grand nombre et le plus possible en format libre, et leurs contraintes économiques : ils ne sont pas subventionnés, il est donc impératif de vendre des livres pour pouvoir en éditer de nouveaux. Autrement dit la question est : *comment financer l’Open Access tout en garantissant un contenu de qualité ?*

Une seconde *contrainte* à prendre en considération est la Loi DADVSI de 2006, une loi relative aux droits d’auteur, aux droits voisins et à l’exception handicap pour l’accessibilité. Il le prenne en compte depuis deux ans et cela a un impact fort sur leur activité.

### Le XML : eXtensible Markup Langage

C’est un langage dit “de balisage”, de codage de contenus, dont l’objectif est l’échange entre systèmes informatiques, le transfert des données et de leurs structures. C’est un standard universel et multilingue d’échanges d’informations. Appliqué aux documents textuels, il permet d’identifier de façon logique la structure et l’organisation de l’information textuelle.  
Ce choix de langage a donc deux avantages principaux : il offre une grande structuration de texte et il est massivement utilisé par la communauté scientifique (ce qui lui assure un peu plus de pérennité et d’interopérabilité qu’un système *maison*).  
Par ailleurs, pour augmenter encore la qualité structurelle de l’encodage et assurer sa pérennité, ce langage a été couplé à l’initiative [TEI](http://books.openedition.org/oep/1298?lang=fr) (Text Encoding Initiative), qui a pour vocation d’encadrer, orienter et unifier les systèmes d’encodage des travaux scientifiques dans le domaine des humanités numériques.

### Bref historique de la chaîne

![shéma historique de la chaîne](https://lh3.googleusercontent.com/H2fWtO17amcnBN3DsXkfOuojLJzB8BwEKz_m8oRzKXzOA2-UPE6Dqi8kvDO7E1cs1lxY6mX3-Wes=s0 "schema-historique.png")

La chaîne actuelle se compose actuellement de deux types d'éléments :

+ les technologies et standards : ils utilisent l’unicode, le langage XML, [DTD](https://fr.wikipedia.org/wiki/Document_type_definition) (Document Type Definition)-TEI, dont la fonction principale est de structurer les documents.
+ les flux : qui vont permettre de lier et générer le passage d’un fichier à un autre et automatiser certaines fonctionnalités dans la production de cette chaîne. Ce sont les scripts et les feuilles de transformation [XSLT](https://fr.wikipedia.org/wiki/Extensible_Stylesheet_Language_Transformations) (eXtensible Stylesheet Language Transformations). Le logiciel XML Editor est par ailleurs utilisé pour générer les différents supports de sortie.

Le principe de cette chaîne est donc de générer plusieurs supports à partir d’un unique format pivot. Celle-ci pourrait être schématisée de cette manière (Schéma de D. Roux) :

![schéma de la chaîne xml](https://lh3.googleusercontent.com/-NObAV_CmO7Q/WkOpZ_XN3RI/AAAAAAAAAMM/OD0RC1nhQl081YsFIstip-kEbm8gouchQCLcBGAs/s0/schema-chaine.png "schema-chaine.png")

### Limites et avantages de la chaîne

Grâce à cette chaîne XML, c’est la chaîne de production qui a été rationalisée, en permettant une intervention éditoriale unique pour la publication de plusieurs supports. Les contenus sont désormais balisés, consolidés, pérennes et interopérables. Cette solution permet également de garantir l’équilibre financier d’ENS Éditions puisqu’elle ne nécessite pas d’intervenants externes. La structure est totalement **autonome**, et propose un contenu en open source, tout en réalisant un gain financier indispensable à son bon fonctionnement. La diffusion de publications de qualité, standardisées et accessibles est ainsi garantie dans les meilleures conditions possibles dans la communauté des chercheurs. ENS Éditions remplit ainsi ses fonctions avec ses contraintes propres. Un second avantage de la chaîne est l’accessibilité, puisqu’ils produisent des contenus nativement structurés, les fichiers XML permettent par exemple de générer des fichiers **Daisy**.

Quelques limites subsistent tout de même, notamment le fait que tous les livres ne puissent pas intégrer complètement la chaîne jusqu’à l’OEB (Open Edition Book), par exemple les *Précis de structure syllabique*. Une telle organisation demande également une expertise en amont de la fabrication de l’objet éditorial. Ce qui induit une nouvelle contrainte, la nécessité d’évaluer correctement le ratio temps / plus value éditoriale. Il ne faut pas rentrer dans un système qui ne serait pas rentable, une fois de plus il faut trouver un équilibre entre qualité et faisabilité.
