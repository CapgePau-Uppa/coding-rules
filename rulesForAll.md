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
Dans le cas où la classe a plusieurs constructeurs, il faut concentrer les initialisations
dans un seul constructeur et utiliser les constructeurs délégués this(….) dans tous les autres.

**JAVA_05**  
Nommage Constantes (statiques, enum…) : EN_MAJUSCULES_SEPARE_PAR_UNSERSCORES
Nommage Méthodes : minusculePuisMajusculePourChaqueDebutDeMot. Leur nom devrait commencer/contenir un verbe.
