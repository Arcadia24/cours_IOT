# Coffre connecté
### Résumé du projet

Un mini-coffre sécurisé contrôlé par un ESP32, qui :

Détecte un code secret saisi via 3 boutons physiques
Déverrouille le coffre à l’aide d’un servomoteur si le code est correct
Utilise un capteur MPU6050 pour détecter les mouvements ou tentatives d’ouverture forcée
Allume une LED embarquée en cas de succès
(Extension facultative) Possède une interface web locale embarquée

### Liste des composants

| Composant                      | Référence / Détail                               |
| ------------------------------ | ------------------------------------------------ |
| **Microcontrôleur**            | XIAO ESP32-C6 ou Rasp pico                       |
| **Capteur de mouvement**       | MPU6050 (accéléromètre + gyroscope)              |
| **Servomoteur**                | Attention positional ou continuous               |
| **Boutons poussoirs** (x3)     | Pour former un code secret                       |
| **LED Néopixel**               | Pour savoir si le coffre est ouvert ou non       |
| **Breadboard**                 | Pour tester sans soudure                         |
| **Connexion WiFi**             | Réseau local pour extension web                  |

## 📚 Étapes du projet

### ✅ 1. Tests de chaque composant
- Test boutons
- Test LED Néopixel
- Test servo
- Test MPU6050

### ✅ 2. Lecture du code secret
- Saisie via les boutons (ex: A-B-C)
- Vérification du mot de passe

### ✅ 3. Déverrouillage du coffre
- Rotation servo si code bon
- LED allumée pour confirmation

### ✅ 4. Détection de mouvement
- Lecture du MPU6050
- Allumage LED si mouvement détecté

### ✅ 5. Conception du coffre
- Concevoir la base du coffre
- Attention à ce que toutes les pièces s'emboitent bien

### ✅ 6. Assemblage final
- Garder la breadboard pour que les plus gros composants soient réutilisés par la suite

---

## ✨ Extension facultative

> Interface Web embarquée (ESP32 héberge une page HTML)
- Saisie du code via navigateur
- Ouverture du coffre à distance
- Affichage de l’état
