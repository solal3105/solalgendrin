+++
title = "Product Owner"
subtitle = "Hiveo - En cours"
tags = [
    "article",
    "Product Design",
]
date = "2019-01-01"
label = "article"
image = "/images/product_design.svg"
+++
## Hiveo c’est quoi

Lors de toute conclusion d’un contrat d’un montant supérieur ou égal à 5000€, une entreprise A (Donneur d'ordre) doit réclamer à l’entreprise B (fournisseur) certains documents, c’est ce que l’on appelle « l’obligation de vigilance ».

Hiveo est une application métier qui propose une solution de collecte de documents en vue de vérifier la conformité d’un fournisseur sur un modèle gratuit pour le l'entreprise B, appelée "déposante".

Ainsi, il existe deux types d'utilisateurs à Hiveo : 

- Les collectants, utilisateurs qui collectent les documents légaux de leurs fournisseurs
- Les déposants, utilisateurs qui déposent les documents légaux pour leurs donneurs d'ordre

L'application métier permet aux utilisateurs collectant de répondre à l'obligation de vigilance à laquelle ils sont soumis dans le cadre de la relation avec leurs déposants.

Cette obligation de vigilance s'applique pour toute prestation annuelle de plus de 5000€ et doit être mise à jour tous les 6 mois, jusqu’à échéance du contrat pour chaque déposant. Pour les collectants avec un nombre conséquent de déposants, cela représente une charge de travail conséquente (mise à jour du dossier, vérifier, relances des déposants, archivage) 

D'autant plus que l’obligation de vigilance ****ne concerne pas uniquement les déposants. En effet le non respect de ces obligations peut mettre en péril les deux parties prenantes d’un contrat. De ce fait le collectant est ce que l’on qualifie de «solidairement responsable» de la vigilance ou de la négligence de son déposant.

### Les documents gérés par Hiveo

Hiveo gère trois types de document : les documents légaux, les documents complémentaires et les documents relationnels.

#### **Les documents légaux**

Les documents légaux sont les trois types de document obligatoires pour un collectant afin de respecter son obligation de vigilance. Ces derniers regroupent le justificatif d'immatriculation, l'attestation sociale de vigilance et la liste des salariés étrangers soumis à autorisation de travail.

![https://downloads.intercomcdn.com/i/o/88949650/0d933fdc4887235caddfa35a/documents+le%CC%81gaux.png](https://downloads.intercomcdn.com/i/o/88949650/0d933fdc4887235caddfa35a/documents+le%CC%81gaux.png)

Les documents légaux sont mutualisés : Si plusieurs collectants ont un compte Hiveo, un déposant ne va mettre qu'une seule fois ses documents en ligne. Ils seront accessibles par l'ensemble des entités qui en font la demande.

#### **Les documents complémentaires**

Les documents à ajouter par un déposant dépendent des souhaits des collectants avec lesquels il travaille. Les documents complémentaires sont mutualisés. Par exemple, si plusieurs collectants demandent une attestation de responsabilité civile professionnelle, cette pièce ne sera à mettre qu'une seule fois en ligne. A noter que, bien que mutualisés, ces documents ne sont accessibles que par les collectants qui ont souhaité les collecter.

#### **Les documents relations**

Les documents relations sont les documents qui sont propres à la relation contractuelle entre un collectant et un déposant.

Ces documents peuvent être, par exemple, des conditions particulières ou un questionnaire sécurité. Ils sont le plus souvent à télécharger, à remplir et à signer électroniquement pour être validés par la plateforme.

Ces documents ne sont pas mutualisés. Ils sont visibles uniquement par le collectant qui en a fait la demande.

### Les étapes pour l'utilisateurs

Pour ce travail, nous allons nous concentrer sur l'amélioration du parcours déposant, et plus précisément sur son usage du logiciel métier lors du dépôt de documents.

Pou une plus grande compréhension du parcours global d'un utilisateur déposant, voici un User Flow récapitulatif

![../2020_experience_hiveo/Untitled.png](../2020_experience_hiveo/Untitled.png)

1. Un déposant apprend l’existence d’Hiveo
    1. Il reçoit l’email pour créer son compte
    2. Il se rend sur la page pour créer son compte
2. Le compte est créé et vérifié
    1. Il se connecte à Hiveo
    2. **Il dépose ses documents :**  le parcours est découpé en plusieurs étapes. Le déposant peut déposer plusieurs documents simultanément.

        **Ainsi la plateforme :**

        1. Affichera une page au déposant affichant toutes les actions possible pour le dépôt des documents
        2. Reconnaitra automatiquement les documents déposés
        3. Extraira les données importantes de ces documents
        4. Vérifiera les documents suivant les règles législatives en vigueur
        5. Acceptera le dépôt du document, ou demandra à l'utilisateur déposant de le vérifier.

        C’est spécifiquement sur ce premier point que va se concentrer l’audit : sur le formulaire de vérification et sur la complétude des informations manquantes.

3. Il est relancé automatiquement par mail pour mettre à jour ses documents

### Persona type - Rôle déposant

#### Connaissances

L’utilisateur qui dépose ne dispose pas nécessairement de connaissances en informatique, sur le processus de dépôt en ligne, ou encore sur le rôle d’Hiveo dans la relation. Cependant il connaît généralement bien les obligations légales qu’il à envers son client ( l’utilisateur collectant ) .

#### Rôle type

L’utilisateur type sera soit secrétaire administratif soit artisan.

#### Ambitions & frustrations

Il souhaite déposer ses documents sans peine, qu’on l’avertisse lorsqu’une action est nécéssaire sur la plateforme . En réalité, vu que ce n’est pas dans la majorité des cas son corps de métier, moins il a d’interaction avec notre plateforme, mieux c’est !

## Analyse analytique

L’équipe produit possède des outils analytiques afin d’analyser le comportement des utilisateurs sur sa plateforme. Ils sont réalisés avec la plateforme Hotjar.  Ils permettent d'avoir une vision qualitative et quantitative de l'utilisation de la plateforme. 

Parcours deposant qui neccesite 6 upload de documents.

[https://insights.hotjar.com/r?site=1735064&recording=3356963999&token=b19bc014e25f7d87427009a587e6b4a7](https://insights.hotjar.com/r?site=1735064&recording=3356963999&token=b19bc014e25f7d87427009a587e6b4a7)

### Heatmap

![../2020_experience_hiveo/heatmap-5652487-scroll-desktop.jpg](../2020_experience_hiveo/heatmap-5652487-scroll-desktop.jpg)

### Cliques de souris

![../2020_experience_hiveo/heatmap-5652487-movement-desktop-3.jpg](../2020_experience_hiveo/heatmap-5652487-movement-desktop-3.jpg)

### Mouvement de souris

![../2020_experience_hiveo/heatmap-5652487-movement-desktop-4.jpg](../2020_experience_hiveo/heatmap-5652487-movement-desktop-4.jpg)

Retour sur 878 utilisateurs desktop

## Analyse Ergonomique

Une analyse approfondie du contexte d'usage et de l'utilisation actuelle de la plateforme nous a permis de confronter les parcours utilisateurs désirés de l'expérience vécue. Nous nous sommes basés sur les heuristiques de Bastien et Scapin pour structurer nos problématiques en thématiques.

Afin d'identifier les différents points de frustration que rencontre les déposants à cette étape du parcours, nous allons extraire les différents problèmes de l'interface en nous basant sur les critères d'évaluation de **Bastien & Scapin.**

Ci-dessous notre analyse à chaud des critères de Bastien & Scapin **pour évaluer une interface utilisateur :**

[Bastien__Scapin.pdf](../2020_experience_hiveo/Bastien__Scapin.pdf)

## Hypothèses

Les métriques quantitatives, croisées aux analyses qualitatives de l'usage qui est fait de la plateformes, nous ont permis de définir des hypothèses quiu seront une base de travail pour la définition de nos user stories.

→ Restructurer le Dashboard permet d'améliorer l'expérience utilisateur du déposant, ce qui permettra de diminuer le nombre d'appel au support d'Hiveo

→ Améliorer la structure de l'information permettra d'améliorer le taux de complétude des documents (qui est un facteur différenciant d'Hiveo)

→ Afficher l'ensemble des versions des documents déposés par l'utilisateur permettra de réduire la friction utilisateur ce qui permettra de réduire la dette technique liée aux documents déposés inutilement (ou par erreur)

## Glossaire

Afin d'améliorer la compréhension commune du document et des spécifications nous avons préparé un glossaire correspondant au langage utilisé au sein d'Hiveo.

[Copy of Glossaire](https://www.notion.so/49bc68ef02b64ec48f1fa2bc928a0b0f)

---

## Préconisations

Nous avons choisi de regrouper l'ensemble de ses tickets au sein d'un unique épique appelé "Amélioration des taux de complétude".

4 axes majeurs ont étés identifiés dans l'épique :

- Améliorer l'architecture de l'information de l'affichage des révisions
    - Impact technique conséquent : afficher l'ensemble des révisions nécessite de passer sur une base de donnée temporelle, ce qui nécessite un rework technique du calcul de l'état des dossiers
    - Valeur dégagée pour l'utilisateur déposant conséquente, L'utilisateur pourra désormais visualiser l'ensemble des révisions opérationnel courantes. Ce qui lui permettra d'avoir une meilleure visualisation de l'état de son dossier et une meilleure compréhension des actions a effectuer.
- Afficher les révisions futures
    - Impact technique modéré, fonctionnalité déjà existante mais les révisions ne peuvent s'afficher du à l'impossibilité du back de communiquer plus d'une révision avec le front. Il s'agit donc de faire disparaitre la notion "singleActive".
    - Valeur dégagée pour l'utilisateur modérée, ce travail permettra de diminuer la frustration utilisateur engendrée par le l’absence d'affichage d'une révision futures dans certains cas de figures.
- Afficher les révisions passées
    - Impact technique Conséquent, non borné du au manque d'analyse technique sur le sujet, pas d'existant applicatif
    - Valeur utilisateur collectant modéré : permettrai au collectant de visualiser l'ensemble des révisions pour un document lors des 5 dernières années directement directement depuis l'interface lors d'un contrôle d'une institution étatique de contrôle par exemple
- Retravailler la section de dépôt du document
    - Impact technique faible ce sujet nécessite uniquement du développement Front-end qui pourra être réalisé par un développeur junior à la fin de sa montée en compétence
    - valeur utilisateur déposant conséquente, ce redesign permettra de réduire le nombre de cas où l'utilisateur cherche où il doit déposer ses documents et de diminuer la frustration engendré par une architecture de l'information non pertinente pour les cas d'usages soulevés lors de l'analyse analytique

    ![../2020_experience_hiveo/IMG_6D7D742D8601-1.jpeg](../2020_experience_hiveo/IMG_6D7D742D8601-1.jpeg)

Chaque préconisation est accompagnée d'une User story, d'un indicateur d'importance, d'une maquette et enfin des règles de fonctionnements désirés d'un point de vue utilisateur. 

**Préconisations completes :** 

[Prconisations.pdf](../2020_experience_hiveo/Prconisations.pdf)

## KPIs

Afin de mesurer la vérification de ses Hypothèses nous allons suivre 4 KPIs :

→ Le `NPS` (Net Promoter Score)

→ Le `taux de complétude` des documents moyen des déposants

→ Le nombre de conversation intercom avec le flag `annule_remplace`

---
