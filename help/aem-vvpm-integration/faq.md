---
title: FAQ sur l'intégration Veeva Vault
description: FAQ sur l'intégration Veeva Vault
exl-id: c308ebb3-7881-4094-9f35-c67a96fb5ab1
source-git-commit: b024e4295b5b37030c1524342832400c279c650a
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 1%

---

# Questions fréquentes

**Quelles métadonnées doivent être synchronisées avec Veeva ?**

Il est important de comprendre les métadonnées en fonction du type de contenu (par exemple les promotions) dans le portail Veeva. Après avoir consulté le portail Veeva, créez le schéma de métadonnées de contenu dans AEM afin de contenir toutes les métadonnées pertinentes pour chaque ressource/page et configurez l’intégration pour mapper les métadonnées entre les deux systèmes.

**L&#39;intégration prend-elle en charge les documents liés à Veeva ? Dans le cas contraire, quels types de relations sont pris en charge ?**

Non. Voir [Documentation Veeva](https://vaulthelp2.vod309.com/wordpress/admin-user-help/documents-admin-user-help/about-document-relationships/). Le document lié (type de relation de référence) est l’un des types de relation standard qui ne peuvent pas être créés ou supprimés via l’API en raison de leur comportement spécial dans Vault. Le composant, les documents annexes et tout autre élément ne figurant pas dans cette liste doivent pouvoir être configurés via la configuration AEM Veeva Cloud.

**L’intégration prend-elle en charge le contenu modulaire d’AEM ?**

Oui, l’intégration prend en charge les fragments de contenu et les fragments d’expérience AEM.

**L&#39;intégration prend-elle en charge le contenu modulaire Veeva ?**

Non, pas pour le moment.

**L’intégration synchronise-t-elle les annotations visuelles Veeva avec AEM ?**

Non, pas pour le moment. Les annotations visuelles ne sont accessibles que via API as a PDF.

**Comment définir des autorisations sur les documents VPM synchronisés par l&#39;intégration ?**

L’intégration utilise un utilisateur du service pour charger des documents via l’API.  Les règles d&#39;affectation de valeur par défaut et de remplacement de documents (rôles d&#39;affectation de valeur par défaut aux documents) sont uniquement prises en charge dans l&#39;interface utilisateur VPM et ne sont pas appliquées lors de l&#39;utilisation de l&#39;API. Il est recommandé d’utiliser le contrôle d’accès dynamique (DAC) pour les affectations de rôles. DAC est appliqué à tous les points de contact, y compris l’API. [Voir la documentation ici.](http://vaulthelp2.vod309.com/wordpress/admin-user-help/ah-user-permissions-access-control/about-dynamic-access-control-for-documents/)

**L&#39;intégration prend-elle en charge plusieurs instances VPM ?**

L’intégration utilise une approche de configuration cloud qui permet de configurer plusieurs points d’entrée Veeva à partir d’une instance AEM.

**L’intégration prend-elle en charge la publication AEM ?**

Non, cette intégration ne fonctionne qu’avec l’auteur AEM. Il est destiné à faciliter les cycles de révision du MLR avant la publication du contenu.
