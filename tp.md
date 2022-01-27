
#### Membres :
Louis Huret, Steeven Michnievich, Anthony Leclerc, Julien Chassaing

# Description des tâches réalisés :

- Ajout d'un Jenkisfile dans lequel nous avons mis les différentes actions d'intégration continue.
> Nous avons fait en sorte d'avoir plusieurs stage correspondant aux différentes tâches et actions.
> Le stage **build** qui fait en sorte comme son nom l'indique de build le code du projet java et de mettre le résultat dans le dossier **target**. C'est également dans cette étape que sera gérer l'artefact permettant de retrouver cette ressource sur Jenkins par exemple.

> Nous avons ensuite l'étape de **test** permettant de tester notre code à partir des différentes fonctions de tests présente dans le projet. Et nous enregistrons les résultats de test également dans le dossier **target**.
