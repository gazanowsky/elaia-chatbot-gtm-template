# elaia-chatbot-gtm-template

## Description

Ce fichier JSON permet d'importer les balises nécessaires à la mise en place du suivi des événements du chatbot Elaia. 
Des événements sont envoyés à GA4 conformément au plan de taggage plus bas. 

## Plan de taggage 

| Étape                             | Objectif                                                                 | Nom de la balise                   | Déclencheur                          | Variables / Exemple dataLayer                                                                                         |
|----------------------------------|--------------------------------------------------------------------------|----------------------------------|------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| **Ouverture (clic)**              | Suivre le nombre d’utilisateurs qui interagissent via le chatbot (bulle) | GA4 - Event - elaia_open         | Clic sur la bulle                   | `dataLayer.push({'event':'elaia_open'});`                                                                             |
| **Lancement d’une conversation** | Suivre quand un utilisateur lance une conversation                       | GA4 - Event - elaia_conversation_started | Clic sur le bouton "Discuter maintenant" | `dataLayer.push({'event':'elaia_conversation_started'});`                                                             |
| **Choix du contact**              | Connaître le nombre de demandes de contact et la méthode utilisée        | GA4 - Event - elaia_contact      | Clic sur un bouton de contact      | `dataLayer.push({'event': 'elaia_contact', 'contact_method': 'email'});` (contact_method peut être 'email', 'whatsapp', 'messenger') |
| **Interactions avec la FAQ**     | Compter les interactions FAQ et identifier les questions les plus consultées | GA4 - Event - elaia_faq          | Clic sur une section FAQ déroulée  | ```dataLayer.push({<br>  'event': 'elaia_faq',<br>  'index': 0,<br>  'question': 'Quelles sont les horaires de réception?'<br>});``` |
| **Retour à l’accueil depuis la messagerie** | Compter le nombre de retours à l'accueil depuis la messagerie             | GA4 - Event - elaia_back         | Clic sur "Retour à l’accueil"      | `dataLayer.push({'event':'elaia_back'});`                                                                              |


## Instructions d'installation 

1. Télécharger le fichier JSON [Elaia]([url](https://github.com/gazanowsky/elaia-chatbot-gtm-template/blob/main/elaia-gtm-template.json))
