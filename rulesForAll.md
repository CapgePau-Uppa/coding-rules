# GENERAL RULES

**GENERAL_00**  
Utiliser l'anglais pour le nommage et les commentaires.

**GENERAL_01**  
Aération du code, Saut de ligne entre les parties logiques.

**GENERAL_02**  
Appliquer la règle SOLID (Single Responsibility, Open/closed, Liskov substituion, Interface Segregation, Dependency Inversion).
Keep It Simple Stupid, Don't Repeat Yourself.

**GENERAL_03** 
Correct > Lisible > Performant (Favoriser dans cet ordre).

**GENERAL_04**  
Noms prononçables
	Package : toutenminusculeetausingulier (lower_camel_case)
	Classe : MajusculePourChaqueDebutDeMot (upper_camel_case)
	Variables : minusculePuisMajusculePourChaqueDebutDeMot.
Les noms de variables composés d'un seul caractère doivent être évités sauf pour des variables provisoires (index d'une boucle).

**GENERAL_05**  
Documenter l'intention et non le déroulement.

**GENERAL_06**  
Utilisez les design patterns quand c’est possible et renseignez-les proprement dans les noms de classes: Factory, Builder, Listener, Adapter etc.

**GENERAL_07**  
Il est obligatoire de séparer le modèle, l’interface et le contrôleur (MVC). Pour vérifier qu’il s’agit bien d’une implémentation MVC, il ne doit y avoir aucun import de classes GUI dans une classe model ou process et inversement.

# JAVA RULES

**JAVA_00**  
Organisez une classe du plus général (service ou méthode publiques) au plus précis par convention :
	Attributs statiques/enum,
	Bloc statiques,
	Attributs non statiques,
	Constructeurs,
	Les autres méthodes,
	Les inners class/interfaces.

**JAVA_01**  
Pas plus de 5 appels en cascade.

**JAVA_02**  
Évitez les appels répétitifs à une méthode sur un même objet (getter).

**JAVA_03**  
Pas plus de 10 paramètres, et essayer de tendre vers le moins possible.

**JAVA_04**  
Dans le cas où la classe a plusieurs constructeurs, il faut concentrer les initialisations dans un seul constructeur et utiliser les constructeurs délégués this(….) dans tous les autres.

**JAVA_05**  
Nommage Constantes (statiques, enum…) : EN_MAJUSCULES_SEPARE_PAR_UNSERSCORES.
Nommage Méthodes : minusculePuisMajusculePourChaqueDebutDeMot. Leur nom devrait commencer/contenir un verbe.

**JAVA_06**  
Regroupez les catchs quand c’est possible (si c’est la même action à mener derrière chaque catch). Préférez le multi-catch plutôt qu’un unique catch d’Exception.Evitez d’imbriquer les try/catch. Utilisez les exceptions Java existantes au lieu d’en créer des nouvelles.

**JAVA_NOT_00**  
N’utilisez pas la réflexion (en général).

**JAVA_NOT_01**  
Ne manipulez pas le Garbage Collector (Interdiction d’utiliser System.gc()).

**JAVA_NOT_02**  
N’utilisez pas les anciennes collections synchronisées (Vector, HashTable…).

**JAVA_NOT_03**  
Ne retournez pas null (sauf @Override ou forcé par une librairie). Préférez les Optional (de java), chaine vide, liste vide… ou lever une exception en fonction des cas. Lancez une exception quand le comportement est faux ou inattendu.
