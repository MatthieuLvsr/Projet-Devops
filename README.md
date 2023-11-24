# Projet-Devops

## GitFlow
Ce projet suit un modèle GitFlow pour la gestion du code source. Le GitFlow définit un ensemble de branches pour organiser le développement, les versions et les corrections de bugs.

### Branches Principales
- master : Branche principale contenant le code en production, représentant les versions stables livrées.
- develop : Branche de développement pour l'intégration continue du travail en cours.

### Branches de Fonctionnalités
- feature/ : Les branches de fonctionnalités sont créées à partir de develop pour développer de nouvelles fonctionnalités ou travailler sur des tâches spécifiques. Une fois terminées, elles sont fusionnées dans develop.

### Branches de Préparation de Version
- release/ : Les branches de préparation de version sont créées à partir de develop pour préparer une nouvelle version pour le déploiement. Elles permettent des tests finaux et des corrections de bugs mineurs avant la fusion dans master.

### Branches de Correction de Bugs
- hotfix/ : Les branches de correction de bugs sont créées à partir de master pour résoudre des problèmes critiques en production. Elles sont ensuite fusionnées dans master et develop.

### Règles de Protection des Branches
La branche master est protégée, nécessitant des validations pour être fusionnée.
Les branches de version (release/*) nécessitent des validations pour garantir la stabilité avant la fusion dans master.
Les branches de fonctionnalités (feature/*) peuvent être fusionnées dans develop après revue de code.