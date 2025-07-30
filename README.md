# elaia-chatbot-gtm-template

## Description

Ce fichier JSON permet d'importer les balises nécessaires à la mise en place du suivi des événements du chatbot Elaia. 
Des événements sont envoyés à GA4 conformément au plan de taggage plus bas. 

## Plan de taggage 

| Étape                             | Objectif                                                                 | Nom de l'événement                   |
|----------------------------------|--------------------------------------------------------------------------|----------------------------------|
| **Ouverture (clic)**              | Suivre le nombre d’utilisateurs qui interagissent via le chatbot (bulle) | elaia_open         |
| **Lancement d’une conversation** | Suivre quand un utilisateur lance une conversation                       | elaia_conversation_started |
| **Choix du contact**              | Connaître le nombre de demandes de contact et la méthode utilisée        | elaia_contact      |
| **Interactions avec la FAQ**     | Compter les interactions FAQ et identifier les questions les plus consultées | elaia_faq          |
| **Retour à l’accueil depuis la messagerie** | Compter le nombre de retours à l'accueil depuis la messagerie             | elaia_back         |


## Instructions d'installation 

#### 1. Télécharger le fichier ([elaia-gtm-template.json](https://github.com/gazanowsky/elaia-chatbot-gtm-template/blob/main/elaia-gtm-template.json))

#### 2. Aller sur https://wwww.google.tagmanager.com

#### 3. Séléctionner l'onglet **Admin** > **Importer le container**
 
   <img width="1849" height="867" alt="image" src="https://github.com/user-attachments/assets/1d803f1f-a169-45f5-8629-46ae80e2eafe" />

#### 4. Importer le fichier téléchargé puis cochez **Fusionner** et **Renommer les balises, déclencheurs et variables générant des conflits**

   <img width="1187" height="913" alt="image" src="https://github.com/user-attachments/assets/a89feb96-963a-49f3-beac-1407bb4f692d" />

#### 5. Indiquer l'ID de mesure GA4 dans la balise **GA4 - Chatbot Events (Elaia)**

<img width="1187" height="913" alt="image" src="https://github.com/user-attachments/assets/06c1bdcb-ead4-44e5-8983-35c3bcac3bc3" />


