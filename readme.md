# NavexWp2 - Extension WooCommerce de Suivi de Livraison

## Description

NavexWp2 est une extension pour WooCommerce qui intègre le service de livraison Navex à votre boutique. Elle vous permet de gérer la création d'expéditions, de suivre les colis et de synchroniser les statuts de livraison directement depuis votre tableau de bord WordPress.

## Fonctionnalités

*   **Intégration API :** Connectez facilement votre boutique à l'API Navex via une page de configuration simple.
*   **Création d'Expéditions :**
    *   Créez une expédition et obtenez un numéro de suivi directement depuis la page de détail d'une commande.
    *   Générez des expéditions en masse pour plusieurs commandes en une seule fois depuis la liste des commandes.
*   **Suivi de Colis :**
    *   Vérifiez le statut de livraison d'un colis à tout moment.
    *   Affichez les informations de suivi (code, lien, statut) dans les détails de la commande.
*   **Synchronisation Automatique :** Un processus automatisé vérifie périodiquement le statut des livraisons et met à jour le statut de la commande WooCommerce en "terminée" lorsque le colis est livré.
*   **Statut de Commande Personnalisé :** Ajoute un statut "En attente de validation par l'administrateur" pour un meilleur contrôle du flux de commandes.

## Installation

1.  Téléchargez le fichier `.zip` du plugin.
2.  Depuis votre tableau de bord WordPress, allez dans `Extensions` > `Ajouter`.
3.  Cliquez sur `Téléverser une extension` et sélectionnez le fichier `.zip` que vous avez téléchargé.
4.  Cliquez sur `Installer maintenant`, puis sur `Activer`.

## Configuration

1.  Une fois le plugin activé, allez dans `WooCommerce` > `NavexWp Settings`.
2.  Remplissez les champs suivants avec vos informations d'identification Navex :
    *   **API Endpoint :** L'URL de base de l'API Navex.
    *   **API Username :** Votre nom d'utilisateur pour l'API.
    *   **API Key :** Votre clé d'API.
    *   **Designation :** Une désignation par défaut pour vos envois.
3.  Cliquez sur `Enregistrer les modifications`.

## Utilisation

### Créer une expédition pour une seule commande

1.  Allez sur la page de détail d'une commande WooCommerce.
2.  Dans la section "NavexWp Tracking" sur le côté, cliquez sur le bouton `Get Code`.
3.  Le plugin contactera l'API Navex, créera l'expédition et remplira automatiquement le code et le lien de suivi.

### Créer des expéditions en masse

1.  Allez dans la liste des commandes (`WooCommerce` > `Commandes`).
2.  Cochez les cases des commandes que vous souhaitez expédier.
3.  Cliquez sur le bouton `Shipping Navex` en haut de la page.
4.  Confirmez l'action. Le plugin créera une expédition pour chaque commande sélectionnée.

### Suivre un colis

1.  Allez sur la page de détail d'une commande.
2.  Dans la section "NavexWp Tracking", le statut actuel est affiché.
3.  Pour rafraîchir le statut, cliquez sur le bouton `Check Status`.
