# Le phénomène Big Data
## Introduction
Les données se produisent aujourd’hui à un rythme effréné. De nouvelles unités pour estimer la quantité de données font leur apparition tels que le ZettaByte (10<sup>21</sup> octets), le YottaByte (10<sup>24</sup> octets), le BrontoByte (10<sup>27</sup> octets) ou encore le GeopByte (10<sup>30</sup> octets). L’IDC (International Data Corporation) prévoit qu’en 2025, la quantité des données produites à l’échelle mondiale atteindra 163 ZettaBytes dont plus de 25% seront créées en temps réel par des objets connectés qui en produisent plus de 95% [Reinsel, 17]. La Big Data est une conséquence directe de cette "digitalisation" de la vie humaine. L’Internet des Objets - IoT (de l’anglais Internet of Things), les objets connectés, les réseaux sociaux et le Cloud Computing ont tous contribué à cette évolution technologique. Les connaissances pouvant être extraites de ces énormes volumes de données forcent les organisations d’y investir pour assurer leur pouvoir concurrentiel. Toutefois, dans le contexte Big Data, de nombreux concepts largement adoptés dans les technologies traditionnelles ne sont plus applicables. A tire d’exemple, la normalisation des données relationnelles n’a plus d’importance en Big Data ; des nouvelles bases de données, dites NoSQL, prennent de plus en plus de place dans les marchés des bases de données et ne tiennent pas en considération les formes normales. Les bases de données NoSQL s’intéressent plutôt au stockage de très gros volumes de données, de différentes structures, de sorte que le traitement de ces données soit rapide et efficace.

Avant l’émergence des technologies Big Data, les entreprises distinguaient entre deux types de données : vivantes ou archivées. Les données vivantes ne concernent que celles nécessaires à l’activité quotidienne de l’entreprise, les autres étaient systématiquement archivées. En outre, les archives ne pouvaient être gardées pendant de longues périodes à cause des limites des solutions traditionnelles de stockage et de leurs coûts élevés ainsi que de la complexité des processus de gestion qui manquaient d’évolutivité et de flexibilité. En revanche, les technologies Big Data ont été conçues pour collecter, stocker, analyser et exploiter de gros volumes de données. Cela a donc permis aux entreprises de profiter pleinement de l’ensemble de leurs données sans avoir recours à l’archivage.

Pour toutes ces raisons, de nombreux projets importants ont été lancés dans différents pays. En 2012, l’Administration de Barack Obama a investi plus de 200 millions de dollars sur un projet de Recherche & Développement en Big Data, intitulé « *Big Data Research and Development Initiative* », dans le but d’améliorer leur compétence à extraire des connaissances et des nouvelles idées à partir de larges collections de données numériques. L’administration était convaincue que ce projet leur promettrait de transformer leur capacité à utiliser les technologies Big Data pour la découverte scientifique, la recherche environnementale et biomédicale, l’éducation et la sécurité nationale [The White House, 12]. Les Nations Unies ont également publié un rapport, intitulé « *Big Data for Development: Opportunities and Challenges* » qui vise à souligner les principales préoccupations concernant les défis de la Big Data et à favoriser le dialogue sur la façon dont elle peut servir le développement international [Global Pulse, 12]. À la suite de ces projets, de nombreux modèles et cadres ont été développés et des nouvelles technologies ont été créées dans le but de fournir plus de capacité de stockage, théoriquement pouvant aller jusqu’à l’infini, des traitements parallèles et des analyses en temps réel des données hétérogènes.

Bien qu’aucune définition standard ne soit encore reconnue pour le terme "Big Data", de nombreux travaux de recherche tentent de le définir selon différents points de vue. La section suivante de ce blog est réservée à la définition de la Big Data et à la discussion de différentes propriétés qui la caractérisent. Ensuite, nous présentons des exemples d’application dans différents domaines économiques et sociaux. Enfin, la dernière section présente le cycle de vie des projets Big Data ainsi que les grands défis encore ouverts à la recherche.
## Définition et Caractéristiques de la Big Data
Gartner a défini la Big Data comme étant des sources d’information à haut volume, à haute vélocité et/ou à haute diversité qui nécessitent de nouvelles formes de traitement pour permettre l’amélioration de la prise de décision, la découverte d’informations et l’optimisation des processus [Gartner, 21]. Gantz et Reinsel [Gantz, 11] définissent les technologies Big Data comme étant une nouvelle génération de technologies et d’architectures, conçues pour extraire une valeur économique à partir de très gros volumes de données, en permettant la capture, la découverte et/ou l’analyse à grande vitesse. Chen et Zhang [Chen, 14-a] proposent deux faces de la Big Data. D’un côté, la Big Data est extrêmement précieuse pour produire de la productivité dans les entreprises et des percées révolutionnaires dans les disciplines scientifiques, ce qui pourrait nous donner la possibilité de faire de grands progrès dans de nombreux domaines. De l’autre côté, la Big Data est confrontée à de nombreux défis, tels que les difficultés dans la saisie, le stockage, l’analyse et la visualisation de données. Par ailleurs, les données sont collectées en continu auprès de différentes sources (réseaux sociaux, enregistrements de transactions commerciales de banques, comportements d’utilisateurs sur des sites e-commerces, données de santé, articles publiés sur Internet, …). Cette diversification de données et les contraintes de volumétrie et de vitesse de traitement posent de nombreux challenges à la qualité et à la sécurité de données.

Nous pouvons ainsi définir la Big Data comme étant un ensemble de technologies et de moyens (modèles, techniques, cadres de travail, …) qui permettent de collecter, stocker et traiter, à une grande vitesse, de gros volumes de données hétérogènes dans l’objectif d’en tirer du profit. Ces données peuvent être structurées, semi-structurées ou non-structurées. La tendance aujourd’hui concernant la production de données penche vers des données semi-structurées plus que structurées et des données non-structurées plus que semi-structurées. De nombreux travaux de recherche caractérisent la Big Data par le modèle 5V illustré dans la Figure 1.
<p align="center">
  <img src="https://github.com/Cloud-Elit/big_data_phenomenon/assets/142179779/04fc96a5-24e2-4d55-82f8-693d1cfb9c13" /><br/>
  <i>Figure 1. Modèle 5V de la Big Data</i>
</p>

- Le **Volume** fait référence aux énormes quantités de données générées chaque seconde ; le volume de données joue un rôle important dans la mise en œuvre des outils et des modèles de stockage et de traitement de données.
- La **Vélocité** fait référence à la vitesse à laquelle les données sont produites et traitées. Les données peuvent être importées selon deux modes : les données importées par lots (ou batch), dans lequel des ensembles de données se chargent en une seule fois, et les flux de données (ou streaming), dans lequel les données sont continuellement importées et traitées à la volée.
- La **Variété** fait référence à l’hétérogénéité de données et de leurs sources. Les données structurées englobent un format de données unifié et peut être facilement géré avec des systèmes de gestion de bases de données relationnelles. En revanche, les données non-structurées et semi-structurées sont plus difficiles à analyser et nécessitent des infrastructures de traitement plus avancées.
- La **Véracité** fait référence à la cohérence et à la fiabilité des données. Les données peuvent être classées selon le degré de leur qualité (données de bonne ou de mauvaise qualité ou, si on ne peut pas évaluer leur qualité, les classer en données de qualité indéfinie).
- La **Valeur** fait référence à l’utilité des données dans la prise de décision et aux profits que l’on peut tirer de ces gros volumes de données. Il s’agit donc d’une des caractéristiques les plus pertinentes de la Big Data car elle reflète les bénéfices des organisations.

Certains travaux tels que [Katal, 13], [Kaisler, 13], [Gani, 15] et [Khan, 18] considèrent la "**Complexité**" comme étant une sixième caractéristique de la Big Data. La complexité mesure le degré d’interconnexion et d’interdépendance des structures de données de sorte qu’un petit changement, ou une combinaison de petits changements, dans un ou plusieurs éléments, peut produire de très grands changements qui se répercutent dans tout le système et affectent considérablement son comportement. Les auteurs de [Khan, 18] vont plus loin et caractérisent la Big Data par un modèle 10V. Outre les 5V vus jusqu’ici, Khan et al. définissent les caractéristiques suivantes :

- La **Viscosité** reflète la complexité des processus de gestion des données en Big Data.
- La **Variabilité** fait référence à un flux de données incohérent qui peut parfois être affiché.
- La **Volatilité** fait référence à la durée de vie pendant laquelle les données sont valides et pendant combien de temps elles doivent être stockées.
- La **Viabilité** fait référence à la capacité de la Big Data d’être vivante et active ainsi que sa capacité à se développer et à produire plus de données en cas de besoin.
- La **Validité** fait référence à l’exploitation des relations qui peuvent exister entre les données. Un ensemble de données peut ne pas avoir de problèmes de véracité mais peut ne pas être valide s’il n’est pas correctement compréhensible. De même, un ensemble de données peut être valide pour une application ou une utilisation spécifique et, en même temps, invalide pour une autre application ou utilisation.

Pour mieux comprendre l’ensemble de ces caractéristiques, Hashem et al. [Hashem, 14] classifient la Big Data selon cinq aspects, à savoir les sources de données, le format de données, le stockage de données, la préparation de données et, enfin, le traitement de données. 

Concernant le premier aspect, qui est "les sources de données", on trouve des données générées par :

- des médias sociaux qui permettent de partager et d’échanger des informations et des idées sur des communautés et des réseaux virtuels tels que les blogs et les réseaux sociaux.
- des machines qui produisent, de façon automatique, des grandes quantités d’informations à partir du matériel et des logiciels comme des calculateurs et des appareils médicaux.
- des objets connectés qui comprennent, entre autres, les Smartphones, les appareils photo numériques, les tablettes, les équipements intelligents (Télévision, Climatiseur, …). Lorsque ces appareils se connectent les uns aux autres via Internet, ils produisent des processus et des services intelligents qui répondent à des besoins économiques, environnementaux, sanitaires, etc.

Le deuxième aspect concerne "le format de données". Les données peuvent être structurées, semi-structurées ou non-structurées. Les données structurées sont souvent gérées en SQL ; elles sont faciles à saisir, interroger, stocker et analyser à condition que leurs volumes ne dépassent pas les capacités des systèmes de gestion des bases de données relationnelles (SGBDRs). Les données semi-structurées, par exemple des fichiers XML ou JSON, peuvent se présenter sous la forme de données structurées qui ne sont pas organisées en modèles de bases de données relationnelles. La capture de données semi-structurées pour l’analyse est différente de la capture d’un format structuré. Par conséquent, la capture de données semi-structurées nécessite l’utilisation de règles complexes qui décident de manière dynamique du processus à appliquer suite à la réception de nouvelles données. Enfin, les données non-structurées, telles qu’un texte libre ou des fichiers multimédia, sont des données qui ne suivent pas un format spécifié. La collecte et l’analyse de ce type de données constitue aujourd’hui un vrai défi pour les projets Big Data.

Le troisième aspect concerne "le stockage de données". Pour couvrir tous les formats de données, de nouveaux types de bases de données ont été développés que l’on désigne généralement par NoSQL. Différentes catégories existent dans ces bases de données : celles qui stockent les données sous formes de paires "clé-valeur", celles qui regroupent les colonnes dans des colonnes "larges" afin d’optimiser le stockage et le traitement, celles qui stockent les données sous forme de documents, généralement JSON, et enfin, celles qui stockent les données sous forme de graphes centrés sur la gestion des relations entre les objets. L’avantage majeur des bases de données NoSQL réside dans l’absence de schémas fixes pour stocker les données ni de jointures entre les tables ce qui permet un stockage et un traitement distribués de données ainsi qu’une mise à l’échelle plus simple. 

Le quatrième aspect concerne "la préparation de données". Cet aspect comporte différents processus tels que :

- le "nettoyage" qui consiste à identifier et à nettoyer des données incomplètes, obsolètes ou de mauvaise qualité.
- la "transformation" qui consiste à transformer les données dans une forme adaptée à l’analyse. 
- la "normalisation" qui consiste à structurer les données dans des schémas structurés pour simplifier leur exploitation ou encore minimiser la redondance.

Et enfin, le cinquième aspect concerne "le traitement de données" qui peut être soit par lots (traitement en batch) soit en temps réel (ou quasi-temps réel). Les systèmes basés sur MapReduce de la plateforme Hadoop[^1] ont été adoptés par de nombreuses organisations au cours des dernières années pour les travaux par lots de longue durée tandis que les systèmes de traitement en temps réel (ou quasi temps réel) permettent la mise à l’échelle des applications sur des clusters de machines comprenant un grand nombre de nœuds de traitement.
## Ubiquité de la Big Data
Les données aujourd’hui sont générées en grandes quantités, changent rapidement et se présentent sous diverses formes difficiles à gérer et à traiter à l’aide des SGBDRs ou d’autres technologies traditionnelles. Les solutions Big Data fournissent des outils, des méthodologies et des technologies, qui n’étaient auparavant pas disponibles. Ces solutions peuvent être utilisées pour capturer, stocker, rechercher et analyser les données rapidement afin d’extraire des relations et d’en déduire des informations qui peuvent être exploitées pour l’innovation et le gain concurrentiel. Les industries recherchent en continuité de nouvelles et meilleures façons de maintenir leur position et d’être préparées pour l’avenir. La Big Data leur fournit un moyen pour capturer des informations et des idées afin de rester en compétition dans la rude concurrence. 

Auparavant, la quantité de données générées n’était pas trop élevée et leur archivage avait pour but d’analyser l’historique des informations (pour des besoins d’audit, de contrôle, de détection d’intrusion, de prévision, de classement, etc.). Aujourd’hui, comme le volume de données se mesure en petaoctets, il n’est plus possible de les archiver et de les récupérer à nouveau pour l’analyse car les besoins ont changé ; les scientifiques de données doivent avoir en main toutes les données pour des analyses prédictives ou de classification, souvent en temps réel, ce qui n’était pas possible auparavant. Nous pouvons constater les avantages des techniques de la Big Data à travers une étude de cas présentée par la banque américaine Zions Bancorporation [Dark Reading, 12]. Cette étude a révélé qu’il fallait entre 20 et 60 minutes pour chercher parmi des données cumulées pendant un mois en utilisant les systèmes SIEM (Security Information and Event Management) traditionnels alors qu’en utilisant son nouveau système Hadoop exécutant des requêtes avec MapReduce et Hive, les mêmes résultats ont été obtenus en environ une minute. L’utilisation avantageuse des techniques de la Big Data telles que les capacités élevées de stockage, de traitement et d’analyse rapide des gros volumes de données non-structurées ne peut qu’améliorer la compétitivité des entreprises.

L’IoT représente l’un des principaux domaines en forte liaison avec la Big Data. D’une part, les objets connectés constituent la principale source générant des données et, d’autre part, les plateformes Big Data permettent d’exploiter efficacement ces grandes quantités de données. Cela a permis aux solutions IoT d’évoluer et d’intégrer de nombreux secteurs sociaux et économiques. Voici quelques exemples d’application IoT/Big Data :

- **Transport** : il est tout-à-fait possible, grâce à des capteurs installés sur des véhicules, de suivre leurs positions géographiques. La collection et l’analyse en temps réel de ces informations apportent de nombreux avantages aux entreprises et aux particuliers. A titre d’exemples, les entreprises de logistique peuvent superviser et gérer les véhicules, optimiser et adapter les plans de livraison, etc. Les taxis et les entreprises de location des voitures de tourisme avec chauffeurs (VTC) en profitent également en mettant en relation les clients et les chauffeurs, aider les chauffeurs à se diriger vers des endroits où il y a plus de possibilité de trouver des clients, etc. Les particuliers peuvent également en profiter grâce à des appareils SoS (Save our Souls) qui peuvent émettre automatiquement des demandes d’assistance immédiate en cas d’accidents.
- **Santé** : les plateformes de santé connectées (e-santé) permettent à de nombreuses sources de collecter et de transmettre des données sur les individus pour fournir des services personnalisés. Les données des laboratoires, les symptômes des patients téléchargés à partir de capteurs distants ou intégrés, les comptes rendus des opérations hospitalières, les données pharmaceutiques, et bien d’autres, constituent de grands ensembles de données médicales. L’analyse de ces données en temps réel permet d’assister les médecins à adapter des traitements ou d’intervenir rapidement en cas de danger. La sauvegarde de ces données auprès des organisations compétentes permet aux médecins d’urgence de mieux diagnostiquer les problèmes de santé des individus et aux chercheurs de mieux réaliser leurs études dans le respect total de la vie privée des individus.
- **Réseaux Sociaux** : les technologies de la Big Data sont très utilisées dans le domaine des réseaux sociaux aussi bien pour les plateformes qui fournissent des services que pour les organisations intéressées par l’analyse des profils et l’exploitation des informations des utilisateurs enregistrés sur ces plateformes. A titre d’exemple, une entreprise, en connaissant les préférences de ses clients potentiels, peut adapter ses produits afin de s’adresser à un plus grand nombre de personnes. En suivant ce que pensent leurs clients de leurs produits, une entreprise peut avoir un retour d’information lui permettant de mieux s’adapter aux besoins du marché. Un autre exemple d’utilisation de la Big Data dans les réseaux sociaux concerne les élections politiques. La Big Data a joué un rôle déterminant dans la campagne de réélection du président américain Barack Obama en 2012 [InfoWorld, 13], dans les campagnes électorales lors du référendum au Royaume-Uni sur le Brexit ainsi que dans la campagne électorale du président américain Donald Trump pour la présidentielle américaine. Pendant toutes ces compagnes, les intéressés se sont appuyés sur les technologies de la Big Data pour mieux adapter leurs discours et s’adresser directement aux électeurs [Libération, 17].
- **Audit** : les entreprises effectuent souvent l’analyse des audits pour renforcer leurs sécurités, prévoir des plans d’actions ou pour des simples opérations de classification ou de prévision. Par exemple, l’examination des journaux (logs) et l’analyse de l’historique des trafics réseaux et des évènements de sécurité permettent de détecter les anomalies et les intrusions ainsi que de prévenir des cyber-attaques. Les techniques de la Big Data aident non seulement à ne plus avoir besoin de supprimer ces journaux et ces historiques de trafics mais aussi à faciliter leur exploitation afin de renforcer la sécurité des organisations.
- **E-commerce** : les grandes entreprises du commerce électronique traitent chaque jour d’énormes quantités de données dans le but de prendre des décisions commerciales (adapter les prix, passer des commandes, faire des offres spéciales, etc.). Par exemple, eBay utilise des entrepôts de données de plusieurs petaoctets pour gérer les commandes et réaliser des opérations d’analyse sur les recommandations des consommateurs et les transactions commerciales entre les utilisateurs (vendeurs et acheteurs). Un autre exemple est celui d’Amazon qui a su profiter de la Big Data pour devenir la plus grande plateforme du commerce électronique mondiale. Amazon collecte des données individuelles concernant chacun de ses clients lorsqu’ils utilisent leurs sites web. En plus de ce que le client achète, Amazon garde également une trace des articles consultés, de l’adresse de livraison des utilisateurs ainsi que les avis laissés par les acheteurs. Pour améliorer leurs services, des inventaires sont suivis de façon automatique pour s’assurer que les commandes sont exécutées rapidement. Des modules intelligents permettent de choisir l’entrepôt le plus proche de l’utilisateur, réduisant considérablement les délais d’expédition. Amazon exploite ses données via un moteur de recommandation ; chaque fois qu’un utilisateur cherche un produit spécifique, le moteur de recommandation devine ce qui peut l’intéresser pour le convaincre à l’acheter.
## Cycle de vie des projets Big Data et principaux défis
L’importance de la Big Data réside dans la capacité technique de collecter et d’exploiter efficacement un très grand volume de données quels que soient leurs formats. Grâce à ces techniques, les organisations peuvent avoir une meilleure maitrise de leurs données ce qui permet d’améliorer leurs activités à différentes échelles : mieux se protéger, mieux vendre, mieux s’adapter aux besoins du marché, etc. En revanche, les chercheurs et les professionnels sont confrontés à de nombreux défis et problèmes pour améliorer les mécanismes d’exploitation des données. Les caractéristiques de la Big Data rendent les processus de collecte, de stockage, d’analyse et d’extraction des connaissances très complexes. Dans [Talha, 19] et [Talha, 20-a], nous avons discuté de nombreux problèmes liés à la Qualité et à la Sécurité de données en Big Data. Dans cette section, nous exposons certains des défis les plus discutés dans la littérature pour chaque phase du cycle de vie Big Data. 

De nombreux travaux identifient quatre phases principales du cycle de vie d’un projet Big Data. Comme illustré dans la Figure 2, la première phase consiste à collecter, de différentes sources, de très gros volumes de données hétérogènes ; la deuxième phase consiste à intégrer toutes ces données sur une plateforme distribuée qui est le lac de données (Data Lake en anglais) ; la troisième phase consiste à analyser ces données pour en déduire des connaissances et des nouvelles idées afin de les exploiter dans la quatrième phase et d’en extraire de la valeur.
<p align="center">
  <img src="https://github.com/Cloud-Elit/big_data_phenomenon/assets/142179779/875b802c-d7b0-42db-bd98-f475a7405e37" /><br/>
  <i>Figure 2. Cycle de vie des projets Big Data (inspirée de [Alladi, 18] et [Hakuta, 14])</i>
</p>

Les défis à relever pendant la phase de collection de données consistent généralement à mettre en place des mécanismes efficaces et des techniques qui peuvent supporter de très gros volumes de données qui se génèrent à une très grande vitesse et par différentes sources. La collection doit se produire dès que les données sont générées, dans des environnements sécurisés, tout en s’assurant de leur véracité et de la fiabilité de leurs sources. Selon le type de données, structurées ou non-structurées, il faut mettre en place des outils adaptés. Selon les fournisseurs de données (services internes à l’organisation, des organismes certifiés, des objets connectés, des réseaux sociaux, etc.), il faudra déployer tous les mécanismes et aspects techniques et matériels pour garantir la qualité et la sécurité de données.

Concernant la phase de stockage de données, les scientifiques sont souvent confrontés à des problématiques de réduction des coûts et d’optimisation des ressources matérielles et logicielles. Les plateformes de stockage doivent être distribuées au sein d’un même site géographique et/ou sur des sites géographiques différents (souvent dans des pays ou des continents différents afin de minimiser les risques des catastrophes naturelles ou de guerres). La distribution de données pose de nombreux problèmes tels que la gestion de l’intégrité, de la disponibilité et de la redondance de données. En outre, les plateformes de stockage doivent être évolutives de sorte que les processus d’augmentation et de réduction des espaces de stockage doivent être automatiques et ne doivent pas impacter la disponibilité de données. Par ailleurs, la qualité et la sécurité de données constituent deux principaux défis à tenir en considération pour les données d’une entreprise. De nombreux processus pour assurer la qualité de données, tels que le nettoyage et l’intégration de données, doivent être mis en place. Nous reviendrons dans le chapitre suivant sur les problèmes de la qualité de données en Big Data. Pour la sécurité des données, il s’agit d’un des problèmes les plus complexes lors de la phase de stockage de données. En effet, de nombreux problèmes, tels que l’intégration des politiques de contrôle d’accès, le contrôle d’accès à granularité fine, la protection de la vie privée des individus, etc., sont encore ouverts à la recherche.

L’exploitation des données commence à la phase d’analyse qui consiste à comprendre les relations entre les données et y appliquer des algorithmes d’exploration de données pour en extraire des connaissances. L’analyse peut être effectuée en temps réel (sur des flux de données) ou sur des données au repos à travers des traitements par lots. De nombreux domaines, comme le transport, la finance, l’e-santé et l’e-commerce nécessitent de traiter les données en temps réel, ou quasi-temps réel, pour pouvoir prendre des décisions rapides. D’autres applications telles que l’analyse de l’historique des transactions ou des comportements des utilisateurs, l’analyse des journaux, etc. permettent aux organisations d’extraire des informations précieuses et de construire des modèles de données qui peuvent affecter positivement ou négativement leurs positions concurrentielles, surveiller leurs flux d’entrée et de sortie, etc. L’analyse de données doit relever de nombreux défis liés principalement à la nature complexe de la Big Data, y compris les 5V, ainsi que les besoins d’évolutivité, de performances et d’adaptation [Wang, 16], [Tsai, 16].

La dernière phase dans le cycle de vie est l’extraction des connaissances et des nouvelles idées afin de les transformer en des valeurs tangibles. Le tout premier défi à ce niveau réside dans la validité des résultats. Selon si les calculs et les requêtes ont été appliqués sur des données correctes, des données incorrectes ou des données déduites, l’efficacité des résultats change. A cela s’ajoute d’autres problèmes tels que la représentation des données de sortie et leur transformation en des formats prêts à l’exploitation. Par ailleurs, la gouvernance de données constitue un autre défi à tenir en considération lors de l’exploitation de données. Il s’agit de contrôler la conformité des données vis-à-vis de la loi en vigueur, de la transparence et des responsabilités des individus et des systèmes d’information. L’identification des relations entre les données peut mener à la déduction d’informations sensibles ou confidentielles pouvant mettre en danger la vie privée des individus. Jensen dans [Jensen, 13] discute de nombreux défis de la protection de la vie privée dans le contexte Big Data tels que la gestion du consentement des individus, l’obligation par la loi de supprimer les données personnelles, les attaques de ré-identification, etc. 
## Bibliographie
- [Alladi, 18] Alladi, Bhima Sankaram & Prasad, Srinivas. (2017). Big data life cycle: security issues, challenges, threat and security model. International Journal of Engineering & Technology. Volume 7. DOI: 10.14419/ijet.v7i1.3.9666. 
- [Chen, 14-a] Chen, C.L. Philip & Zhang, Chun-Yang. (2014). Data-intensive applications, challenges, techniques and technologies: A survey on Big Data. Information Sciences. 275. 314–347. DOI: 10.1016/j.ins.2014.01.015. 
- [Dark Reading, 12] darkreading. (2012). A Case Study In Security Big Data Analysis. Available online: https://www.darkreading.com/security-monitoring/a-case-study-in-security-big-data-analysis (last accessed December 25, 2021)
- [Gani, 15] Gani, Abdullah & Siddiqa, Aisha & Band, Shahab & Nasaruddin, Fariza. (2015). A survey on Indexing Techniques for Big Data: Taxonomy and Performance Evaluation. Knowledge and Information Systems. 46. DOI: 10.1007/s10115-015-0830-y. 
- [Gantz, 11] Gantz, John & Reinsel, David. (2011). Extracting Value from Chaos. International Data Corporation (IDC).
- [Gartner, 21] Gartner. (2021). Gartner Glossary - Big Data. Available online: https://www.gartner.com/en/information-technology/glossary/big-data (last accessed December 25, 2021)
- [Global Pulse, 12] United Nations Global Pulse. (2012). Big Data for Development: Challenges & Opportunities.
- [Hakuta, 14] Hakuta, Keisuke & Sato, Hisayoshi. (2014). Cryptographic Technology for Benefiting from Big Data. Springer, The Impact of Applications on Mathematics 2014. 85-95. DOI: 10.1007/978-4-431-54907-9_6. 
- [Hashem, 14] Hashem, Ibrahim & Yaqoob, Ibrar & Anuar, Nor & Mokhtar, Salimah & Gani, Abdullah & Khan, Samee. (2014). The rise of "Big Data" on cloud computing: Review and open research issues. Information Systems. 47. 98-115. DOI: 10.1016/j.is.2014.07.006. 
- [InfoWorld, 13] InfoWorld. (2013). THINK BIG DATA - The real story of how big data analytics helped Obama win. Available online: https://www.infoworld.com/article/2613587/the-real-story-of-how-big-data-analytics-helped-obama-win.html (last accessed December 25, 2021)
- [Jensen, 13] Jensen, Meiko. (2013). Challenges of Privacy Protection in Big Data Analytics. IEEE International Congress on Big Data. 235-238. DOI: 10.1109/BigData.Congress.2013.39. 
- [Kaisler, 13] Kaisler, Stephen & Armour, Frank & Espinosa, J. & Money, William. (2013). Big Data: Issues and Challenges Moving Forward. Proceedings of the Annual Hawaii International Conference on System Sciences. 995-1004. DOI: 10.1109/HICSS.2013.645. 
- [Katal, 13] Katal, Avita & Wazid, Mohammad & Goudar, R.H.. (2013). Big data: Issues, challenges, tools and Good practices. IEEE. 404-409. DOI: 10.1109/IC3.2013.6612229. 
- [Khan, 18] Khan, Nawsher & Alsaqer, Mohammed & Shah, Habib & Badsha, Gran & Abbasi, Aftab & Salehian, Solmaz. (2018). The 10 Vs, Issues and Challenges of Big Data. 52-56. DOI: 10.1145/3206157.3206166. 
- [Libération, 17] Libération. (2017). Succès fous (4/4) - Cambridge Analytica, big data et gros dégâts. Available online: https://www.liberation.fr/futurs/2017/08/17/cambridge-analytica-big-data-et-gros-degats_1590468/ (last accessed December 25, 2021)
- [Reinsel, 17] Reinsel, David & Gantz, John & Rydning, John. (2017). Data Age 2025: The Evolution of Data to Life-Critical; Don't Focus on Big Data; Focus on the Data That's Big. IDC White Paper.
- [Talha, 19] Talha, Mohamed & Abou El Kalam, Anas & Elmarzouqi, Nabil. (2019). Big Data: Trade-off between Data Quality and Data Security. The 10th International Conference on Ambient Systems, Networks and Technologies (ANT 2019). April 29 - May 2, 2019, Leuven, Belgium. Procedia Computer Science. 151. 916-922. DOI: 10.1016/j.procs.2019.04.127. 
- [Talha, 20-a] Talha, Mohamed & Elmarzouqi Nabil & Abou El Kalam, Anas. (2020). Quality and Security in Big Data: Challenges as opportunities to build a powerful wrap-up solution. Journal of Ubiquitous Systems and Pervasive Networks. 12. 09-15. DOI: 10.5383/JUSPN.12.01.002. 
- [The White House, 12] The White House. (2012). PRESS RELEASE: Obama Administration Unveils "Big Data" Initiative: Announces $200 Million in New R&D Investments. Available online: https://obamawhitehouse.archives.gov/the-press-office/2015/11/19/release-obama-administration-unveils-big-data-initiative-announces-200 (last accessed December 25, 2021)
- [Tsai, 16] Tsai, Chun-Wei & Lai, Chin-Feng & Chao, Han-Chieh & Vasilakos, Athanasios. V.. (2016). Big data analytics: a survey. Journal of Big Data. DOI: 10.1007/978-3-319-44550-2_2. 
- [Wang, 16] Wang, Hai & Xu, Zeshui & Fujita, Hamido & Liu, Shousheng. (2016). Towards Felicitous Decision Making: An Overview on Challenges and Trends of Big Data. Information Sciences. 367. DOI: 10.1016/j.ins.2016.07.007. 
[^1]: http://hadoop.apache.org/
