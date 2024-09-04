# Projet Eyes : Gestion de la Centralisation des Logs avec Docker

## Contexte d'entreprise

**Entreprise :** Zentech  
**Contexte :** Zentech est une entreprise spécialisée dans la fourniture de solutions de sécurité informatique. L’entreprise a récemment subi une série d'incidents de sécurité qui ont mis en lumière la nécessité de centraliser la gestion des logs pour améliorer la détection des menaces et la réponse aux incidents.  
**Rôle des étudiants :** Vous êtes un membre de l'équipe des experts sécurité chez Zentech. Votre manager, **Solène**, Directrice de la Sécurité de l'Information, vous a demandé de mener une étude approfondie sur la mise en place d'une solution de centralisation des logs. Cette étude doit être accompagnée par un POC (proof of concept) de la solution que vous recommanderez.

**Scénario :**  
Solène vous a assigné plusieurs tâches critiques pour évaluer la faisabilité de cette solution. Vous devrez démontrer votre expertise technique, évaluer les options possibles, et fournir des recommandations claires basées sur vos résultats. Cette étude doit être présentée par toute votre équipe.

---

## Etapes

### Partie 1 : Etude

1. **Les solutions possibles**  
   Enumérez trois solutions possibles de centralisation et de gestion des logs. Une solution basée sur un Cloud PRovider, une solution basée sur un logiciel commercial et une solution basée sur un ou plusieurs logiciels open source.
   Pour chaque solution, proposez maximum 2 slides PPT mettant en avant une description de la solution et son niveau de compléxité d'installation et de maintenance, un schéma d'architecture de la solution ainsi qu'une étude simple des coûts.
   
 2. **Le comparatif**  
   Présentez un comparatif de vos solutions proposées (sous forme d'un slide PPT contenant un tableau comparatif). Choisissez les dimension de comparaison que vous jugerez pertinents.
   Mettez en avant la solution ELK (open source) et défendez ses avantages.

## POC
La solution retenue que vous souhaitez lui dédier un POC est une plateforme ELK (Elasticsearch, Logstash et Kibana).

### Partie 1 : Installation de Docker

1. **Installation sur Windows**  
   Documentez les étapes d'installation de Docker sur un poste de travail Windows. Énumérez les étapes précises à suivre pour installer Docker Desktop, incluant toute vérification post-installation nécessaire.

2. **Installation sur Linux**  
   Le département DevOps a plusieurs serveurs Linux. Mme. Dupont souhaite savoir comment installer Docker sur ces systèmes.   
   Expliquez comment installer Docker sur une machine Linux basée sur Debian/Ubuntu. Indiquez également comment vérifier que Docker est correctement installé et comment configurer l'utilisateur pour exécuter Docker sans utiliser de sudo.

### Partie 2 : Configuration de la centralisation des logs

3. **Configuration de l'infrastructure Docker**   
   Rédigez un fichier `docker-compose.yml` qui permet de déployer Elasticsearch, Logstash, et Kibana sur un réseau Docker dédié. Assurez-vous que les conteneurs puissent communiquer entre eux.

4. **Configuration de Logstash**  
   Solène souhaite comprendre comment les logs des conteneurs Docker seront collectés par Logstash.  
   Rédigez un fichier de configuration `logstash.conf` qui permettra de collecter les logs des conteneurs Docker et de les envoyer à Elasticsearch. Expliquez également les principaux paramètres de cette configuration. (max 2 slides PPT)

5. **Déploiement d'une application générant des logs**  
   Pour tester la solution de centralisation des logs, il est nécessaire de déployer une application qui génère des logs.  
   Déployez une application simple (par exemple, un serveur Nginx) sur le réseau Docker. Décrivez les commandes utilisées pour ce déploiement et expliquez comment vérifier que les logs sont bien collectés par Logstash. (max 1 slide ppt)

### Partie 3 : Analyse des logs et recommandations

6. **Accès et configuration de Kibana**  
   Décrivez comment accéder à Kibana et configurer un index pattern pour visualiser les logs collectés. Quels sont les éléments clés à vérifier dans Kibana pour s'assurer que la configuration est correcte ?

7. **Analyse des logs**  
   Vous avez détecté des anomalies dans les logs générés par l'application Nginx (Par exemple des erreur 500 ou 403).  

   En utilisant Kibana, identifiez et décrivez une ou deux anomalies potentielles que vous pourriez rencontrer dans les logs (par exemple, tentatives d'accès non autorisées). Proposez des mesures correctives pour chaque anomalie détectée.

8. **Recommandations finales**  
   Sur la base de votre expérience Solène vous demande de fournir des recommandations pour l'implémentation de cette solution à l'échelle de l'entreprise.  
 
   Rédigez une courte recommandation (2 slides max) qui résume les avantages de la centralisation des logs via ELK, les défis potentiels à anticiper, et les bonnes pratiques pour une mise en œuvre réussie.



### Présentation et envoi des PPT

- Chaque équipe doit présenter son étude collectivement et une démonstration de ses travaux dans un temps définit.
- Les PPT doivent être envoyés à l'intervenant : raouf.amdouni@intervenants.efrei.net
