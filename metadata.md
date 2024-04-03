---
product: adobe experience manager
solution: Experience Manager
description: Documentation du Experience Manager de conseil
type: Documentation
git-repo: https://github.com/AdobeDocs/adobe-consulting-services.fr-FR
index: y
source-git-commit: e2dac4b36fb94d72b72ef6f73a77e3f566539444
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 54%

---


# Métadonnées pour utilisation interne

Dans le système de création GitHub, les métadonnées sont hiérarchisées et définies selon les niveaux de précédent croissants suivants.

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

Vous trouverez des informations supplémentaires sur les métadonnées dans la section [guide de création interne](https://experienceleague.adobe.com/docs/authoring-guide-exl/using/authoring/metadata.html).
