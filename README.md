# Cycle de vie projet

## Bienvenue

Bienvenue sur la branche `cyclevieprojet`.

Cette branche correspond au cours **Industrialiser un projet informatique**. Elle a pour objectif de vous aider à comprendre comment passer d'une idée ou d'un prototype à un projet **maîtrisé, reproductible et défendable**.

Ici, on ne s'intéresse pas seulement au code. On travaille aussi sur la façon de **cadrer un besoin**, **organiser une équipe**, **stabiliser un environnement**, **tester**, **documenter**, **déployer** et **soutenir** un projet de manière professionnelle.

## Ce que vous allez apprendre

À la fin de ce cours, vous devrez être capables de :

- analyser un besoin et clarifier le périmètre d'un projet ;
- transformer un objectif flou en livrables concrets et vérifiables ;
- organiser le travail d'équipe avec branches, tickets et merge requests ;
- rendre un projet reproductible sur plusieurs postes ;
- intégrer les tests dans le flux normal du développement ;
- produire une documentation utile pour l'équipe, les utilisateurs et les évaluateurs ;
- préparer un déploiement propre et limiter les risques de sécurité ;
- présenter un projet avec des preuves, des choix argumentés et une démonstration cohérente.

## Fil rouge du cours

Le cours suit un projet exemple appelé **ResaMat**, une application de prêt de matériel à l'IUT.

Ce fil rouge permet d'aborder de façon concrète :

- le cadrage du besoin ;
- l'organisation du dépôt ;
- la gestion des tâches et des revues ;
- la reproductibilité de l'environnement ;
- les tests ;
- la documentation ;
- le déploiement ;
- la soutenance du projet.

Des activités et comparaisons sont également proposées autour d'autres situations de projet, notamment pour apprendre à relire, critiquer et améliorer une organisation de travail.

## Thèmes abordés

Le cours couvre notamment les points suivants :

- qu'industrialiser dans un projet informatique ;
- les risques d'un projet non structuré ;
- le cahier des charges et les critères d'acceptation ;
- la collaboration d'équipe et la qualité des merge requests ;
- la maîtrise de l'environnement de travail ;
- la reproductibilité comme indicateur de maturité ;
- les tests continus et leur intégration au flux projet ;
- la documentation pour plusieurs publics ;
- le déploiement et la sécurisation minimale ;
- la soutenance comme démonstration de maîtrise ;
- la place de l'IA dans un projet et les règles d'usage à fixer en équipe.

## Support du cours

Le support principal se trouve dans [`cours/COURS.html`](/Users/juliennigou/iut-kourou/cours/COURS.html).

Il s'agit d'un support **Reveal.js** navigable dans le navigateur.

## Ouvrir le cours localement

Depuis la racine du dépôt :

```bash
git switch cyclevieprojet
cd cours
python3 -m http.server 8000
```

Puis ouvrez dans votre navigateur :

```text
http://localhost:8000/COURS.html
```

## Exporter le support en PDF

Pour générer une version PDF des slides :

1. lancez le serveur local dans le dossier `cours` ;
2. ouvrez `http://localhost:8000/COURS.html?print-pdf` ;
3. utilisez l'impression du navigateur avec l'option **Enregistrer en PDF** ;
4. choisissez de préférence le mode **paysage** et activez les **arrière-plans graphiques**.

## Attendus pour les étudiants

Ce cours vous demande de développer une posture de travail plus rigoureuse :

- expliciter vos choix ;
- rendre votre travail visible ;
- produire des preuves de qualité ;
- limiter l'improvisation ;
- construire un projet que quelqu'un d'autre peut comprendre, relancer et évaluer.

L'objectif n'est pas d'alourdir votre travail, mais de vous apprendre à produire un projet plus solide, plus lisible et plus professionnel.

## En résumé

Un bon projet ne se reconnaît pas seulement à son interface ou à quelques fonctionnalités qui marchent. Il se reconnaît au fait qu'il peut être :

- compris ;
- repris ;
- testé ;
- corrigé ;
- déployé avec méthode ;
- défendu clairement.

Cette branche est donc votre point d'entrée pour travailler cette compétence de **cycle de vie projet**.
