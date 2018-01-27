Kovri Lightweight C++ I2P Router Script

Version 1 français- sgp / cryptochangements

Le Monero est une monnaie électronique sécurisée et intraçable.  Il est open-source, décentralisé, et facilement accessible à tous.

Dans cette vidéo, nous allons parler de la technologie d'anonymat appelée Kovri.

Jusqu'à maintenant, nous avons  démontré la façon dont Monero obscurcit l'information stockée sur le blockchain.

Les bagues de signatures obscurcissent l'expéditeur, les adresses furtives préviennent les observateurs externes de découvrir l'adresse de destination, et les bagues de transactions confidentielles cachent le nombre de Monero transmis.
Par contre, quelques informations personnelles et identifiables peuvent être divulguées lorsqu'une transaction est annoncée sur le réseau.

Ce problème de fuite d'information privée est colmaté avec la venue de Kovri.  

Kovri est une technologie d'anonymat gratuite, décentralisée, fondée sur les spécifications ouverte du protocole I2P.  Kovri utilise du cryptage ainsi que des techniques d'acheminement sophistiquées pour créer un revêtement privé sur le réseau internet.  Ce revêtement de protection permet aux utilisateurs de cacher leurs positions géographiques et leurs adresses IP.  Une adresse ip est comme une adresse domiciliaire sur internet.  Il s'agit donc , à tout de moins, d'une information très délicate. 

Examinons maintenant quelques scénarios pour voir comment cette modeste application de sécurité aide à renforcer l'anonymat de ses utilisateurs. 

Supposons qu'Alice voudrait envoyer une transaction à Bob. Le porte-monnaie d'Alice crée une transaction et la divulgue sur le réseau Monero.  Le réseau Monero est constitué de nœuds qui communiquent ensemble en acheminant des messages à travers une série d'adresses IP.  Ceci implique qu'il est possible de retracer les données géographiquement, pendant qu'elles traversent l'internet, du début jusqu’à la fin de leurs routes.  Même si les porte-monnaie des expéditeurs ou ceux des récipiendaires demeurent privés, Alice prend un risque lorsqu'elle divulgue sa transaction, car certains nœuds pourraient enregistrer les adresses IP.  Un adversaire bien nantis pourrait tenter d'associer les transactions avec les adresses IP afin de déterminer l'origine des transactions.  Ceci pourrait potentiellement permettre à l'adversaire d'empêcher le relai de ses transactions sur le réseau ou, encore pire, de se présenter à sa porte.  

Maintenant, imaginons un autre exemple. Supposons que Charlie veut supporter le réseau Monero en exploitant son propre un nœud chez lui.  Après quelques semaines, Charlie reçoit une note de bris de contrat, car l’exploitation de nœud violerait les termes de service de son fournisseur internet.

Ou considérez ceci: Supposons que Dave est responsable d’un bassin de mineur et qui fait don  d’une portion de ses gains à un parti politique ou à une cause controversée.  Les autres nœuds pourraient  délibérément refuser la résolution de ses blocks pour exprimer leur désaccord avec ses opinions politiques ou sociales.

Alice, Bob, Charlie et Dave ont tous quelque chose en commun: leur adresses IP sont détectable sur le réseau.  Des usagers peuvent essayer de cacher leurs adresses IP avec des réseaux TOR ou des  réseau privé virtuel. Par contre, chacune de ces  stratégies ont des lacunes importantes. 

Le réseau TOR est géré par des autorités dont la confiance laisse à désirer et qui allouent  à certains opérateur de nœuds TOR une influence démesurée dans le consensus du réseau. Le consensus du réseau  détermine ultimement qui est autorisé à relayer le trafic dans le réseau TOR—et cela basé sur les opinions des autorités.

Par ailleurs, les attaques de corrélations sont possibles auprès des réseaux privés virtuels fiables.  Une attaque nombreuse permettrait de facilement dé-anonymiser le trafic d’un utilisateur.

Alors, qu’est-ce  qu’Alice, Bob, Charlie et Dave peuvent faire pour  atténuer ces menaces?  Ils peuvent utiliser Kovri. 
S’ils utilisent exclusivement Kovri sur le réseau Monero, personne ne pourra détecter leurs adresses ips, rendant la surveillance passive impraticable tout en améliorant substantiellement la résistance du Monero à la censure.

Comme vous voyez, Kovri est une application qui permet à ses utilisateurs de transmettre leurs transactions de façon encore plus anonyme.

Plongeon maintenant dans les technicalités afin de voir ce qui se cache sous le capot de la technologie Kovri.

Kovri dirige le trafic dans le réseau I2P en utilisant du cryptage en bulbe d’ail et de l’acheminement en bulbe d’ail.  L’information voyage à l’intérieur d’un revêtement de réseau privé par l’entremise de message recevant une couche  d’encryptions  à chaque fois que le message est relayé par un pair dans le réseau. Comme une poupée russe. Chaque poupée interne contient un verrou et une clé publique pour la poupée suivante. Les pairs sur le réseaux sont incapable de lire le contenu du message relayé, ce qui rend  l’information envoyé par l’expéditeur, ou reçu par le destinataire,  tout à fait sécurisée.

La seule information visible pour les pairs est l’instruction d’acheminement vers le prochain pair. 

Pour atteindre une meilleure confidentialité, moyennant une petite baisse de performance, les utilisateurs sont capables de se connecter à d’autres pairs.  Essentiellement, Kovri masque le traffic internet  d’une application pour le rendre anonyme à l’intérieur du réseau.

Avec ces caractéristiques, Kovri est une merveilleuse solution pour communiquer anonymement sur IRC, par e-mail, ou pour accéder à des services cachés.

Kovri révolutionnera les connections pairs à pairs tout en renforçant la résilience et l’anonymat de réseau au niveau mondial.
Les nœuds malicieux ne pourront plus menacer les utilisateurs qui crée des transactions, ou de  bloquer leur propagations à travers le réseau.

Kovri sera inclus dans les prochaines sorties de Monero et sera activé par défaut.  De plus Kovri sera doté  d’un API  commun qui permettra à d’autres applications ou crypto-monnaie  de l’utiliser.  Pas juste le Monero.

Pour connaître d’avantage sur le Monero ou sur le projet Kovri, veuillez consulter Getmonero.org et GetKovri.org


