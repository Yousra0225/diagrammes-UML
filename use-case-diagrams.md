# Use Case Diagrams

## Définition

Le **diagramme de cas d'utilisation** (use case diagram) décrit les **interactions entre les utilisateurs (acteurs)** et un **système**.  
Il ne montre pas comment le système fonctionne, mais ce qu'il permet de faire.

---

## Éléments de base

| Élément              | Symbole UML        | Description technique                                                             |
|----------------------|--------------------|------------------------------------------------------------------------------------|
| **Acteur**           | 👤 (stickman)       | Utilisateur ou système externe interagissant avec le système                      |
| **Cas d’utilisation**| ⭕ (ovale)          | Fonction offerte par le système                                                   |
| **Système**          | ▭ (rectangle)      | Conteneur des cas d'utilisation                                                   |
| **Association**      | ➖ (ligne)          | Lien entre acteur et cas d'utilisation                                            |
| **Include**          | `<<include>>`       | Une action **nécessaire** et incluse automatiquement dans une autre              |
| **Extend**           | `<<extend>>`        | Une action **optionnelle**, déclenchée dans des conditions particulières          |

---
### 🎭 Acteurs
- **Utilisateur** : peut s'inscrire, se connecter, envoyer et lire un message  
- **Admin** : peut se connecter, gérer les utilisateurs, consulter les logs

---
## 🔸 Cas d'utilisation

| Cas                           | Acteur concerné | Notes                                |
|-------------------------------|-----------------|--------------------------------------|
| S’inscrire                    | Utilisateur     |                                      |
| Se connecter                  | Utilisateur, Admin | Utilisé par les deux                |
| Envoyer un message            | Utilisateur     |                                      |
| Lire un message               | Utilisateur     |                                      |
| Gérer les utilisateurs        | Admin           | Peut inclure *Rechercher un utilisateur* |
| Rechercher un utilisateur     | Admin           | `<<include>>` dans *Gérer les utilisateurs* |
| Consulter les logs système    | Admin           | `<<extend>>` de *Gérer les utilisateurs* (optionnel) |


## Exemple concret : Application de reservation Kékés voyages : 
![diagramme-use-case-kékés-voyages](data/use-case-diagram-for-travel-agency.jpg)

