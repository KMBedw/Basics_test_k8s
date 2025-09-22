# Questions sur Kubernetes

Ce document contient une série de questions qui vous guideront à travers les différentes étapes d'apprentissage de Kubernetes, en suivant le guide pratique du fichier readme.md.

## Prérequis

1. Quels sont les trois outils essentiels à installer avant de commencer à travailler avec Kubernetes ?
2. Comment vérifier que Docker est correctement installé sur votre système ?
3. Comment vérifier que Minikube est correctement installé et fonctionne sur votre système ?
4. Comment vérifier que kubectl est correctement installé et configuré pour communiquer avec votre cluster ?

## 1. Création et déploiement d'une image Docker

1. Qu'est-ce qu'un Dockerfile et à quoi sert-il ?
2. Quelles sont les principales instructions que l'on retrouve dans un Dockerfile ?
3. Comment construire une image Docker à partir d'un Dockerfile ?
4. Comment tagger une image Docker avec un nom spécifique ?
5. Comment pousser une image Docker vers Docker Hub ?
6. Pourquoi est-il important de se connecter à Docker Hub avant de pousser une image ?
7. Comment vérifier qu'une image a été correctement poussée vers Docker Hub ?

## 2. Comprendre et créer un Pod Kubernetes

1. Qu'est-ce qu'un Pod dans Kubernetes ?
2. Pourquoi dit-on que le Pod est l'unité de base dans Kubernetes ?
3. Quelles sont les principales sections d'un fichier YAML définissant un Pod ?
4. Quelle est la différence entre les sections `metadata` et `spec` dans un fichier YAML Kubernetes ?
5. Comment créer un Pod à partir d'un fichier YAML ?
6. Comment vérifier que votre Pod a été correctement créé et est en cours d'exécution ?
7. Comment obtenir des informations détaillées sur un Pod spécifique ?
8. Comment accéder aux logs d'un Pod ?
9. Quelles sont les principales limitations des Pods individuels ?
10. Pourquoi utilise-t-on généralement des contrôleurs comme les Deployments plutôt que de gérer directement des Pods ?

## 3. Déployer l'application avec un Deployment Kubernetes

1. Qu'est-ce qu'un Deployment dans Kubernetes ?
2. Quels sont les avantages d'utiliser un Deployment par rapport à la création directe de Pods ?
3. Quelles sont les principales sections d'un fichier YAML définissant un Deployment ?
4. À quoi sert le champ `replicas` dans un Deployment ?
5. Quelle est la fonction des `labels` et des `selectors` dans un Deployment ?
6. Comment créer un Deployment à partir d'un fichier YAML ?
7. Comment vérifier que votre Deployment a été correctement créé ?
8. Comment vérifier que les Pods gérés par votre Deployment sont en cours d'exécution ?
9. Comment mettre à jour un Deployment existant ?
10. Comment faire évoluer (scale) le nombre de réplicas d'un Deployment ?

## 4. Exposer l'application avec un Service Kubernetes

1. Qu'est-ce qu'un Service dans Kubernetes ?
2. Pourquoi avons-nous besoin de Services dans Kubernetes ?
3. Quels sont les différents types de Services disponibles dans Kubernetes ?
4. Quelle est la différence entre un Service de type ClusterIP, NodePort et LoadBalancer ?
5. À quoi servent les champs `port` et `targetPort` dans un Service ?
6. Comment créer un Service à partir d'un fichier YAML ?
7. Comment vérifier que votre Service a été correctement créé ?
8. Comment obtenir l'adresse IP de Minikube ?
9. Comment accéder à votre application via le Service NodePort ?
10. Pourquoi utilise-t-on généralement des Services pour exposer des applications plutôt que d'accéder directement aux Pods ?

## 5. Test du Load Balancing

1. Qu'est-ce que le Load Balancing dans Kubernetes ?
2. Comment Kubernetes répartit-il le trafic entre plusieurs Pods ?
3. Comment pouvez-vous tester que le Load Balancing fonctionne correctement ?
4. Pourquoi est-il important d'avoir plusieurs réplicas de votre application pour le Load Balancing ?
5. Comment identifier quel Pod a traité une requête spécifique ?
6. Quels sont les avantages du Load Balancing pour la disponibilité et la performance de votre application ?

## 6. Test du Service Discovery et Rééquilibrage

1. Qu'est-ce que le Service Discovery dans Kubernetes ?
2. Comment Kubernetes gère-t-il la découverte des services ?
3. Que se passe-t-il lorsqu'un Pod géré par un Deployment tombe en panne ?
4. Comment supprimer manuellement un Pod pour tester le rééquilibrage ?
5. Comment vérifier que Kubernetes a créé un nouveau Pod pour remplacer celui qui a été supprimé ?
6. Comment vérifier que le trafic est correctement redirigé vers le nouveau Pod ?
7. Pourquoi le Service Discovery est-il important dans un environnement de microservices ?

## 7. Configuration et test d'Ingress Kubernetes

1. Qu'est-ce qu'un Ingress dans Kubernetes ?
2. Quelle est la différence entre un Ingress et un Service ?
3. Qu'est-ce qu'un Ingress Controller et pourquoi est-il nécessaire ?
4. Comment activer l'addon Ingress dans Minikube ?
5. Comment vérifier que l'Ingress Controller est correctement déployé ?
6. Quelles sont les principales sections d'un fichier YAML définissant un Ingress ?
7. À quoi servent les annotations dans un Ingress ?
8. Comment créer un Ingress à partir d'un fichier YAML ?
9. Comment vérifier que votre Ingress a été correctement créé ?
10. Comment configurer votre fichier hosts pour tester l'accès via Ingress ?
11. Quels sont les avantages d'utiliser un Ingress par rapport à un simple Service NodePort ?

## 8. Nettoyage

1. Pourquoi est-il important de nettoyer les ressources après avoir terminé vos tests ?
2. Comment supprimer un Pod spécifique ?
3. Comment supprimer un Deployment spécifique ?
4. Comment supprimer un Service spécifique ?
5. Comment supprimer un Ingress spécifique ?
6. Comment supprimer toutes les ressources créées à partir de fichiers YAML ?
7. Comment arrêter et supprimer complètement un cluster Minikube ?