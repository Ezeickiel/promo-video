Kovri Lightweight C++ I2P Router Script

Version 1 français- sgp / cryptochangements

Monero est une monnaie électronique sécurisée et intraçable.  Elle est open-source, décentralisée et facilement accessible pour tous.

Dans ce vidéo, nous allons parler d'une technologie d'anonymat appelée Kovri.

Jusqu'à maintenant, cette série a présenté la façon dont Monero obscurcit l'information stockée sur le blockchain.
Les bagues de signatures obscurcissent l'expéditeur, les adresses furtives préviennent les observateurs extérieurs de découvrir l'adresse de destination, et les bagues de transactions confidentielles cachent le nombre de Monero transmis.
Par contre, quelques informations personnelles et identifiables peuvent être divulgées lorsqu'une transaction est annoncée au réseau.

Cette fuite d'information privé est colmatée avec Kovri.  

Kovri est une technologie d'anonimat gratuite, décentralisée, fondée sur les spécifications ouverte de I2P.  Kovri utilise du cryptage ainsi que des techniques d'acheminement sophistiquées pour créer un revêtement privé sur le réseau internet.  Ce revêtement de protection permet aux utilisateurs de cacher leurs positions géographiques et leurs adresses IP.  Une adresse ip est comme une adresse domiciliaire mais pour internet.  Il s'agit donc , à tout de moins, d'une information très délicate. 

Examinons maintenant quelques scénarios pour voir comment cette modeste application de sécurité aide à renforcer l'anonymat de ses utilisateurs. 

Supposons qu'Alice voudrait envoyer une transaction à Bob. Le porte-monnaie d'Alice crée une transaction et la divulge sur le réseau Monero.  Le réseau Monero est constitué de noeuds qui communiquent ensemble en acheminant des messages à travers une séries d'adresses IP.  Ceci implique qu'il est possible de retraçer les données géographiquement, pendant qu'elles traversent l'internet, partout, entre le début et la fin de leurs parcours.  Même si les porte-monnaies des expéditeurs et des récipiendaires, ainsi que les montants demeurent privés, Alice prend un risque lorsqu'elle divulgue sa transaction, car certains noeuds pourrait noter les adresses IP.  Un adversaire bien nantis pourraient tenter d'associer des transactions avec des adresses IP afin de déterminer l'origine des transactions.  Ceci pourrait potentiellement permettre à l'adversaire d'empêcher le relai de ses transactions sur le réseaux ou encore pire, de se présenter à sa porte.   les expéditeurs et les récipiendaires sont anonymes une série de noeuds interconnectéAlice est , et elle est prête à dire au réseau de nœuds et mineurs qu'elle voudrait que le réseau inclut sa transaction dans le prochain bloc.

Alice est connecté à pluseurs, mais pas tous, les nœuds du réseau. Sa requête de transaction va devoir atteindre autant de nœuds que possible pour avoir la plus grande chance d'être inclus dans le prochain bloc. Elle est connecté à 5 nœuds du réseau, elle envoie donc sa requête de transaction aux 5 nœuds. Le système continue comme ça jusqu'à beaucoup de nœuds ont cette donnée

Malheureusement, il y a toujours un peu de danger en envoyant sa requête. C'est possible que des nœuds du réseau enregistre l'adresse IP dont la requête vient. Une adresse IP est comme votre adresse de domicile, mais pour votre connexion internet. Un attaquant ne peut pas savoir si la première adresse IP qu'il a eu est la vraie adresse du envoyeur, et il ne peut pas savoir les détails de la transacion comme l'envoyeur, le montant, ou le récepteur. Pourtant, l'attaquant peut associer une transaction, comme la transaction qu'Alice a créé dans cet exemple, avec une adresse IP pour lui aider deviner l'envoyeur.

Un attaquant peut donc frapper à la porte d'Alice et exiger qu'Alice lui donne ses clés privées pour qu'il peut enquêter. Alternativement, l'attaquant peut essayer de bloquer les transactions d'Alice d'être transmis au réseau. On appel ce genre d'attaque une "Attaque Sybil"

Qu'est-ce qu'on peut faire pour atténuer ce problème? Alice ne sait pas quels nœuds enregistrent sa adresse IP, donc elle ne peut pas éviter ces mouvais nœuds. Son seul choix est de cacher sa adresse IP.

Il existe pluseurs de façons de cacher votre adresse IP. On peut utiliser TOR, un VPN, ou I2P. Nous allons nous concentre sur I2P dans cette vidéo puisque c'est le réseau dont Kovri participe.

Dans une seule phrase, Kovri est un routeur simple pour le réseau I2P qui est programmé en C++ et il est compatible avec des cryptomonnaies. I2P est une couche d'internet qui rend toutes les connexions dans le réseau privée. Au lieu de se connecter directement au réseau, comme un site du web, tout l'information est transmis aux autres routeurs du réseau I2P. Ces routeurs savent peu ou aucun détails sur la donnée qu'ils transmettent, du coup toute la donnée est privée.

Kovri sera intégré avec Monero dans des futures sorties et il sera activé par défaut pour annoncer les transactions aux réseau.

Maintenant, quand Alice envoie sa requête de transaction travers le réseau I2P avec Kovri, personne ne pourra savoir sa adresse IP. Les nœuds du réseau Monero qui enregistre des adresses IP ne verra qu'une adresse .i2p qui ne sert à rien. Donc, si ces nœuds continuent à enregistrer des adresses IP, ce genre d'information ne sera plus utile.

En outre, supposons qu'Alice a un fournisseur d'accès internet qui ne veut pas qu'elle utilise Monero. Alice peut choisir d'envoyer tout la donnée de Monero travers le réseau I2P. Maintenant, son fournisseur d'accès internet ne pourra pas savoir qu'elle utilise Monero.

Bref, Kovri est un routeur qui permet à utilisateurs de Monero de se connecter au réseau I2P pour qu'ils peuvent envoyer anonymement des requêtes de transaction. Des nœuds du réseau Monero ne pourra plus enregistrer les vrais adresses IP d'utilisateurs de Monero.

Visitez getkovri.org pour en savoir plus sur Kovri, ou getmonero.org pour en savoir plus sur Monero
