---
product: adobe experience manager
solution: Experience Manager
description: Consultation de la documentation Experience Manager
type: Documentation
git-repo: https://github.com/AdobeDocs/adobe-consulting-services.fr-FR
index: true
source-git-commit: f491b48a151904f13becc146beab52600c9cef46
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 2%

---


# Métadonnées à usage interne

Les métadonnées dans le système de création GitHub sont hiérarchiques et sont définies selon les niveaux de précédent croissants suivants.

1. metadata.md
1. ToC
1. Article

Les métadonnées définies dans le fichier metadata.md s’appliquent à l’ensemble du référentiel, mais elles peuvent être remplacées au niveau de la table des matières et de l’article. Tout remplacement des métadonnées doit être effectué au niveau le plus bas possible.

metadata.md

* `product`
* `git-repo`
* `index: y`

ToCs

* `sub-product`
* `user-guide-title`

Article

* `title`
* `description`

Vous trouverez des informations supplémentaires sur les métadonnées dans le [guide de création interne](https://experienceleague.adobe.com/docs/authoring-guide-exl/using/authoring/metadata.html).
