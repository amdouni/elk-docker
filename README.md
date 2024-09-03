Entreprise : SecureTech Corp
Contexte : SecureTech Corp est une entreprise spécialisée dans la fourniture de solutions de sécurité informatique. L’entreprise a récemment subi une série d'incidents de sécurité qui ont mis en lumière la nécessité de centraliser la gestion des logs pour améliorer la détection des menaces et la réponse aux incidents.
Rôle des étudiants : Vous êtes un membre de l'équipe de sécurité informatique chez SecureTech Corp. Votre manager, Mme. Laura Dupont, Directrice de la Sécurité de l'Information, vous a demandé de mener une étude approfondie sur la mise en place d'une solution de centralisation des logs en utilisant Docker.

Scénario : Mme. Laura Dupont vous a assigné plusieurs tâches critiques pour évaluer la faisabilité de cette solution. Vous devrez démontrer votre expertise technique, évaluer les options possibles, et fournir des recommandations claires basées sur vos résultats. Cette étude doit être finalisée dans un délai de 3 heures.

Questions pour l'examen :
Partie 1 : Installation de Docker (20 points)
Installation sur Windows (10 points) :
Mme. Dupont vous demande de documenter les étapes d'installation de Docker sur un poste de travail Windows. Énumérez les étapes précises à suivre pour installer Docker Desktop, incluant toute vérification post-installation nécessaire. (5 points)

Question : Décrivez toutes les étapes nécessaires pour installer Docker Desktop sur un système Windows, et comment vérifier que l'installation est réussie.

Installation sur Linux (10 points) :
Le département DevOps a plusieurs serveurs Linux. Mme. Dupont souhaite savoir comment installer Docker sur ces systèmes.

Question : Expliquez comment installer Docker sur une machine Linux basée sur Debian/Ubuntu. Indiquez également comment vérifier que Docker est correctement installé et comment configurer l'utilisateur pour exécuter Docker sans utiliser de sudo.

Partie 2 : Configuration de la centralisation des logs (40 points)
Configuration de l'infrastructure Docker (10 points) :
SecureTech Corp prévoit de déployer une stack ELK pour centraliser les logs.

Question : Rédigez un fichier docker-compose.yml qui permet de déployer Elasticsearch, Logstash, et Kibana sur un réseau Docker dédié. Assurez-vous que les conteneurs puissent communiquer entre eux.

Configuration de Logstash (15 points) :
Mme. Dupont souhaite comprendre comment les logs des conteneurs Docker seront collectés par Logstash.

Question : Rédigez un fichier de configuration logstash.conf qui permettra de collecter les logs des conteneurs Docker et de les envoyer à Elasticsearch. Expliquez également les principaux paramètres de cette configuration.

Déploiement d'une application générant des logs (15 points) :
Pour tester la solution de centralisation des logs, il est nécessaire de déployer une application qui génère des logs.

Question : Déployez une application simple (par exemple, un serveur Nginx) sur le réseau Docker. Décrivez les commandes utilisées pour ce déploiement et expliquez comment vérifier que les logs sont bien collectés par Logstash.

Partie 3 : Analyse des logs et recommandations (40 points)
Accès et configuration de Kibana (10 points) :
Mme. Dupont souhaite que vous configuriez Kibana pour visualiser les logs centralisés.

Question : Décrivez comment accéder à Kibana et configurer un index pattern pour visualiser les logs collectés. Quels sont les éléments clés à vérifier dans Kibana pour s'assurer que la configuration est correcte ?

Analyse des logs (20 points) :
Vous avez détecté des anomalies dans les logs générés par l'application Nginx.

Question : En utilisant Kibana, identifiez et décrivez une ou deux anomalies potentielles que vous pourriez rencontrer dans les logs (par exemple, tentatives d'accès non autorisées). Proposez des mesures correctives pour chaque anomalie détectée.

Recommandations finales (10 points) :
Sur la base de votre expérience dans ce lab, Mme. Dupont vous demande de fournir des recommandations pour l'implémentation de cette solution à l'échelle de l'entreprise.

Question : Rédigez une courte recommandation (150-200 mots) qui résume les avantages de la centralisation des logs via Docker, les défis potentiels à anticiper, et les bonnes pratiques pour une mise en œuvre réussie.
