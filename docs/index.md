---
title: Vue d'ensemble du projet
---

<style>
    @media screen and (min-width: 76em) {
        .md-sidebar--primary {
            display: none !important;
        }
    }
</style>

# Vue d'ensemble du projet

!!! info "Informations générales"
    **Titre**: Cogik — Construction progressive de besoins communicatifs et de flux conversationnels  
    **Session**: Hiver 2026  
    **Auteur(s)**: Lens Durandisse  
    **Thème(s)**: Langue, Développement mobile, Génie logiciel  
    **Superviseur(s)**: Louis-Edouard Lafontant  

## Description du projet

<!-- > :bulb: N'oubliez pas d'effacer ou mettre en commentaires les notes (`>`) en début de section -->

### Contexte

Ce projet est une tentative d'explorer une façon "novatrice" d'apprendre une langue et de construire un logiciel approprié à cette fin. Je mets novatrice entre guillemets parce qu'un argument crédible pourrait être avancé pour dire qu'en réalité c'est la façon dont apprennent les bébés et les enfants, plutôt que les méthodes populaires établies de nos jours. 

Elle consiste en ceci : apprendre une langue selon nos besoins immédiats. Un enfant apprend le mot "pomme" seulement lorsqu'il ou elle en a besoin. Il apprend à dire "je m'appelle X" seulement quand il ressent le besoin de se présenter. Dans un village qui ne contiendrait qu'une poignée de personnes, il n'y aurait presque jamais vraiment le besoin de se présenter. Tout le monde connaît tout le monde. Et donc l'expression "je m'appelle X" n'existerait probablement jamais.

Apprendre "par besoins" est une approche novatrice qui diffère de l'apprentissage par mémorisation de mots et de structures grammaticales (c'est-à-dire l'approche scolaire) et de l'apprentissge par immersion (qui est elle aussi de plus en plus populaire de nos jours). 

<!-- > Présentez le contexte général dans lequel s’inscrit votre projet (social, organisationnel, technologique, éducatif, environnemental, etc.). -->


### Problématique

Ce projet présente une façon beaucoup plus intuitive d'apprendre. On commence par des besoins simples et "évidents" (le besoin de désigner des choses, "ceci est X", "elle s'appelle Y") pour prendre de plus en plus de complexité ("je ressens le besoin de manger un poulet cuit de façon traditionnelle avec ma famille habitant à la campagne")

Ce n'est pas forcément plus amusant au sens ludique, ou en tout cas pas autant que l'approche par immersion, mais c'est beaucoup plus satisfaisant puisque je crois que c'est la façon la plus naturelle d'apprendre.

Cette méthode d'apprentissage tire son intérêt entre autres des faiblesses démontrées des autres méthodes populaires. C'est une alternative intéressante ne serait-ce par ce qu'elle n'a pas encore été vraiment explorée.

Voyons les faiblesses des méthodes actuelles:
-Les inconvénients de la méthode d'apprentissage scolaire ne sont plus à présenter. La majorité des étudiants qui suivent un cours de langue dans le cadre d'un programme ou cursus scolaire en sortent avec peu de compétences réelles dans l'immédiat et oublient pratiquement tout dans les mois et années qui suivent.

En particulier, l'insistance sur l'apprentissage de la grammaire est non seulement démotivante mais aussi très peu efficace. Les études du Dr Krashen ont démontré que l'étude de la grammaire a un impact très limité sur la compétence réelle dans une langue. Les connaissances du cerveau analytique ne se transmettent pas vraiment au cerveau intuitif (celle sur laquelle on se repose en utilisant notre langue maternelle), du moins pas immédiatement et de façon limitée. Et ceci a été démontré pour des étudiants motivés, donc que dire d'apprendre une langue ainsi à une classe avec des profils divers dont la majorité n'ont pas toujours choisi d'être là? 

-Les inconvénients de l'apprentissage par immersion commencent à devenir de plus en plus visibles depuis qu'elle a commencé à se répandre au cours des dernières années suite à la montée d'internet et de la multiplication du contenu numérique en ligne. 

Bien que ce soit une méthode qui s'est révélée motivante et efficace pour une partie de la population, elle n'a pas la structure dont a besoin la majorité des gens. Les résultats prennent du temps à être visibles et elle est très chronopage dépendemment de comme elle est implémentée (tout le monde n'a pas le temps d'écouter des heures de séries télévisées tous les jours...)

Apprendre par besoins donne à la fois la structure que manque la méthode par immersion et la dopamine (du moins une partie) que manque celle par la grammaire. C'est une méthode combinant le meilleur de deux mondes.

<!-- > Décrivez le problème central ou la question de recherche que votre projet cherche à adresser, pourquoi s'y intéresser et les faiblesses des solutions actuelles. 
> Le problème doit pouvoir être compris indépendamment de la solution envisagée. -->


### Proposition et objectifs

Les objectifs de ce projet sont les suivants : 

- Créer une application suffisamment complète pour donner une bonne idée de la vision du projet (l'apprentissage par besoin) et sur le fonctionnement du dit application. Cela impliquera d'implémenter toutes les fonctionnalités et le squelette de l'application.

Bien sûr, le but n'est pas de faire une application qui implémente la vision à 100% vu le peu de temps à ma disposition. Elle pourra se contenter d'être entièrement fonctionnelle et de servir de démo convaincante. Par exemple, il va de soi que je n'aurai pas le temps de développer une application qui en avril pourra être pris en main par n'importe qui et amener une personne au niveau B1 en langue (ou même A2). Cependant, plusieurs exemples d'exercices doivent être implémentés. De plus, quelques leçons/niveaux doivent aussi être entièrement complétées. Finalement le squelette de ce que va couvrir l'application pour une langue choisie (probablement anglais) doit aussi avoir été faite (même si la majorité des leçons ne seront pas réellement implémentées en avril) 

- Créer une application ludique, agréable à utiliser et "tape à l'oeil". Je vise un design moderne du même style que des applications célèbres comme Duolingo, Lingonaut, Lingodeer. Bien sûr les animations seront beaucoup plus limitées vu le peu de temps à ma disposition.

- Montrer à quel point l'apprentissage puisse être intuitif au travers de ce qui aura été implémenté dans cette application. 

L'apprentissage par besoins, bien que structurée, demande aussi de tatônner un peu et de faire des hypothèses. Si j'apprend l'expression "Ceci est une pomme", je ne sais pas tout de suite quelle partie de l'expression réfère au fruit sphérique rouge. Est-ce le mot "ceci" ou le mot "pomme" ? De même si je dis "la pomme est tombée", je ne sais pas directement ce qui réfère à une action : le mot "est" ou "tombée" ou les 2 ? Ce sont des choses que l'utilisateur apprendra indirectement par exposition répétée et par déductions automatiques faites par le cerveau.

Le défi sera de rendre l'apprentissage assez intuitive pour que ces connexions puissent se faire. Un de mes objectifs est donc de prouver avec le peu que j'aurais implémenté que cette méthode peut être efficacement exécuté au travers de mon application. 

Il y a aussi bien sûr la question du caractère intuitif de l'utilisation de l'application elle-même (la signification des symboles, la facilité de la prise en main, etc.)
<!-- > Présentez votre proposition de projet et les objectifs visés. Expliquez en quoi votre approche répond à la problématique identifiée. 
> Assurez-vous d'avoir, dans la mesure du possible, des objectifs mesurables, raisonnnables dans le temps et non redondants entre eux. -->


### Méthodologie

<!-- > Expliquez comment vous comptez aborder le projet : démarche générale, grandes étapes prévues, itérations, types de validations envisagées. -->



### Validation et Évaluation

<!-- > Indiquez comment vous évaluerez que votre solution répond aux objectifs du projet (ex. scénarios d’usage, tests, retours utilisateurs, indicateurs qualitatifs ou quantitatifs). -->


## Équipe

Lens Durandisse: Responsable de projet

## Échéancier

!!! info
    Le suivi complet est disponible dans la page [Suivi de projet](suivi.md).

| Activités                      | Début   |   Fin   | Livrable                            | Statut      |
|--------------------------------|---------|---------|-------------------------------------|-------------|
| Ouverture de projet            | 12 jan. | 12 jan. | Proposition de projet               | ✅ Terminé  |
| Études préliminaires           | 12 jan. | 23 jan. | Document d'analyse                  | 🔄 En cours |
| Analyse des exigences          | 20 jan. | 27 jan. | Spécifications de l'extension       | 🔄 En cours |
| Prototypage                    | 27 jan. | 10 fev. | Prototype v1                        | ⏳ À venir  |
| Évaluation 1                   | 16 fev. | 20 jan. | Feedback (rapport)                  | ⏳ À venir  |
| Sprint 1                       | 16 fev. | 9 mar.  |  Extension v1                       | ⏳ À venir  |
| Évaluation 2                   | 9 mar. | 13 mar.  | Feedback (rapport)                  | ⏳ À venir  |
| Sprint 2                       | 9 mar. | 30 mar.  | Extension v2                        | ⏳ À venir  |
| Sprint 3 (peaufinement)        | 30 mar. | 17 avr. | Extension finale                    | ⏳ À venir  |
| Évaluation 3                   | 9 mar. | 13 mar.  | Feedback (rapport)                  | ⏳ À venir  |
| Présentation + Rapport         | 17 avr. | 30 avr. | Présentation + Rapport              | ⏳ À venir  |
