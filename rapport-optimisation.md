# Rapport d’optimisation du projet ScrollyTelling

[Page Speed Insights - Rapport du 12 mai 2024, 20:23:33](https://pagespeed.web.dev/analysis/https-delphine-tim-momo-com/h6nzvjqsj1?form_factor=mobile)

## Problème #1

### Dimensionnez correctement les images

La taille de certaines images est très grande, alors que je n'ai pas besoin qu'elles soient aussi grandes. Plus les images sont grandes, plus elles sont lourdes.

### Action concrète pour résoudre le problème

Pour optimiser, je vais devoir réduire la taille des images pour qu’elle soit moins lourde. Puisque je n’ai pas besoin que certaines de mes images soient aussi grandes, je vais donc réduire leur format. Les images vont donc passer de plus de 2000 pixels en largeur à 750 pixels.

### Résultat
Cela a amélioré la performance sur mobile et sur desktop. Ça indique que deux images pourraient être réduites encore davantage, donc je pourrais envisager de le faire. Le score total est passé d'environ 50% à 76% sur mobile. En utisant les ordinateurs de l'école, ce chiffre passe plutôt à 

## Problème #2

### Différez le chargement des images hors écran

Les images se chargent toutes en même temps, même si on ne les voit pas, ce qui peut ralentir le temps de chargement d'une page, surtout sur des appareils mobiles ou des connexions internet plus lentes.

### Action concrète pour résoudre le problème

Je vais ajouter dans les balises `<img>` dans le HTML un attribut `loading="lazy"`, ce qui va permettre aux images de se charger seulement lorsque l'utilisateur s'apprête à les voir, donc progressivement.

### Résultat
Cela a amélioré la performance du site et les images se chargent progressivement.

## Problème #3

### Diffusez des images aux formats nouvelle génération

Certains formats d'images sont plus lourds que d'autres et peuvent  ralentir le chargement d'une page. Il existe d'autres formats qui peuvent réduire la taille des images en gardant la qualité, comme `.webp`.

### Action concrète pour résoudre le problème

Je vais modifier le format de certaines images qui semblent plus lourdes et qui utilisent un ancien format en format `.webp`. Ça va permettre d'améliorer les performances de chargement de la page tout en gardant une qualité d'image.

### Résultat
Cela a amélioré les performances du site web. Certaines images n'ont pas encore été changées en .webp, car cela ne fonctionnait pas (images de fond). Éventuellement, il serait pratique de changer leur format également.

## Rapport projet ScrollyTelling après optimisation

[Page Speed Insights - Rapport du 13 mai 2024, 13:03:02](https://pagespeed.web.dev/analysis/https-delphine-tim-momo-com/6mee6d0p3s?form_factor=desktop)