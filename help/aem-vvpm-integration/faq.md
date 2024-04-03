---
title: FAQ sur l’intégration de Veeva Vault
description: FAQ sur l’intégration de Veeva Vault
exl-id: c308ebb3-7881-4094-9f35-c67a96fb5ab1
source-git-commit: e4a5e55ac9b79a8de7dfa8ddd3d0ad99560917b8
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 1%

---

# Questions fréquentes

**Quelles métadonnées doivent être synchronisées avec Veeva ?**

Il est important de comprendre les métadonnées en fonction du type de contenu (promotions, par exemple) dans le portail Veeva. Après avoir consulté le portail Veeva, construisez le schéma de métadonnées de contenu dans AEM afin de contenir toutes les métadonnées pertinentes pour chaque ressource/page et configurez l’intégration pour mapper les métadonnées entre les deux systèmes.

**L’intégration prend-elle en charge les documents liés à Veeva ? Dans le cas contraire, quels types de relations sont pris en charge ?**

Nombre Voir [Documentation de Veeva](https://vaulthelp2.vod309.com/wordpress/admin-user-help/documents-admin-user-help/about-document-relationships/). Le document lié (type de relation de référence) est l’un des types de relation standard qui ne peuvent pas être créés ou supprimés via l’API, car ils ont un comportement Vault spécial. Les composants, les documents annexes et tout autre élément non répertorié dans cette liste doivent pouvoir être configurés via la configuration AEM cloud Veeva.

**L’intégration prend-elle en charge le contenu modulaire AEM ?**

Oui, l’intégration prend en charge AEM fragments de contenu et d’expérience.

**L’intégration prend-elle en charge le contenu modulaire Veeva ?**

Non, pas pour le moment.

**L’intégration synchronise-t-elle les annotations visuelles de Veeva avec AEM ?**

Non, pas pour le moment. Les annotations visuelles ne sont accessibles que via l’API en tant que PDF.

**Comment définir les autorisations sur les documents VVPM synchronisés par l’intégration ?**

L’intégration utilise un utilisateur de service pour charger des documents via l’API.  Les règles de remplacement et de défaut des documents (rôles par défaut sur les documents) ne sont prises en charge que dans l’interface utilisateur VVPM et ne sont pas appliquées lors de l’utilisation de l’API. Il est recommandé d’utiliser le contrôle d’accès dynamique (DAC) pour les affectations de rôles. Le contrôle d’accès est appliqué par l’intermédiaire de tous les points de contact, y compris l’API. [Consultez la documentation ici.](http://vaulthelp2.vod309.com/wordpress/admin-user-help/ah-user-permissions-access-control/about-dynamic-access-control-for-documents/)

**L’intégration prend-elle en charge plusieurs instances VVPM ?**

L’intégration utilise une approche de configuration cloud qui permet à plusieurs points d’entrée Veeva d’être configurés à partir d’une instance AEM.

**L’intégration prend-elle en charge AEM publication ?**

Non, cette intégration fonctionne uniquement avec AEM auteur. Il est destiné à faciliter les cycles de révision MLR avant la publication du contenu.
