# Small blocks : an apology

## Why write this now ?

This article is NOT for the blocksize debate veterans that have been around for many years. They have already most probably heard this argument a thousand times. I hope this article could help the newcomers in the _wonderful_ world of Bitcoin, or those that are not here yet, but will join us in the years to come, or even those that only have a casual interest on Bitcoin (no _skin in the game_ yet !) but might be interested by what I have to say.  

Here is why I felt it could be useful to write this :
* Useful information is spread across dozens of articles, blog posts, forums, tweets, reddit or videos over the past 3 years or so. You cannot ask someone new to the field to go and screen through all that shit himself, at least not without first giving him some synthetic argument about what is at stake and why things are the way they are today.
* It is even more important today than what we should call a _speculative bubble_ on ICO and "crypto" has inflated in 2017, understandably attracting a lot of interest beyond the usual _afficionados_. Wave after wave of new users, investors and simple observers swept across our field, they are clueless of course (which is fine), but it makes them easy preys for the crooks, scammers and various sociopaths.
* I first thought that Bcash hardfork last august definitely settled the debate, and that since everyone now have the choice to go with _small_ or _big_ blocks as they feel confortable with, each side will go its merry way and never ever argue again. Too bad it didn't last long before Bcash became a tool of [agitprop](https://en.wikipedia.org/wiki/Agitprop) leveraged by a small group whose leaders are a [prooved scammer](https://dankaminsky.com/2016/05/02/validating-satoshi-or-not/) and a [narcist sociopath](https://www.youtube.com/watch?v=oCOjCEth6xI) that have made up a new narrative in which Bcash is _the true and unique_ Bitcoin, in what seems to be an attempt to leverage the brand in their own interest. But anyway, we're not talking about Bcash here, so let's move on.

## Prerequisites

Bitcoin is a complex matter, and would deserve a whole book to be discussed at lenght. But since it just means to be a readable article, here is the hypothesis of my argument :
1. Bitcoin is not a business, nor is it a currency and most importantly it is **not** a payment network. Factually, Bitcoin is [a software, it is code, information](https://hackernoon.com/why-america-cant-regulate-bitcoin-8c77cee8d794), **period**.
2. While runned by a network of peers, this code enable generation, safe conservation and trade of a kind of commodity, that is digital, scarce and rival, and commonly called "bitcoins".
3. To achieve that, the peers of the network all agree on a protocol, a set of rules that has been designed to make Bitcoin a ["peer-to-peer electronic cash system"](https://bitcoin.org/bitcoin.pdf). Here we should make immediately clear that opposite to a very common misunderstanding of the word _cash_ (an ignorance easily exploited by Bcash propagandists), **cash does not mean "pocket money" or "microtransaction"**. Cash is money that can be used for ultimate settlement of debt because it does not rely on a third party like says credit card. Historically, cash has been _gold_, so remember that next time someone tells you "Bitcoin betrayed Satoshi's vision, because the whitepaper is talking about _cash_, not _gold_". He has either being deceived or is trying to deceive you.
4. The main part of Bitcoin's value is to be a monetary system whose rules nobody can change. It's a network of _peers_, which means that they're all equal and enforcing the same set of rules. It's not a democracy where some ill-defined _majority_ can impose anything on the minority. Each peer is free to enforce the rules he thinks appropriate, but must suffer the consequences of his choice. 

## Three arguments to keep the blocks small

1. Bitcoin does impose a trade-off between "ease-of-transaction" (enabled by having bigger blocks) and "ease-of-validation" (the smallest the blokcs, the easier to validate). What's important is the two side of the deal are not of equal importance : the latter is critical while the former is not. That means **we must never trade "ease-of-validation" for "ease-of-transaction"**. 
2. Today, there is no alternative to running a full node to validate transactions and enforce protocol. Bigger blocks raise the requirement to operate a full node yourself, while by keeping blocks small you actually make it easier and easier as domestic computers become more powerful.
3. With Bitcoin we only have one shot, if we mess things up we are very unlikely to recreate the same conditions. That's why we must be very prudent, especially regarding modifications on the protocol level. I know some people won't get it, but in Bitcoin _not doing anything_ is the best option most of the time. 

### The "ease of transaction" versus "ease of validation" trade-off

In case you bought into some _blockchain_ bullshit made up by consultants, it is useful to remind that the _blockchain_ is not a magical tool, that is a scheme made to solve **one** problem, that is double spend in a decentralized open system. This scheme comes with serious constraints and trade-off, one of those being if you increase transactions output (number of transaction every second), you also increase the cost for every node to validate and broadcast an increased number of transaction. 

As everybody should know, [there is no free meal](https://en.wikipedia.org/wiki/There_ain%27t_no_such_thing_as_a_free_lunch). Having bigger blocks allows for more transactions to be processed on the network, but as you raise the cost of operating a full node, you effectively push more and more users out of the network as their node eventually becomes incapable to catch up on the present block (this is not theoretical, this is real and this has been happening to [Ethereum](https://hackernoon.com/the-ethereum-blockchain-size-has-exceeded-1tb-and-yes-its-an-issue-2b650b5f4f62) for some time now). The question is then : should we prefer processing more transactions at the cost of having less nodes on the network ? 

Let's try the two sides of the question with _ad absurdum_ arguments : 
1. If Bitcoin's blockchain processed **1 block of 200kb every hour**, technical requirement would become very low, meaning that virtually any device connected to the internet could run its own full node, including phones. On the other hand, the transactions output would be seriously crippled, meaning that it would be used for large amount, international transfer or when one really needs censorship resistant money (buying a cup of coffee in Palo Alto obviously doesn't qualify as such).
2. Now, let's say that we can process **1 block of 1gb every 2 seconds** : transaction output is ridiculously large, everyone can use it including for microtransactions like buying a cup of coffee every morning. Great, isn't it ? But there's a price to pay : technical requirements for running a full node had become so huge that only miners and some big companies can afford one.

In our first hypothesis, it would definitely be an annoyance for many users, most use cases would be out-priced and we definitely would not see mass consumers adoption in a near future. But the point is that even in this extreme case, Bitcoin can still do what it was meant for, _peer-to-peer electronic cash_. 

Now on the 2nd hypothesis, while it sounds great, something tragic happened : Bitcoin is not anymore, and you got Paypal 2.0 instead. Congratulations, you just reinvented _fiat world_, except with slightly different actors. Why ? Because one day the 3 or 4 compagnies that run full nodes will raise the 21 millions cap on the number of bitcoins, or will make any change to the protocol, or freeze your UTXO, and you won't do anything about it, because you are not a _peer_. You will be as powerless as you are today. 

Now back to reality. Things are obviously more balanced today, but Bitcoin is arguably already a bit too much on the ease-of-transaction side. Why ? The conditions faced by the network nowaday are not too much adversarial, in fact it is relatively ideal : reliable internet infrastructures on a global scale, no ban on mining or running a full node. But despite operating under quite friendly conditions, we observe that mining is already relatively centralized (it could be much worse though), and most users just keep their bitcoins on third party custody, or at best with a light client wallet. What would happen if China's internet infrasctructure was suddenly severed from the rest of the world ? What if a western country or a coalition of states declared a _real_ ban on Bitcoin, seizing everything that is on an exchange and a cracking down on the people that run a full node at home ? 

Bitcoin is designed to keep running even on very hard environment, but it seems that **we** haven't prepared too well for that.

### If you want to be a peer, you have to run your node

What I mean by being a _peer_, is that you don't depend on anybody to validate any transaction and make sure that everyone is enforcing the consensus you agreed with. And today it can only be done by running a full node.

An analogy with gold can helps us understand why control from all peers is important. 

Gold is the best money humanity ever had... except it failed and it has ceased to be the basis of our monetary system for some time now. 

Gold has many great features that make it sound money, like durability, divisibility, low stock-to-flow ratio etc, but it also has shortcomings. Transaction costs are very high, because it is not easy to test that the gold you are given is of a said weight and finness, especially if you have to repeat the test for every transaction you are making. A solution that people confronted with this issue came up with was to delegate this operation to some _authority_ that is supposed to certify that a coin is made of some that weight of gold of a said finness. Another solution would be to leave his gold in deposit to some bank, and use scriptural money to transact.

But there is a big trade-off : by doing that, individual actors are in giving some power over their own property to thier parties. That kind of _counterparty risks_ are what Bitcoin was made to annihilate. The fact is that actors endorsed with this power will abuse it, and more sooner than later. Political power had **always** debased the coins they were supposed to guarantee. Banks have **always** lend their deposit by making more gold receipt than they actually have in their vault. 

Recurrent crisis in the XIXth century pleaded for the creation of a _lender of last resort_, central banks that are still around today. As gold became more and more concentrated in a few central banks vaults, it became very easy for most european governments to seize their gold at the outburst of WW1.

Why Bitcoin would be fundamentally different ? Because when you run a Bitcoin full node, it would be as if you were able to test the gold used in every transaction since the dawn of time and discard every piece of counterfeited gold that ever existed, so that when someone would give you a gold ingot as a payment you would instantly know that it is pure gold. It is orders of magnitude safer and more efficient than gold.

On the other hand, not using a full node would be a lot like gold coinage as you need to trust some third party to validate **your** bitcoins. You trust them not to abuse this power, and we all know given sufficient time they will.

Il existe aujourd'hui quantité de porte-monnaie électronique, ou _wallet_, qui ne se synchronisent pas avec la blockchain et se contente d'interroger les noeuds pour obtenir leur balance et diffuser leurs transactions. Ces wallets sont souvent appelé SPV, pour _simplified payment verification_, et ne font en gros que télécharger une partie des informations sur un bloc qui les intéresse pour pouvoir vérifier l'existence d'une transaction antérieure. 

Ces wallets "légers", plus pratiques pour l'utilisateur et opérables sur téléphone, souffrent néanmoins de plusieurs défauts :
* Ils sont dépendants de l'existence de noeuds en nombre suffisant pour répondre à leur requête, et sont davantage vulnérables en cas d'attaque.
* Ils exposent davantage d'informations qui permettent de relier les adresses de l'utilisateur à son identité réel, et impactent donc négativement la confidentialité de ces transactions (même si un système appelé _Bloom filter_ a depuis été implémenté pour mitiger ce problème).
* Mais leur défaut le plus grave, c'est qu'ils ne sont que des _leechers_ du réseau, et pas des pairs. Ils ne relaient ni ne valident ni les transactions, ni les blocs. Ils sont incapables de détecter un bloc invalide ou une modification de protocole, et peuvent être trompés et suivre une autre chaîne avec des règles de validation différentes. 

La dernière vulnérabilité n'est pas que théorique : en novembre 2017, une tentative très controversée de hardfork, S2X, a échoué car quasiment aucun noeud n'avait choisi d'effectuer la mise à jour nécessaire. Les nouveaux blocs créés aurait donc été rejetés comme invalides par l'ensemble du réseau, une situation très dangereuse pour les mineurs qui auraient choisi de s'aventurer à miner ce fork. Si le réseau n'avait été constitué que de SPV wallet, ces derniers auraient accepté sans broncher le nouveau protocole sans même que les utilisateurs n'en soient avertis. 

### We won't have a second chance

As of today there are hundreds of _altcoin_. Most of them are just Bitcoin copycat and dead or dying by now, but some people think that altcoins could coexist significantly with Bitcoin, or even that some altcoin could displace Bitcoin as the top crypto currency. It seems very unlikely :

* Une des promesses de Bitcoin est que le nombre de bitcoins en existence ne dépassera jamais 21 millions. Créer des altcoins est une façon de contourner cette limite et de recréer une forme d'inflation qui dilue à la fois la valeur de chaque bitcoin et aussi celle de chaque altcoin. C'est pourquoi sur le long terme il ne pourra subsister qu'une seule crypto monnaie, Bitcoin.
* Bitcoin est la seule occurrence d'une monnaie dont la croissance a été entièrement organique et réellement anarchique. **Tous** les altcoins sans aucune exception sont dirigés par une équipe qui agit comme leur propriétaire légitime. Ces "leaders" constituent un point unique de défaillance, ils peuvent être corrompus ou éliminés. Il y a une forme _d'immaculée conception_ de Bitcoin qu'aucun altcoin n'est en mesure de reproduire. 

* If it was really possible to have an 

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

