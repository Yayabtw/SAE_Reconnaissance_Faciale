# SAÉ: Modélisation mathématique<br>Reconnaissance faciale en temps réel

## Description du projet

Le but de cette SAÉ est de construire un système de reconnaissance faciale qui fonctionne en temps réel.

Le système utilise la caméra de votre PC (ou alors une caméra externe) pour capturer des images de visages. Ainsi, on pourra construire un **dataset** contenant des visages de différentes personnes associées à leurs noms.

Par la suite, on entraînera un **algorithme de classification** permettant de prédire le nom de la personne qui se trouve devant la caméra en fonction de son visage.

## Prérequis

- Python 3.8+
- Jupyter Notebook
- Bibliothèques Python : NumPy, Pandas, Scikit-learn, TensorFlow/Keras

## Algorithmes et Modèles

### Régression Logistique

La régression logistique est un modèle de classification linéaire simple mais efficace, souvent utilisé comme point de départ pour les problèmes de classification. Dans notre contexte, il sert à distinguer si une image contient ou non un visage spécifique. Ce modèle est particulièrement utile pour comprendre les bases de la classification binaire et pour établir une ligne de base de performance sur notre ensemble de données.
### Arbre de Décision

Les arbres de décision classifient les données en apprenant une série de questions à poser sur les caractéristiques des données jusqu'à ce qu'une décision puisse être prise. Ils sont visuellement intuitifs et faciles à interpréter, mais peuvent souffrir de surapprentissage si les arbres deviennent trop complexes. Dans notre projet, les arbres de décision sont utilisés pour identifier les visages en fonction des caractéristiques extraites des images.
### Réseau de Neurones (Dense)

Les réseaux de neurones denses, ou réseaux pleinement connectés, sont formés de couches où chaque neurone est connecté à tous les neurones de la couche précédente et suivante. Ces modèles sont capables de capturer des relations complexes entre les entrées grâce à leur structure profonde et à leur capacité d'apprentissage. Dans la reconnaissance faciale, ils apprennent à reconnaître des motifs complexes dans les images de visages, bien qu'ils puissent nécessiter de grandes quantités de données pour bien performer.
### Réseau de Neurones Convolutifs (CNN)

Les CNN représentent l'état de l'art pour la reconnaissance d'images. Grâce à leur architecture unique, capable d'extraire progressivement des caractéristiques de haut niveau à partir de données brutes, ils sont particulièrement adaptés à la reconnaissance faciale. Les couches convolutives filtrent les images pour en extraire des caractéristiques telles que les bords et les formes, tandis que les couches de pooling réduisent la dimensionnalité. Nous utilisons des CNN pour leur capacité à apprendre des caractéristiques faciales discriminantes, conduisant à une précision élevée dans la reconnaissance des individus.

## Consignes

1. **Comprenez les 2 notebooks** en détails, et, si besoin, débuggez-les jusqu'à ce qu'ils fonctionnent correctement (chez moi, ils marchent).
2. **Adaptez le 2ème notebook** à d'autres algorithmes de classification de votre choix, tels que la régression logistique, les arbres de décision, etc.
3. Essayer d'adapter votre système pour le **cas d'utilisation de reconnaissance binaire** suivant: le système devra répondre `admis` ou `non admis` suivant que le visage détecté est le votre ou non.
4. Documentez-vous sur les **réseaux de neurones** et essayez d'implémenter et d'intégrer un algorithme de classification par réseaux de neurones.
5. Si vous avez le temps, documentez-vous sur les **réseaux de neurones convolutionnels** (qui sont spécialisés dans le traitement des images) et essayez d'implémenter et d'intégrer un algorithme de classification par réseaux de neurones convolutionnels.
6. Rendez votre projet sous la forme d'un **répertoire GitHub** .  Votre  repo contiendra un **fichier README** (md file) et plusieurs **notebooks jupyter** (ipynb files) propres et commentés  qui présentent votre projet.
