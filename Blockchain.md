#En finir avec la Blockchain
Qu'est-ce que “la blockchain” ? Souvent présentée comme "la technologie sous-jacente de Bitcoin", le terme est en fait bien postérieur à ce dernier, et n'est pas employé dans le fameux whitepaper de Satoshi Nakamoto publié en 2008. Quelques éléments semblent revenir constamment quand on essaie de la définir : tout le monde s’accorde sur le fait qu’il s’agit d’une “base de données” ou d’un “registre” de “transactions”, qu’elle est “décentralisée” ou en “pair-à-pair”, et aussi “sécurisée” et “immuable”. On ajoute parfois, à raison, qu’elle nécessite un “jeton”, c’est-à-dire une forme d’unité monétaire intrinsèque. 

Aujourd’hui, c’est surtout une solution à la recherche d’un problème, et une source de malentendu majeur sur ce qu’est Bitcoin, le problème qu’il résout, et pourquoi cela va (peut-être) changer le monde. 

Cet article constitue une tentative d’expliquer ce qu’est une blockchain en partant de la première et de la seule réellement opérationnelle à l’heure actuelle, celle de Bitcoin. Son objectif n’est pas de rentrer dans les subtilités techniques, mais de poser de façon suffisamment claire une définition simple, qui puisse servir de critère pour déterminer la pertinence d’une blockchain dans des cas d’usage précis. 

Bitcoin et le problème de la double-dépense

Revenons à l’archétype, la blockchain de Bitcoin. Quel est son rôle ? Pour son inventeur, Satoshi Nakamoto, il s’agit d’une solution au problème de la "double-dépense", c’est-à-dire le risque qu’une même unité monétaire puisse être dépensée deux fois de façon frauduleuse. 

Il s’agit d’un problème très ancien, et qui concerne en fait tous les paiements hors ceux effectués en cash. Prenons l’exemple du chèque de banque : si Bob fait un chèque à Alice pour régler une dette, comment cette dernière peut-elle être sûre qu'il ne s'agit pas de ce qu’on appelle communément un “chèque en bois”, et que Bob n'a pas déjà dépensé les mêmes euros en faisant un autre chèque à quelqu’un d’autre, Eve par exemple ? La solution traditionnelle à ce problème est le recours à un tiers, en l'occurrence une banque, qui supervise les comptes d’Alice, Bob et Eve, et est en mesure de voir que l'argent destiné à Alice a déjà été payé à Eve, et donc d'empêcher qu’il fasse l’objet d’une deuxième transaction. Le problème est exactement le même pour Visa, Paypal ou Alipay. 

Jusqu’à aujourd’hui, la seule solution pour éviter le recours à ce tiers validateur était l’utilisation d’espèces, ou cash, c’est-à-dire d’une forme d’argent qui a sa valeur en soi, et n’est pas une créance opposable à un tiers, comme le chèque ou la carte bancaire. Les espèces ont toutefois un défaut : elles doivent être remis de la main à la main, et ne permettent donc pas d’effectuer des paiements à distance. Elles peuvent également être malcommodes à stocker et à transporter. 

La raison d’être des banques et des intermédiaires de paiement est de proposer divers instruments fiduciaires, comme les chèques, les cartes bancaires, réseaux de paiement etc, qui permettent de contourner ces inconvénients. Cette intermédiation constitue donc un compromis entre sécurité et commodité : la monnaie fiduciaire est plus facile à utiliser et permet des paiements à longue distance, mais introduit de nouveaux risques inhérents à la présence d’un tiers de confiance, ce qu’on appelle des risques de contrepartie.

En apportant une solution à ce problème de double-dépense qui permet de se passer de tiers de confiance, Bitcoin est donc la première forme de monnaie à cumuler la qualité principale du cash, qui est de permettre un règlement immédiat d’une dette sans tiers validateur, et les avantages des instruments fiduciaires en termes de distance et de rapidité de paiement. 

La blockchain de Bitcoin

Nous avons donc posé que la blockchain de Bitcoin était une solution au problème de la double dépense qui permettait de se passer de tiers validateur, mais comment réalise-t-elle ce tour de force ? 

Ce qu’on appelle une “blockchain” est fondamentalement un système distribué d'enregistrement et de validation d'informations. Le coup de génie de Satoshi Nakamoto est d’inverser le postulat de base des réseaux de paiement traditionnels, qui repose sur le secret et la transmission confidentielle d’informations sensibles pour garantir la sécurité des transactions. Dans Bitcoin, au contraire, tout est public et transparent : les balances, l’historique des transactions et les transactions elles-mêmes. 

Au lieu de reposer sur une entité unique seule à pouvoir contrôler les transactions, tous les participants vont vérifier toutes les transactions eux-mêmes. En faisant tourner le code de Bitcoin sur un ordinateur et en se connectant au réseau, Eve n’a besoin de personne pour s’assurer que le bitcoin que Bob va lui envoyer est bien disponible à l'adresse indiqué par ce dernier, et n'a pas déjà été utilisé dans une transaction destinée à Alice. 

Bien sûr, cela ne peut fonctionner que si Bob n'a pas la possibilité de falsifier la blockchain, par exemple en fabriquant de la fausse monnaie qu'il pourra ensuite utiliser pour payer Eve et Alice.

Il y a donc deux opérations à considérer séparément : l’enregistrement de la balance de Bob et la validation de cette balance. Nous venons de voir que cette deuxième opération était effectuée indépendamment par les participants du réseau, mais qu’en est-il de la première ? Comment sont fixées les règles qui permettent à Alice de déterminer qu’un enregistrement de la balance de Bob dans la blockchain est légitime ou non ? 

Cela nous amène à la question fondamentale pour évaluer la sécurité d'une blockchain : qui peut y écrire, et à quelles conditions ? 

En effet, si Bob peut y inscrire une transaction frauduleuse dans la blockchain et la faire passer pour valide, il n'aura aucune difficulté à la corrompre pour son propre bénéfice. L’intégrité de l’information visible dans la blockchain, et donc sa valeur, ne dépendent in fine que des règles qui déterminent à quelles conditions un acteur est autorisé à y écrire, autrement dit de son protocole de validation. 

Ce protocole permet donc aux utilisateurs/validateurs de contrôler que l’enregistrement d’une information dans la blockchain respecte les règles. Dans le cas de Bitcoin, trois mécanismes garantissent que les données inscrites dans la blockchain sont correctes : 
1. La preuve de travail (proof of work) : afin d’obtenir le droit d’ajouter un bloc dans la blockchain, il faut être le premier à résoudre un problème mathématique très difficile, qui nécessite beaucoup de puissance de calcul, et donc de l’énergie. Pouvoir écrire dans la blockchain de Bitcoin n’est pas gratuit, et est même aujourd’hui très cher. 
2. La récompense : les acteurs qui consomment de l’énergie pour écrire dans la blockchain, les “mineurs”, sont récompensés par la création de nouveaux bitcoins. Ce point est capital, car ainsi les mineurs ont un réel intérêt à maintenir l’intégrité du réseau : en cas de malversations de leur part, la confiance des utilisateurs déclinerait rapidement et leur récompense perdrait toute valeur.  
3. La validation : valider un bloc est aussi simple pour un utilisateur que le créer est coûteux pour un mineur. Ainsi, si un participant du réseau diffuse un bloc qui ne respecte pas les « règles du jeu » (exemple réel : des mineurs s’allouent plus de bitcoins en récompense que ce qui est prévu dans le code), ce dernier sera rejeté par tous les participants du réseau, quand bien même la preuve de travail serait valide. Le mineur malhonnête aura donc consommé l’énergie de la preuve de travail en pure perte.

Contrairement à la définition que nous avons rappelé plus haut, la blockchain n’a donc, en soi, rien d’immuable. En effet, si en vertu du protocole, un acteur a plus de pouvoir d’enregistrement que tous les autres réunis, absolument rien n'empêche de falsifier les événements enregistrés dans la blockchain, par exemple d’inverser des transactions à son propre profit. 

Cette possibilité a été envisagée en théorie dès le White Paper de Satoshi Nakamoto sous le nom « d’attaque 51 % », et on trouve également des cas de "réécriture" de blockchain dans la réalité : par exemple, Vitalik Buterin, le créateur d’Ethereum, a décidé de modifier la blockchain suite au hack de la DAO en 2016 afin d’effacer les gains du hacker. Dans cette configuration, une cryptomonnaie présente donc les mêmes enjeux politiques et les mêmes risques de manipulation qu’une monnaie fiat, et l’utilisation d’une blockchain n’est donc en rien une garantie d’inviolabilité. 

Si Bitcoin est révolutionnaire, cela n'a pas tant à voir avec la blockchain en tant que telle, mais bien plutôt avec les puissants mécanismes d'incitation que Satoshi Nakamoto a su trouver pour amener les utilisateurs à protéger l'intégrité du réseau. La dimension technologique est en effet loin d'être primordiale dans Bitcoin, dont l'innovation est avant tout de proposer un système anarchique dans lequel se produit spontanément un alignement des objectifs de différents acteurs, sans qu’aucun ne puisse le remettre en cause. Ce mécanisme est si puissant que, parti de rien il y a moins de 10 ans, Bitcoin a réussi à survivre et à prospérer en dépit des nombreuses attaques dont il est sans cesse l’objet.