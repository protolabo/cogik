---
title: Suivi du projet
---

<style>
    @media screen and (min-width: 76em) {
        .md-sidebar--primary {
            display: none !important;
        }
    }
</style>

# Suivi de projet

<!-- > :bulb: Cette page documente l’évolution du projet dans le temps.
> Elle sert à rendre visibles les décisions, ajustements et apprentissages.
> Les entrées peuvent être hebdomadaires ou bi-hebdomadaires.  
> N'oubliez pas d’effacer ou de mettre en commentaires les notes (`>`) avant la remise finale. -->

---

## Semaine 1 (12–18 janvier)

### Objectifs de la période

- Clarifier la problématique
- Explorer les solutions existantes

### Travail réalisé

!!! abstract "Avancement"
    - [x] Analyse de solutions existantes

### Décisions et ajustements

<!-- > À compléter uniquement si des choix structurants ont été faits
> ou si l’orientation du projet a évolué. -->

!!! info "Décisions"
    - Choix du navigateur par défaut pour l'extension : Chrome (/ Chromium)

### Difficultés rencontrées

<!-- > À compléter uniquement si des obstacles ont eu un impact réel
> sur l’avancement du projet. -->

!!! warning "Difficultés"
    - Limitations de la gestion du cache sur Firefox

## Semaine 6 (16–22 janvier)

### Objectifs de la période

- Implémenter la base de l'application
- Faire le 1er diagramme de classe
- Préparer la présentation orale

### Travail réalisé

!!! abstract "Avancement"

-> Compte-rendu
-Documentation importante effectuée sur React/ReactNative. Je suis assez familier avec la base de ces langages maintenant, ou en tout cas tout ce que j'ai utilisé pour concevoir la 1re version de l'application cette semaine

-Page d'acceuil de l'application et 1re leçon implémentées de façon satisfaisante.
Initialement j'avais dit que je me focuserais seulement sur la 1re leçon mais comme j'ai fini plus rapidement que prévu je me suis attaqué à la page d'accueil (qui elle a pris BEAUCOUP plus de temps).

Pour la page d'acceuil, le focus a principalement était l'aspect esthétique (UI) et ce qui a pris le plus de temps a été la création des différents SVGs utilisés et s'assurer que les dimensions de ces images correspondaient avec celles du site (j'ai fait beaucoup d'essai-erreur en termes de redimensionnement et de positionnement)

-> Ce qu'il reste : 
-Il reste à implémenter la carte et le système de déplacement du train de l'application. Pour l'instant, ce qu'il y a ressemble plus à un placeholder.

Je préfère remettre cette tâche à la semaine prochaine car je dois me concentrer pour l'instant davantage sur le diagramme de classe et sur la présentation orale de demain (sans compter que peut-être avant d'implémenter qqch potentiellement d'aussi chronophage que la carte, il serait préférable d'attendre les premiers retours)

En général, très grande progression effectuée lors de cette semaine !

-> Remarques
-Je m'attends à devoir faire des choix d'optimisation à compter de la semaine prochaine. En effet, l'une des animations implémentées s'est finalement révélée plus lourde que prévu alors qu'au final il me paraissait simple à implémenter (comparé à ce que j'avais déjà implémenté)

-Je compte discuter avec le superviseur sur les outils que je peux utiliser pour évaluer les performances du site en général. En effet, pour l'instant ce qui rend difficile d'évaluer à quel point le code est efficace ou non est que je me fie principalement sur mon impression de la vitesse. Tout me semblait ok jusqu'à ce que j'aie tenté d'implémener l'animation dont j'ai parlé dans le paragraphe du dessus. Étant donné que cette animation n'était pas plus complexe que d'autres précédemment implémentées dans l'application, cela m'amène à me questionner sur la possibilité que je m'étais trompé auparavant quant à l'efficacité de mon code en général
TLDR: Tomber sur un cas de ralentissement évident a attiré mon attention sur la question de performances/efficacité 

### Décisions et ajustements

<!-- > À compléter uniquement si des choix structurants ont été faits
> ou si l’orientation du projet a évolué. -->

!!! info "Décisions"
    - Aucune décision ou choix majeure qui n'aie pas été précédemment disctuée

### Difficultés rencontrées

<!-- > À compléter uniquement si des obstacles ont eu un impact réel
> sur l’avancement du projet. -->

!!! warning "Difficultés"
    Aucune difficulté rencontrée si ce n'est que c'était la première fois que j'interagissais vraiment avec React/ReactNative (et ca s'est bien passé)

## Semaine 10 (16–22 janvier)

### Objectifs de la période

- Approfondir le 1er niveau

### Travail réalisé

!!! abstract "Avancement"
    - Le travail ici est plus conceptuel, donc je préfère parler de "Décision" -> voir section Décisions et ajustements

### Décisions et ajustements

<!-- > À compléter uniquement si des choix structurants ont été faits
> ou si l’orientation du projet a évolué. -->

!!! info "Décisions"
    - J'ai passé le plus clair de la semaine à cogiter sur le niveau principal. Comme on avait discuté, je préfère me concentrer sur un seul niveau (et ainsi pouvoir avoir plus de facilité à automatiser le processus pour le reste des niveaux de l'application) que me disperser sur plusieurs choses. J'ai donc passé beaucoup de temps à réfléchir sur l'architecture qu'aurait un niveau typique. <br> <br>
    Les concepts qui sont sortis de ma réflexion sont les suivantes. Peu de chances de rajouts majeurs par la suite : <br>
    Note: j'ai nommé la mascotte "Chippy" (car cela rappelle un castor + le fait de "chip" du bois) <br><br>
    Objets <br>
    On l'a déjà défini. C'est tout entité physique potentiellement manipulable par le joueur <br> <br>

    Slots <br> 
    Ce sont les supports sur lesquels je compte placer les objets. Pour rendre l'application modulable, je préfère ne pas me reposer sur des photos qui <br>   contiendraient déjà les objets voulus "incrustrés" dans la photo (car cela rendrait la manipulation beaucoup plus compliquée). Je suis donc venu avec l'idée <br> d'avoir des entités spécifiques dans le niveau qu'on appelerait "slots", qui serainet indépendants du background (probablement fait par SVG!) et sur lesquels on pourrait placer les objets. <br>
    La différence entre un slot et un objet est qu'un slot n'est pas forcément manipulable (bien qu'il peut l'être et dans ce cas il serait à la fois objet et <br> slot!). Il est surtout la pour son rôle de support <br>
 
    Zones <br>
    Ce seront les parties explorables de chaque niveau. J'ai introduit ce concept à cause de la petitesse de l'écran qui fait que c'est difficile de tout afficher <br> dans le niveau d'un seul coup sans rendre l'écran étouffant. L'idée est donc que quand on arrive dans le niveau, on est dans la vue principale. À partir  <br> de cette vue, on peut aller à gauche, à droite, devant ou derrière (le bouton "derrière" n'est activé que si on est déjà allé vers l'avant à partir de la vue principale). <br> 
    Comme je suspecte que plus l'utilisateur va avancer dans le roadmap, plus les niveaux vont "grossir", alors on peut mettre plusieurs zones dans une direction donnée (donc on peut mettre 2 zones vers l'avant, 3 vers la droite, etc.). <br>

    Situations <br>
    Ce concept est une généralisation du mot "Évènement". Je veux que cette application reste une appli d'apprentissage de langage, et non pas un jeu. De ce fait, j'aimerais le garder plus passif que le serait un jeu pour bien garder cette distinction le plus possible. <br>
    La philosophie d'un jeu est qu'on fait une action et le monde réagit. La philosophie de cette application est l'inverse : le monde autour de nous est vivant  <br> et le joueur réagit à ce qu'il voit. Il réagit à des "situations". Ces situations peuvent être actives ("La cloche a sonné") et dans ce cas ce sont plus précisément des évènements. <br>
    Mais elles peuvent aussi être passives ("Cet objet que je vois est une pomme"). Pratiquement tout peut être une situation qui déclenche une réaction chez le joueur. <br>
    La simple présence d'un objet est déjà une situation potentielle. L'idée est que l'apprenant va apprendre des expressions dans la langue-cible au travers des réactions du joueur qu'il contrôle. <br>

    Intentions <br>
    J'ai renommé le concept de "besoin" en "intentions" car je le trouvais plus général. Par exemple, c'est étrange de qualifier l'idée "Je veux désigner cet <br>objet que je vois devant moi" de besoin. C'est plus une intention pour moi. Honnêtement, ce mot est tellement abstrait qu'un autre renommage n'est pas  <br> impossible.<br>


Pour être plus concret, voici maintenant des exemples de chacune de ces catégories (j'y ai vraiment pensé en profondeur) : <br>

Intentions <br>
->Désigner des choses de façon simple: <br>
Ex:  <br>
Intention "Je veux désigner la pomme" -> Expression "Apple" ou "This is an apple" <br> <br>
->Réactions simples à de petits évènements <br>
Ex: <br>
Intention "Je suis surpris"-> "Oh!"<br>
Intention "Je suis joyeux" -> "Yes!" ou "Hooray!" <br>
Intention "Je suis choqué" -> "What happened?"<br>
Intention "Je me questionne" -> "Why?" ou "Hmm" <br>
Intention "Mon ventre gargouille" -> "My stomach growled" <br>
Intention "Je suis excité de l'arrivée de Chippy" -> "Chippy is coming!!" <br><br>
->Exprimer ses ressentis primaires<br>
Ex: 
Intention "J'ai faim " -> "I'm hungry"<br>
Intention "J'ai envie de dormir" -> "I'm sleepy"<br>
Intention "J'ai froid" -> "I'm cold"<br>
Intention "Ca m'a fait mal" -> "Ouch"<br>
-> Signaler un problème <br>
Ex:<br>
Intention "Je suis désemparé face à cette fuite" -> "Water!" <br>
Intention "Je suis déçu que mon jouet soit brisé" -> "It's broken" <br>
Intention "Je suis désemparé face à la noirceur" (suite à coupure de courant) -> "No light"<br>
Intention "J'ai besoin d'aide !" (en général) -> "Help!" <br>
-> Interactions avec le chien (ou autre animal de compagnie) <br>
Ex: <br>
Intention "Je veux attirer l'attention de mon chien" -> "Come here!"<br>
Intention "Je veux que mon chien s'assoit" -> "Assis!" <br>
Intention "Je veux que mon chien arrête" -> "Stop!" <br>
Intention "Je veux que mon chien attrape ma balle" -> "Catch that!" <br>
Intention "Je trouve mon chien trop bruyant" -> "You are noisy!"  <br>
Intention "Je veux que mon chien lâche ce qu'il tient dans sa gueule" -> "Drop it!" <br>
-> Interactions avec "Chippy" <br>
Ex:
Intention "Je veux cet objet inatteignable" (en hauteur) -> "I want this" <br>
Intention "Je veux que le four soit mis en marche" -> "Turn it on please" <br>
Intention "Je veux attirer l'attention de papa" -> "Look!" <br>
Intention "Je veux que papa sache ce qui s'est passé" -> "I fell" <br>
Intention "Je veux que papa reste" -> "Don't go!" <br>
-> Indiquer positionnement d'objets (pr Chippy) <br>
Ex:
Intention "Je veux indiquer à papa où est la pomme" -> "The apple is in the box" <br>
Intention "Je veux indiquer à papa où est le chien" -> "The dog is under the sofa" <br><br>
-> Exprimer sa volonté <br>
Ex: 
Intention "Je veux exprimer à papa mon refus" -> "No!" <br>
Intention "Je veux que papa m'aide à monter sur le comptoir" -> "Lift me"<br>
-> Se parler à soi-même<br>
Intention "Je me demande comment le chien est monté aussi haut" -> "How?" <br>

Note: Je vais essayer de finir ma liste d'intentions d'ici vendredi <br>


Objets<br>
définition: un objet est tout ce qui est manipulable<br>
Fruits: pomme, banane, orange<br>
Ustensiles: Cuillère, fourchette, bol, assiette, verre<br>
Être vivants: Chippy, chien, chat<br>
Liquides: eau, lait<br>
Meubles: Lit, table, chaise, sofa<br>
Appareils: four, ordinateur, télévision, lumière<br><br>

Slots<br>
définition : un slot est un support capable d'accueillir des objets. Un slot peut lui-même être un objet (donc manipulable)<br>
Meubles<br>
Maison: sol, plafond, mur, maison (eh oui!), escalier<br>

Zones<br>
définition : partie explorable du niveau<br>
Salon (zone principale)<br>
Cuisine (zone à droite de salon)<br>
Chambre (zone à gauche de salon)<br>
Toilette (zone en face de salon)<br>


Situations <br>
Note : les situations "actives" sont appelées "évènement" <br>
-Visite inattendue de Chippy (évènement) <br>
-Le chien saute sur la table (évènement) <br>
-Le chien apporte un objet (évènement) <br>
-De l'eau coule (évènement) <br>
-Objet posé trop loin <br>
-La cloche sonne (évènement) <br>
-La lumière clignote (évènement) <br>
-La lumière de toute la maison s'éteint (blackout) (évènement) <br>
-Qqch tombe (évènement) <br>
-Qqch fait du bruit (évènement) <br>
-Il manque qqch <br> 
-Un désir survient (envie de manger, vouloir toucher un objet..) <br>
-Une chaise tombe par terre <br>
-L'alarme retentit <br>
-La porte s'ouvre/se ferme <br>
-La télévision grésille <br>
-La télé ne s'ouvre pas <br>

Dans un niveau donné, je vais faire en sorte que les expressions montrées ne prennent pas trop <br>
de liberté pour favoriser les connexions dans le cerveau de l'apprenant. <br>
Ex: "J'ai faim" (niveau 1), "J'ai soif" (niveau 1), "J'ai chaud" (niveau 1), "J'ai mal" (niveau 1) <br>
Ex2: "La pomme est sur la table" (niveau 2), "Le bol est sur la table" (niveau 2), "Le chien est sur le canapé" (niveau 2) <br>

Si j'ai le temps de faire un autre niveau (ce que je ne vais pas assumer vu que je me focus juste sur un niveau actuellement), je vais aussi essayer de garder une <br> certaine constante même si bien sûr les expressions apprises prendront un peu plus de liberté et seront un peu plus enrichies (car sinon l'utilisateur <br> apprendrait un langage "stéréotypé" et scolaire) <br>
Ex: "J'ai faim" (niveau 1) -> "J'ai très faim" (niveau 2) -> "J'ai vraiment une faim de loup" (niveau 3) -> "J'ai si faim que je pourrais avaler un éléphant"  (niveau 4) -> etc. <br>
---
Maintenant, si je regroupe les expressions similaires que je planifie pour le premier incrément, cela donnerait ceci (juste pour montrer comment l'utilisateur  <br> ferait des connexions entre les expressions apprises) : <br>
I am hungry<br>
I am sleepy<br>
I am cold<br>
This is an Apple<br>
This is a Banana<br>
This is a dog<br>
It is broken<br>
It is cool
It is beautiful<br>
Help me!<br>
Lift me!<br>
Follow me!<br>
Hug me!<br>
Give it to me!<br>
Come here!<br>
Sit here!<br>
The apple is in the box<br>
The cat is in the box<br>
The dog is under the sofa<br>
The ball is under the fridge<br>
This is tall<br>
This is big<br>
I like this sound <br>
I don't like this sound <br>
I love Chippy [après qu'il a fait qqch que le joueur a aimé] <br>
I hate Chippy [après qu'il a fait qqch que le joueur a détesté] <br>
You are noisy [dit au chien] <br>
You are fun [dit au chien] <br>
"Yes!" <br>
"No!" <br>
"Where?" <br>
"There!" <br>


### Difficultés rencontrées

<!-- > À compléter uniquement si des obstacles ont eu un impact réel
> sur l’avancement du projet. -->

!!! warning "Difficultés"
    - Limitations de la gestion du cache sur Firefox