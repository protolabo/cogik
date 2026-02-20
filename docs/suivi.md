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
