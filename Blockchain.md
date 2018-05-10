# En finir avec la Blockchain

Qu'est-ce que “la blockchain” ? Souvent présentée comme "la technologie sous-jacente de Bitcoin", le terme est en fait bien postérieur à ce dernier. Il n'est pas employé dans le fameux whitepaper de Satoshi Nakamoto publié en 2008, ni dans les premiers échanges au sein de la communauté.  

Bien qu'il n'y en ait pas de définition suffisamment claire, du moins à notre sens, quelques éléments reviennent constamment : 
* il s’agit d’une “base de données”, ou parfois d’un “registre” de “transactions”, 
* elle est “décentralisée” ou en “pair-à-pair”, 
* elle est aussi “sécurisée” et “immuable”. 
* On ajoute parfois, à raison, qu’elle nécessite un “jeton” pour fonctionner, c’est-à-dire une forme d’unité monétaire intrinsèque. 

Aujourd’hui, c’est surtout une solution à la recherche d’un problème. Plus grave, c'est aussi une source de malentendu majeur sur ce qu’est Bitcoin, le problème qu’il résout, et pourquoi cela va (peut-être) changer le monde. 

Cet article constitue une tentative d’expliquer ce qu’est une blockchain en partant de la première et de la seule réellement opérationnelle à l’heure actuelle, celle de Bitcoin. Son objectif n’est pas de rentrer dans les subtilités techniques, mais de poser de façon suffisamment claire une définition simple, qui puisse servir de critère pour déterminer la pertinence d’une blockchain dans des cas d’usage précis. 

## Bitcoin et le problème de la double-dépense

Revenons à l’archétype, la blockchain de Bitcoin. Pour son inventeur, Satoshi Nakamoto, il s’agit d’une solution au problème de la "double-dépense", c’est-à-dire le risque qu’une même unité monétaire puisse être dépensée deux fois de façon frauduleuse. 

Il s’agit d’un problème très ancien, et qui concerne en fait la plupart des modes de paiement. Prenons l’exemple du chèque de banque : si Bob fait un chèque à Alice pour régler une dette, comment cette dernière peut-elle être sûre qu'il ne s'agit pas de ce qu’on appelle communément un “chèque en bois”, et que Bob n'a pas déjà dépensé les mêmes euros en faisant un autre chèque à quelqu’un d’autre, Eve par exemple ? La solution traditionnelle à ce problème est le recours à un tiers, en l'occurrence une banque, qui supervise les comptes d’Alice, Bob et Eve, et est en mesure de voir que l'argent destiné à Alice a déjà été payé à Eve, et donc d'empêcher qu’il fasse l’objet d’une deuxième transaction. Le problème est exactement le même pour Visa, Paypal ou Alipay. 

Jusqu’à aujourd’hui, la seule solution pour éviter le recours à ce tiers validateur était l’utilisation d’espèces, ou _cash_, c’est-à-dire d’une forme d’argent qui a sa valeur en soi, et n’est pas une créance opposable à un tiers, comme le chèque ou la carte bancaire. Les espèces ont toutefois un défaut : elles doivent être remises de la main à la main, et ne permettent donc pas d’effectuer des paiements à distance. Elles peuvent également être malcommodes à stocker et à transporter. 

La raison d’être des banques et des intermédiaires de paiement est de proposer divers instruments fiduciaires, comme les chèques, les cartes bancaires, réseaux de paiement etc, qui permettent de contourner ces inconvénients. Cette intermédiation constitue donc un compromis entre sécurité et commodité : la monnaie fiduciaire est plus facile à utiliser et permet des paiements à longue distance, mais introduit de nouveaux risques inhérents à la présence d’un tiers de confiance, ce qu’on appelle des risques de contrepartie.

En apportant une solution à ce problème de double-dépense qui permet de se passer de tiers de confiance, Bitcoin est donc la première forme de monnaie à cumuler la qualité principale des espèces, qui est de permettre un règlement immédiat d’une dette sans tiers validateur, et les avantages des instruments fiduciaires, le paiement entre des acteurs éloignés et qui ne se connaissent pas. 

## La blockchain de Bitcoin

Nous avons donc posé que la blockchain de Bitcoin était une solution au problème de la double dépense qui permettait de se passer de tiers validateur, mais comment est réalisé ce tour de force ? 

Ce qu’on appelle une “blockchain” est fondamentalement un système distribué d'enregistrement et de validation d'informations. Le coup de génie de Satoshi Nakamoto est d’inverser le postulat de base des réseaux de paiement traditionnels, qui repose sur le secret et la transmission confidentielle d’informations sensibles pour garantir la sécurité des transactions. Dans Bitcoin, au contraire, tout est public et transparent : les balances, l’historique des transactions et les transactions elles-mêmes. 

Au lieu de reposer sur une entité unique seule à pouvoir contrôler les transactions, tous les participants vont vérifier toutes les transactions eux-mêmes. En faisant tourner le code de Bitcoin sur un ordinateur connecté au réseau, Eve n’a besoin de personne pour s’assurer que le bitcoin que Bob va lui envoyer est bien disponible à l'adresse indiqué par ce dernier, et n'a pas déjà été utilisé dans une transaction destinée à Alice. 

Il y a donc deux opérations à considérer séparément : 
* l’enregistrement de la balance de Bob dans la blockchain,
* la validation de cet enregistrement, qui permet de s'assurer qu'elle n'est pas frauduleuse. 
Pour que chaque participant du réseau puisse valider indépendamment un enregistrement dans la blockchain, il est donc nécessaire que ces participants partagent la même définition de ce qu'est une transaction valide, sans quoi le réseau se fractionnerait, puisqu'une même transation serait considérée valide par certains et pas par d'autres.
Pour résumer, en déléguant la validation des enregistrements indépendamment à chaque acteur du réseau, il est également nécessaire d'imposer un protocole de validation très claire pour permettre à un si grand nombre d'acteurs indépendants d'arriver à un _consensus_ sur une version et une seule du registre. 

## Le protocole de validation 

En effet, si Bob peut y inscrire une transaction frauduleuse dans la blockchain et la faire passer pour valide, il n'aura aucune difficulté à la corrompre pour son propre bénéfice. C'est pourquoi il existe des règles très strictes pour définir à quelles conditions Bob a le droit d'écrire dans la blockchain, et ce qu'il a le droit d'y écrire. 

Il est donc nécessaire d'avoir un protocole commun qui permette aux utilisateurs/validateurs de contrôler que l’enregistrement d’une information dans la blockchain respecte les règles. Dans le cas de Bitcoin, outre le système de _hash_ dont nous reparlerons plus tard, trois mécanismes garantissent que les données inscrites dans la blockchain sont correctes : 
1. La preuve de travail (_proof of work_) : afin d’obtenir le droit d’ajouter un bloc dans la blockchain, il faut être le premier à résoudre un problème mathématique très difficile, qui nécessite beaucoup de puissance de calcul, et donc de l’énergie. Pouvoir écrire dans la blockchain de Bitcoin n’est pas gratuit, et est même aujourd’hui très cher. 
2. La récompense : les acteurs qui consomment de l’énergie pour écrire dans la blockchain, les “mineurs”, sont récompensés par la création de nouveaux bitcoins. Ainsi les mineurs ont un réel intérêt à maintenir l’intégrité du réseau : en cas de malversations de leur part, la confiance des utilisateurs déclinerait rapidement et leurs coûteux investissements en énergie et matériel de minage spécialisé perdraient toute valeur.
3. La validation : valider un bloc est aussi simple pour un utilisateur que le créer est coûteux pour un mineur. Ainsi, si un participant du réseau diffuse un bloc qui ne respecte pas les « règles du jeu » (exemple réel : des mineurs s’allouent plus de bitcoins en récompense que ce qui est prévu dans le code), ce dernier sera rejeté par tous les participants du réseau, quand bien même la preuve de travail serait valide. Le mineur malhonnête aura donc consommé l’énergie de la preuve de travail en pure perte.

## Les attaques contre la blockchain

Contrairement à la définition que nous avons rappelée plus haut, la blockchain n’a donc, en soi, rien d’immuable. En effet, si un seul acteur peut apporter plus de preuve de travail que tous les autres réunis, il lui est possible de réaliser des enregistrements frauduleux. 

Cette possibilité a été envisagée de façon théorique dès le White Paper de Satoshi Nakamoto sous le nom « d’attaque 51 % », c'est-à-dire qu'un seul acteur possède plus de 51% de la puissance de calcul du réseau. 

Mais ce n'est pas qu'un cas d'école théorique, on trouve également des cas de "réécriture" de blockchain dans la réalité : par exemple, Vitalik Buterin, le créateur d’Ethereum, a décidé de modifier cette blockchain suite au hack de la DAO en 2016 afin d’effacer les gains du hacker. 

Il est toutefois important de noter que l'attaque 51% ne porte pas sur les règles de validité des transactions, mais ne fait qu'annuler ou bloquer des transactions autrement valides. Tant qu'un nombre suffisant d'utilisateurs est présent sur le réseau pour valider les blocs générés par les mineurs, ces derniers n'ont pas le pouvoir d'imposer des changements dans le protocole ou de réaliser des transactions non conformes à ce protocole.

Dans le cas contraire, une cryptomonnaie présente les mêmes enjeux politiques et les mêmes risques de manipulation que n'importe quel autre système centralisé. Sur une blockchain où seule une poignée d'acteurs détient le pouvoir de valider les transactions, un changement de protocole est une affaire triviale. L’utilisation d’une blockchain n’est absolument pas, _en soi_, une garantie d’inviolabilité, et peut être victime de deux types d'attaques :
* si des clients validateurs ne sont pas largement disséminés sur le réseau, le protocole peut être facilement modifié par collusion d'une poignée d'acteurs majoritaires. 
* Si le minage n'est pas largement décentralisé aussi bien du point de vue des acteurs en présence que de leur emplacement géographique, le risque est celui d'une paralysie du réseau ou d'une censure systématique de certaines transactions par exemple.  

## Conclusion : une proposition de définition de la _Blockchain_

Nous pouvons donner une première définition de ce qu'est une blockchain :
* son objectif est d'éliminer _simultanément_ les risques de contrepartie et de double-dépense.
* pour atteindre son objectif, elle repose sur la réalisation d'un audit exhaustif des transactions par tous les participants du réseau.
* la coordination entre un grand nombre de participants indépendants est atteinte grâce à un protocole, règles déterminant strictement ce qui est valide et ce qui ne l'est pas, ce qui permet d'atteindre un consensus sur l'état du registre.
* la stabilité des règles du protocole est garantie par le nombre et l'autonomie des participants validant les transactions. Si ces derniers sont trop peu nombreux et/ou dépendants d'une entité unique, il est alors trivial de changer les règles du jeu pour ceux qui détiennent la puissance de calcul nécessaire à l'écriture de nouveaux blocs d'informations.
* Enfin, la réalisation de son objet implique des compromis, car pour être efficace elle nécessite une consommation importante de ressources : mémoire, puissance de calcul et bande-passante. Ce point sera traité ultérieurement. 
