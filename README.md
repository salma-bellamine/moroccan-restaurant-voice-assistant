# Agent Conversationnel Vocal pour la Restauration (IA & LLM)

## Présentation du Projet
Ce projet consiste en la conception et le développement d'un agent vocal intelligent automatisé, destiné à gérer la prise de commande à emporter et les interactions téléphoniques pour un restaurant. Développé sur une architecture conversationnelle low-code/no-code (Rounded), l'agent est capable d'interagir naturellement en temps réel avec les clients, de structurer un menu complet, de valider des choix et de collecter des variables contextuelles.

---

## Architecture et Fonctionnement du Flux (Flows)
Le parcours conversationnel est structuré en plusieurs états logiques (nodes) connectés entre eux pour assurer une transition fluide :

1. Call Context (Initialisation) : Initialisation des variables globales nécessaires au suivi de la commande et des informations utilisateur.
2. Accueil : Salutation du client et orientation de l'appel vers la prise de commande.
3. Prise de Commande (prise_de_Commande) : 
   - Gestion d'un menu détaillé (cartes marocaine et internationale, menus spéciaux, desserts).
   - Validation stricte des items demandés par le client.
   - Stockage dynamique dans la variable choix_menue et comptabilisation du nombre de personnes dans nbre_personne.
4. Informations Personnelles (information) : 
   - Collecte du nom complet du client (nom_complet).
   - Collecte du numéro de téléphone (telphone).
5. Modification de Commande (modification_commande) : Gestion des ajouts ou des changements de dernière minute avant la validation finale.

---

## Technologies & Compétences Clés
* Intelligence Artificielle & LLM : Prompt engineering avancé, contraintes de concision (réponses brèves), gestion du contexte conversationnel.
* Architecture Vocale : Conception de machines à états conversationnelles (Nodes & Transitions).
* Gestion des Données : Routage et typage de variables personnalisées (String, Boolean).

---

## Perspectives d'Évolution
* Connexion des webhooks avec une plateforme d'automatisation (Make/Zapier) pour enregistrer automatiquement les commandes dans un fichier Google Sheets ou envoyer une alerte en cuisine.
* Intégration d'un Trunk SIP pour l'attribution d'un numéro de téléphone réel.
