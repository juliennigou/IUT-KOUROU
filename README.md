# IUT-KOUROU

## Bienvenue

Bienvenue sur le dépôt pédagogique **IUT-KOUROU**.

Ce dépôt regroupe plusieurs cours et supports de travail destinés aux étudiants. La branche `main` sert de **point d'entrée** : elle présente l'organisation générale du dépôt et vous aide à retrouver le bon cours.

## Organisation du dépôt

Le principe est simple :

- **une branche correspond à un cours** ;
- la branche `main` sert d'accueil et d'orientation ;
- chaque branche de cours peut contenir son propre support, ses ressources et sa documentation.

Autrement dit, si vous cherchez le contenu d'un cours, il faut vous placer sur la branche correspondante.

## Branches de cours

### Branche actuellement disponible

- `cyclevieprojet` : cours autour du **cycle de vie projet** et de l'industrialisation d'un projet informatique.

Un accès direct est aussi disponible via [`Cycle de vie d'un projet.md`](<Cycle de vie d'un projet.md>).

### Branches prévues

D'autres branches seront ajoutées progressivement, notamment pour les cours suivants :

- **Sécuriser un système d'informatique**
- **Télédétection spatiale 1**
- **Télédétection spatiale 2**

## Comment accéder à un cours

Après avoir cloné le dépôt, vous pouvez afficher les branches disponibles :

```bash
git branch -a
```

Puis vous placer sur la branche du cours voulu :

```bash
git switch cyclevieprojet
```

Si de nouvelles branches ont été ajoutées à distance, pensez à récupérer les dernières informations :

```bash
git fetch --all
```

## Ce que vous trouverez selon les branches

Selon le cours, une branche pourra contenir :

- un support de cours ;
- des exemples ;
- des consignes ou exercices ;
- de la documentation complémentaire ;
- des fichiers utiles pour suivre le cours ou retravailler les notions.

Chaque branche peut donc avoir une structure différente, selon les besoins pédagogiques du cours concerné.

## Recommandation aux étudiants

Pour éviter les erreurs :

- vérifiez toujours sur quelle branche vous vous trouvez ;
- lisez le `README.md` de la branche du cours ;
- utilisez `main` comme page d'accueil, pas comme support principal de cours.

## En résumé

Ce dépôt est organisé pour rester simple à parcourir :

- `main` vous accueille ;
- chaque branche vous emmène vers un cours précis ;
- de nouveaux cours seront ajoutés au fur et à mesure.

Commencez donc par identifier la bonne branche, puis travaillez directement dans le cours correspondant.
