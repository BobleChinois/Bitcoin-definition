# Apologie des petits blocs

## Pourquoi cet article

Cet article ne s'adresse pas aux vieux briscards qui ont pris part aux débats de ces dernières années, ils connaissent déjà les arguments développés ici sur le bout des doigts. Non, cet article est destiné avant tout aux nouveaux venus dans le monde _merveilleux_ de Bitcoin, à ceux qui ne sont pas encore là mais nous rejoindront dans les années à venir, et aussi aux simples curieux qui ne jouent pas (encore ?) leur peau sur Bitcoin mais qui veulent en savoir plus. 

Un tel article m'a semblé nécessaire pour plusieurs raisons :
* L'information disponible à ce sujet est éparpillée sur des dizaines d'articles, de posts de blogs, de forums, de tweets, de reddit et de vidéos sur ces 3 dernières années, et on ne peut pas raisonnablement attendre de tous les néophytes qu'ils se paluchent des centaines d'heures de lecture et de vidéos simplement pour avoir une idée claire des enjeux de ce débat et de son issue.
* Cela est d'autant plus important que la bulle de 2017 a suscité de façon compréhensible un vif intérêt au-delà des cercles d'amateurs endurcis. On a vu arriver ces derniers mois une nouvelle vague d'utilisateurs, d'investisseurs ou de simples curieux qui, évidemment, ne comprennent rien (ce qui est tout-à-fait normal), ce qui fait d'eux des proies particulièrement faciles pour les escrocs et les sociopathes de tout poil qui grouillent dans ce domaine. 
* On pouvait penser que le _hardfork_ de Bcash en août 2017 avait définitivement tranché le débat et que, chacun ayant une chaîne répondant à ses attentes, les partisans des petits blocs et les sectateurs des gros blocs allaient pouvoir s'ignorer superbement et que tout serait bien qui finit bien. Malheureusement, Bcash est en train de se muer en instrument d'[agitprop](https://fr.wikipedia.org/wiki/Agitprop) au service d'une petite frange dirigée par un [escroc patenté](https://dankaminsky.com/2016/05/02/validating-satoshi-or-not/) et un [sociopathe narcissique](https://www.youtube.com/watch?v=oCOjCEth6xI) qui poussent depuis quelques temps la fiction que Bcash est le _seul et unique_ Bitcoin. Je n'y avais guère prêté attention avant de constater récemment que des [gens informés et intelligents](https://www.yours.org/content/for-world-adoption--bch-needs-to-solve-two-main-issues-4b03922c0a0d) étaient en train de tomber dans le panneau. Je n'en dis pas plus pour le moment car l'article concerne Bitcoin, nous règlerons son compte à Bcash dans un autre article.

## Prémisses

Le sujet est complexe et mériterait littéralement un livre entier. Afin de garder cet article le plus concis possible, je vous propose donc d'accepter les hypothèses suivantes :
1. Bitcoin n'est pas un "business", ni une monnaie et encore moins un réseau de paiement, c'est un [logiciel, du code, de l'information](http://www.sosthene.net/bitcoin-bitcoins/), **c'est tout**.
2. Exécuté par un réseau de pairs, ce code permet de générer, sécuriser et échanger des objets numériques rares et rivaux, les bitcoins.
3. Les règles du protocole que suivent ces utilisateurs ont été conçus dans un objectif bien précis : créer un ["peer-to-peer electronic cash system"](https://bitcoin.org/bitcoin.pdf). Petite mise au point : contrairement à une erreur largement répandue (ignorance que les propagandistes de Bcash exploitent sans vergogne), **_cash_ ne signifie pas "petite monnaie" ou "microtransaction"**. Le cash est simplement une [forme d'argent qui a sa valeur _en soi_]((http://www.sosthene.net/finir-blockchain/) et s'oppose à monnaie scrupturale ou fiduciaire. Historiquement, le cash, c'est _l'or_, souvenez-vous en la prochaine fois que vous lirez "Bitcoin a trahi la vision de Satoshi, qui était de faire du cash électronique, pas de l'or".
4. La proposition de valeur de Bitcoin est donc d'être un système monétaire dont aucun acteur ne peut modifier les règles à son avantage, car chacun est un pair, un _égal_, qui contribue à garantir que les _règles du jeu_ restent les mêmes. 

## Trois Arguments en faveur du maintien des petits blocs

1. Bitcoin impose nécessairement un compromis entre "facilité de transaction" et "facilité de validation", mais la facilité de validation est plus critique et doit être préférée sur la facilité de transaction.
2. À l'heure actuelle, il n'y a pas d'alternatives sérieuses à la mise en place d'un noeud personnel pour valider les transactions et donc être réellement un pair sur le réseau. 
3. Bitcoin est une opportunité unique, en cas d'échec nous n'aurons pas de 2ème chance, chaque modification de protocole doit être entreprise avec une prudence extrême. 

### Le nécessaire compromis entre nombre de transactions et facilité de les valider

Contrairement à ce qu'on entend souvent, la _blockchain_ n'est pas magique, c'est un dispositif qui remplit un objectif précis mais qui impose des restrictions et des compromis. L'un de ces compromis est entre le nombre de transactions que le réseau peut traiter par seconde et la facilité avec laquelle ces transactions sont diffusées et vérifiées par les pairs du réseau. 

Contrairement à ce que beaucoup voudraient vous faire croire, il n'y a pas de [repas gratuit](https://en.wikipedia.org/wiki/There_ain%27t_no_such_thing_as_a_free_lunch) : si vous augmentez le nombre de transactions inscrites sur la blockchain en vous contentant de faire des blocs plus gros ou plus rapprochés, vous imposez fatalement à tous les pairs de contrôler et relayer davantage d'informations, ce qui augmente les requis techniques pour opérer un noeud, avec le risque réel qu'une partie du réseau devienne incapable de se synchroniser (c'est ce qui se passe depuis quelques temps sur [Ethereum](https://hackernoon.com/the-ethereum-blockchain-size-has-exceeded-1tb-and-yes-its-an-issue-2b650b5f4f62)). 

Faisons 2 hypothèses extrêmes :
1. 1 bloc de 200kb toutes les heures : les requis techniques sont très faibles, ce qui permet de synchroniser la blockchain de Bitcoin sur à peu près n'importe quel appareil, y compris des téléphones portables récents. En revanche, le nombre de transactions est extrêmement limité, seuls ceux qui ont réellement besoin des caractéristiques de Bitcoin l'utilisent (gros montants, transfers internationaux etc).
2. 1 bloc de 1gb toutes les 2 secondes : Bitcoin peut absorber un nombre gigantesque de transactions par seconde, tout le monde l'utilise pour des micropaiements ou pour acheter un café. En revanche, les requis en termes de puissance de calcul et de bande passante pour simplement opérer un noeud (sans parler de miner donc) sont tellement énormes qu'en gros seuls les GAFA peuvent se le permettre. 

La première hypothèse est certes ennuyeuse, beaucoup de cas d'usage ne sont plus viables et ralentit énormément l'adoption par les utilisateurs. En revanche, cette situation extrême préserve **le** cas d'usage, celui qu'aucun autre service ne peut proposer à part Bitcoin : _peer-to-peer electronic cash_. 

Dans le 2ème cas en revanche, vous avez paypal 2.0, et Bitcoin est mort. Félicitations, vous avez réinventé le système actuel, et le jour où les 3 ou 4 entreprises en mesure d'entretenir des noeuds décideront de relever la limite de 21 millions de bitcoins ou tout autre modification de protocole à leur avantage, vous n'y pourrez rien, vous n'êtes pas pair du réseau.

Aujourd'hui, on peut estimer que dans ce dilemme Bitcoin est déjà un peu trop du côté de la facilité de transaction. Pourquoi ? Le réseau fonctionne aujourd'hui dans des conditions relativement idéales : les infrastructures internet mondiales sont suffisamment intégrées et performantes, aucun État n'a rendu illégal le minage ni la possession d'un noeud Bitcoin. En dépit de ces conditions favorables, le minage tend déjà à se centraliser et nombre d'utilisateurs se contentent encore de laisser leurs bitcoins sur une plateforme d'échange ou un client léger. Que se passerait-il si demain l'internet chinois se trouvait isolé du reste du monde ? Si plusieurs États localisaient les noeuds opérés par des particuliers grâce à leur adresse IP pour les confisquer ?

### Pour être un pair sur le réseau Bitcoin, il n'existe aujourd'hui pas d'alternative au noeud

Être un pair, cela signifie ne dépendre de personne pour être en mesure de valider n'importe quelle transaction, et en premier lieu celles qui nous concernent, ainsi que le respect du consensus par les autres pairs. Aujourd'hui cela n'est possible qu'en opérant son propre noeud. 

On peut passer par une analogie avec l'or pour comprendre pourquoi ce contrôle exercé par l'ensemble des pairs est capital. 

L'or est la meilleure monnaie que l'humanité ait jamais eu... avant Bitcoin du moins. Mais l'or a échoué et n'est aujourd'hui plus la base de notre système monétaire. 

L'or présentait certes toutes les qualités de la monnaie par excellence, durabilité, divisibilité etc, mais avait aussi des défauts très gênants. Les coûts de transaction sont très élevés en raison de la nécessité de vérifier avec exactitude la qualité de l'or, surtout si l'opération doit être répétée à chaque transaction. Une solution classique à ce problème est de déléguer la vérification à une autorité qui frappe la monnaie d'un symbole aisé à reconnaître mais difficile à reproduire, censé garantir qu'une pièce contient une certaine quantité d'or d'une qualité donnée. Une autre solution un peu plus évoluée consiste à remettre son or en dépôt à une banque, qui nous remet en échange des instruments fiduciaires (lettres de change, chèque, lettre au porteur etc) qui nous permettent d'effectuer nos paiements beaucoup plus simplement.

Le problème en procédant ainsi, c'est que les acteurs économiques délèguent en réalité une part importante de leur pouvoir au vérificateur : ce sont les fameux risques de contrepartie, et Bitcoin a précisément été inventé pour les supprimer. Le vérificateur finit en effet systématiquement par abuser de son pouvoir : les souverains ont **toujours** dévalué la monnaie dont ils étaient censé garantir la pureté. De leur côté, les banques ont rapidement compris qu'elles pouvaient tirer d'importants bénéfices en émettant davantage de billets échangeable en or que ce qu'elle possédaient réellement dans leurs coffres. 

Ces pratiques ont entraîné la création des banques centrales que nous connaissons aujourd'hui, et après quelques décennies l'essentiel des réserves d'or s'y étant concentré, les gouvernements européens n'ont plus eu qu'à les saisir au début de la 1ère guerre mondiale pour financer leur effort de guerre. 

Opérer un noeud Bitcoin revient à réaliser un test sur toutes les transactions jamais effectués pour garantir qu'il s'agit bien de vrais bitcoins non dévalués, ce qui est infiniment plus puissant et plus efficace que les tests disponibles pour l'or. Ne pas utiliser son propre noeud revient à s'en remettre à une autorité pour contrôler la qualité des bitcoins que **VOUS** possédez, recréant ainsi la configuration qui a amené à la situation actuelle. 

Il existe aujourd'hui quantité de porte-monnaie électronique, ou _wallet_, qui ne se synchronisent pas avec la blockchain et se contente d'interroger les noeuds pour obtenir leur balance et diffuser leurs transactions. Ces wallets sont souvent appelé SPV, pour _simplified payment verification_, et ne font en gros que télécharger une partie des informations sur un bloc qui les intéresse pour pouvoir vérifier l'existence d'une transaction antérieure. 

Ces wallets "légers", plus pratiques pour l'utilisateur et opérables sur téléphone, souffrent néanmoins de plusieurs défauts :
* Ils sont dépendants de l'existence de noeuds en nombre suffisant pour répondre à leur requête, et sont davantage vulnérables en cas d'attaque.
* Ils exposent davantage d'informations qui permettent de relier les adresses de l'utilisateur à son identité réel, et impactent donc négativement la confidentialité de ces transactions (même si un système appelé _Bloom filter_ a depuis été implémenté pour mitiger ce problème).
* Mais leur défaut le plus grave, c'est qu'ils ne sont que des _leechers_ du réseau, et pas des pairs. Ils ne relaient ni ne valident ni les transactions, ni les blocs. Ils sont incapables de détecter un bloc invalide ou une modification de protocole, et peuvent être trompés et suivre une autre chaîne avec des règles de validation différentes. 

La dernière vulnérabilité n'est pas que théorique : en novembre 2017, une tentative très controversée de hardfork, S2X, a échoué car quasiment aucun noeud n'avait choisi d'effectuer la mise à jour nécessaire. Les nouveaux blocs créés aurait donc été rejetés comme invalides par l'ensemble du réseau, une situation très dangereuse pour les mineurs qui auraient choisi de s'aventurer à miner ce fork. Si le réseau n'avait été constitué que de SPV wallet, ces derniers auraient accepté sans broncher le nouveau protocole sans même que les utilisateurs n'en soient avertis. 

### Nous ne devons pas commettre d'erreur avec Bitcoin, nous n'aurons pas de seconde chance

Il existe aujourd'hui plusieurs centaines d'altcoins. L'immense majorité ne sont que de pales copies de Bitcoin, néanmoins certains soutiennent que les altoins pourraient coexister avec Bitcoin, ou même qu'un de ces altcoins pourraient le supplanter à terme. Cela semble improbable pour deux raisons :

* Une des promesses de Bitcoin est que le nombre de bitcoins en existence ne dépassera jamais 21 millions. Créer des altcoins est une façon de contourner cette limite et de recréer une forme d'inflation qui dilue à la fois la valeur de chaque bitcoin et aussi celle de chaque altcoin. C'est pourquoi sur le long terme il ne pourra subsister qu'une seule crypto monnaie, Bitcoin.
* Bitcoin est la seule occurrence d'une monnaie dont la croissance a été entièrement organique et réellement anarchique. **Tous** les altcoins sans aucune exception sont dirigés par une équipe qui agit comme leur propriétaire légitime. Ces "leaders" constituent un point unique de défaillance, ils peuvent être corrompus ou éliminés. Il y a une forme _d'immaculée conception_ de Bitcoin qu'aucun altcoin n'est en mesure de reproduire. 

Il est donc extrêmement douteux que les altcoins puissent remplacer ou même coexister durablement avec Bitcoin, mais admettons que cela soit possible, quelles sont les conséquences dans l'approche que nous devons avoir vis-à-vis du développement de Bitcoin ?  
* Si nos objectifs peuvent être atteints avec un autre altcoin, alors ce n'est pas grave de pécher par excès de prudence, même si Bitcoin devait décliner à cause de mauvaises décisions nous avons d'autres alternatives. Le marché parlera, tout le monde utilisera Bcash ou Ethereum et tout sera pour le mieux. 
* Si Bitcoin n'est pas remplaçable et que nous n'avons donc qu'une seule chance de créer un standard monétaire décentralisé et résistant à la censure, alors nous devons toujours privilégier la solution la plus sûre pour ne pas compromettre le caractère décentralisé de Bitcoin.

Bref, dans tous les cas il est préférable de garder les blocs petits. 

## Conclusion

Il y a énormément de distractions dans les discussions autour de l'avenir de Bitcoin, ce qui nous empêche de nous poser les vraies questions : qu'est-ce que Bitcoin ? Pourquoi a-t-il autant de valeur ? Quels sont les risques qui pourrait annihiler cette valeur et comment les éviter ? 

Bitcoin est encore à un stade de développement précoce qu'il faut réussir à penser sur plusieurs décennies, beaucoup de choses peuvent se passer mais ce qui est certain, c'est qu'il est difficile d'imaginer un scénario dans lequel Bitcoin échoue _uniquement_ car il ne permet pas d'effectuer des microtransactions on-chain. La réintroduction de risques de contrepartie, c'est-à-dire la possibilité pour un tiers de censurer ou d'inverser des transactions, ou encore bien pire, de modifier unilatéralement le protocole, est en revanche un scénario d'échec extrêmement probable et qui devrait tous nous préoccupper. 

Les partisans de Bcash et des gros blocs en général commettent une erreur d'analyse fondamentale : ils pensent que Bitcoin est un réseau de paiement, et évaluent donc sa réussite en le comparant à Visa ou Paypal. Cela est absurde, car pour atteindre les performances en termes de vitesse de transaction qui permettraient à Bitcoin de concurrencer des réseaux de paiement centralisés, il est nécessaire de sacrifier la possibilité d'avoir des validateurs autres que les mineurs. Une fois que ces derniers sont les seuls _pairs_ du réseau, comme dans le cas de l'or, ce n'est qu'une question de temps avant qu'ils imposent des changements de protocole qui leurs sont favorables.

Bien sûr, cela se fera avec les meilleures raisons du monde, on invoquera l'intérêt général, et le pire, c'est qu'à moins d'un changement radical de culture au sein des populations qui nécessiterait facilement une ou deux générations, la décision de lever la limite des 21 millions sera accueillie avec indifférence, voire peut-être même avec le soutien d'une majorité de la population. Quand tout le monde le réclamera à corps et à cri, que seuls les mineurs et quelques grosses banques possèderont un noeud, vous, petit bitcoiner maximaliste, qu'est-ce que vous allez y faire, hein ?

Tout le sens de Bitcoin est de ne pas être une démocratie, de mettre la création monétaire hors de portée du politique. Si ce type de pressions redevient possible, alors Bitcoin n'a plus aucune raison d'être. La meilleure parade que nous ayons pour le moment est de favoriser le déploiement de noeuds par le maximum d'individus :

* en cas de tentatives d'interdiction et de confiscation par un ou plusieurs gouvernements, notre meilleure protection est le nombre. Il serait trivial de confisquer leur ordinateur à 50 geeks à l'échelle d'un pays, nettement plus problématique pour des milliers d'ordinateurs, impossible si il y a un noeud sur chaque ordinateur du pays,
* l'expérience du hardfork raté de S2X nous a enseigné que si les utilisateurs ne suivent pas, cela peut suffire à faire reculer une attaque extrêmement bien organisée et qui avait le soutien des mineurs. 
* cela a également l'avantage de diffuser une culture de responsabilité et d'améliorer la compréhension de Bitcoin et de son fonctionnement.

Ce n'est évidemment pas suffisant, ni infaillible, mais si vous souhaitez que Bitcoin réussisse c'est encore la meilleure chose que vous puissiez faire.  

