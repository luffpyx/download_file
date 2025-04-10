# download_file
module python qui permet de telecharger des fichier python leger et volumineux 100% fiable lors d'une communication reseau utilisant les sockets

Un outil de transfert de fichiers sécurisé avec suivi de progression entre client et serveur, implémenté en Python.

## Fonctionnalités principales
- **Envoi de fichiers** avec vérification d'existence
- **Réception de fichiers** avec indicateur de progression
- Gestion de la taille des fichiers via struct
- Marqueur de fin de fichier `<EOF>` pour une transmission fiable
- Barre de progression en temps réel avec tqdm

## Structure du code
```python
# Fonction d'écriture de fichier (Réception)
def WriteFile(command, client):
    # Vérification existence fichier
    # Réception taille fichier
    # Téléchargement avec barre de progression

# Fonction de lecture de fichier (Envoi)
def ReadFile(command, client):
    # Vérification existence locale
    # Envoi métadonnées
    # Transfert par blocs de 1024 octets

Prérequis

    Python 3.6+

    Bibliothèque tqdm : pip install tqdm

Utilisation typique

    Client connecté au serveur

    Commande read nom_fichier pour envoyer un fichier

    Commande write nom_fichier pour recevoir un fichier

    Transfert avec vérification d'intégrité

Avantages

    Transfert fiable grâce au marqueur de fin <EOF>

    Suivi précis de la progression

    Gestion des erreurs de fichier introuvable

    Transfert par morceaux pour faible consommation mémoire
