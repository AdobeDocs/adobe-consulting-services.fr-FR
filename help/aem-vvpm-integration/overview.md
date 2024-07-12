---
title: Présentation de l’intégration de Veeva Vault
description: Présentation de l’intégration de Veeva Vault
exl-id: 52cc7290-b7e1-4476-877f-48934e6daf68
source-git-commit: 2e47baa4a255c34b3ca0b8631650dd5d8960fea8
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# Prise en main de l’intégration de Veeva Vault PromoMats et Adobe Experience Manager

Cette intégration va gérer votre contenu, appliquer les droits et la conformité tout en tirant parti de la priorité dans la diffusion de l’expérience de classe.

Cette intégration requiert les versions logicielles minimales suivantes :

* Adobe Experience Manager, 6.5.5+
* Veeva Vault PromoMats, 20R3.2+

>[!NOTE]
>
>Les utilisateurs du service et les autorisations appropriées sont requis dans les deux systèmes pour l’intégration.
>

>[!IMPORTANT]
>
>Cette fonctionnalité n’est pas disponible en standard dans le cadre du produit. La mise en oeuvre nécessite un contrat de maintenance Adobe Consulting. Veuillez contacter votre représentant Adobe pour en savoir plus.
>

## Principes et fonctionnalités

Cette intégration est conçue pour prendre en charge deux cas d’utilisation principaux :

1. Validation du contenu : lorsque du nouveau contenu a été créé ou que du contenu existant a été modifié dans AEM, le contenu doit être approuvé pour être utilisé dans VVPM, dans le cadre du processus d’approbation médicale, juridique, réglementaire (MLR) pour les sciences de la vie.
1. Gestion de contenu : garantissez la visibilité de l’utilisation des ressources en établissant des relations dans PromoMats entre les tactiques numériques (p. ex. email, présentations, sites web) et leurs éléments (p. ex. logos, photographie, graphiques) créés dans AEM pour les documents provenant d’AEM.

Les avantages incluent :

* Conserver une seule source de vérité pour les ressources et le contenu sans duplication dans les référentiels numériques.
* Exploitation de Veeva Vault pour la gestion des droits et de la conformité et des AEM pour le meilleur en matière de classe et de création/diffusion de ressources et de contenu.
* Permet d’automatiser le déplacement du contenu et des métadonnées entre AEM et Veeva Vault.
* Réduit les efforts manuels liés à l’envoi de contenu à Veeva pour les workflows d’approbation.
* Chaque système est utilisé pour ses points forts et le connecteur aide à déplacer automatiquement le contenu entre les systèmes pour accélérer le délai de mise sur le marché.

Que fait l’intégration ?

* Prend en charge l’envoi AEM pages de site, Assets, fragments de contenu et fragments d’expérience à VVPM. AEM pages, fragments de contenu et fragments d’expérience peuvent être envoyés sous forme de PDF de capture d’écran ou d’images. Les fichiers binaires AEM Assets sont envoyés tels quels.
* Prend en charge la synchronisation manuelle et automatisée de certains éléments de métadonnées configurables d’AEM à VPM.
* Prend en charge la synchronisation manuelle et automatisée de certains éléments de métadonnées configurables de VPM à AEM.
* Prend en charge les relations entre AEM pages de site, Assets, fragments de contenu et fragments d’expérience dans VVPM afin d’automatiser les relations de contenu.
* Prend en charge la génération de rendu pour plusieurs types d’appareils.

>[!NOTE]
>
>Pour plus d’informations sur les options de configuration, voir la documentation sur l’utilisation de l’intégration .
>

Que NE fait PAS le connecteur ?

* Ne reproduit pas les processus AEM et les fonctionnalités de Veeva ou vice versa.
* Ne fait pas le MLR seul. Il contribue à l’automatisation de l’envoi de contenu à Veeva là où MLR se produit.
* Non destiné à créer une configuration identique entre AEM et Veeva. Tout le contenu n’a pas besoin de se déplacer entre les deux plateformes.


>[!IMPORTANT]
>
>Cette intégration considère actuellement l’AEM comme la source de vérité pour la synchronisation de contenu.

## Obtention de l’intégration

Pour configurer cette intégration, vous devez suivre les étapes ci-dessous.

Pour demander et configurer l’intégration, veuillez consulter les détails de l’organigramme et de l’organigramme ci-dessous.

![Demander l’accès](assets/integration-request.png)

Détails de l’organigramme (mise en correspondance avec les étapes ci-dessus) :

* **Étape 1** - On suppose que vous disposez déjà, ou êtes en train d&#39;acheter, d&#39;une licence pour Veeva Vault PromoMats et pour Adobe Experience Manager.
* **Étape 2** - Pour tirer parti de l’intégration, une nouvelle commande client qui décrit un accord de maintenance avec Adobe Consulting devra être signée.
* **Étape 3** - Installation, activation et configuration du package d’intégration.

## Assistance

La section suivante décrit comment contacter et consigner un problème avec l’équipe d’assistance.

### Demande d’intégration ou d’assistance Adobe Experience Manager

Les tickets d’assistance peuvent être consignés auprès de l’assistance clientèle d’Adobe. Votre administrateur Adobe Experience Cloud devra se connecter à [Adobe Admin Console](https://adminconsole.adobe.com/), cliquer sur l’onglet Assistance et créer un cas. Pour tout problème lié à l’intégration, veillez à inclure les informations suivantes :

* **Titre du processus** : `AEM - Veeva Vault Integration`
* **Propriétaire du processus** : `Data Engineering`
* **Description** : `Description of the issue`
* **Point de contact** : `The email address(es) for relavant AEM point of contacts for your organization.`
* **AEM URL de l’instance** : `Place the Adobe Experience Manager instance url here.`
* **URL de l’instance de Veeva** : `Place the Veeva Vault PromoMats instance url here.`

### Demande de prise en charge de PromoMats de Veeva Vault

Parfois, le problème rencontré est un problème lié au fonctionnement de l’instance PromoMats de Veeva Vault. Si c&#39;est le cas, il se peut que votre administrateur de PromoMats Veeva Vault soit invité à créer un ticket d&#39;assistance avec l&#39;[assistance Veeva](http://support.veeva.com/). Vous pouvez consulter l’état de l’instance Veeva en accédant à [Veeva Trust](http://trust.veeva.com/).

