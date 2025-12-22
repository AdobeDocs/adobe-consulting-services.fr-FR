---
product: adobe experience manager
solution: Experience Manager
description: Consultation de la documentation Experience Manager
type: Documentation
git-repo: https://github.com/Adobe-Enterprise-Docs/adobe-consulting-services.fr-FR
index: y
hide: n
source-git-commit: d36298f9c8abf2859e2a8fc9be92d2fcae8d60cf
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 54%

---


# Métadonnées pour utilisation interne

Les métadonnées dans le système de création GitHub sont hiérarchiques et sont définies selon les niveaux de précédent croissants suivants.

1. metadata.md
1. Table des matières
1. Article

Les métadonnées définies dans le fichier metadata.md s’appliquent à l’intégralité du référentiel, mais peuvent être remplacées aux niveaux de la table des matières et de l’article. Tout remplacement des métadonnées doit être effectué au niveau le plus bas possible.

metadata.md

* `product`
* `git-repo`
* `index: y`

Tables des matières

* `sub-product`
* `user-guide-title`

Article

* `title`
* `description`

Vous trouverez des informations supplémentaires sur les métadonnées dans le [guide de création interne](https://experienceleague.adobe.com/docs/authoring-guide-exl/using/authoring/metadata.html).
