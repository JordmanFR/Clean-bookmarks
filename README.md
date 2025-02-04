# 🧹 **Nettoyage des marque-pages Firefox**  
*Personnalisation de la barre personnelle avec userChrome.css*

🔖 **Ce fichier CSS permet de :**
- Masquer le texte des dossiers
- Centrer les marque-pages
- Séparer visuellement dossiers (à gauche) et favoris (à droite)
  

![Prévisualisation](https://user-images.githubusercontent.com/83400726/233775520-7a18aefc-4d55-4834-adda-a2b84da42311.png)

---

## 🔧 **Configuration requise**

### 1. Accéder au dossier de profil
```bash
Menu Firefox (☰) > Aide > Plus d'informations de dépannage
```
**OU**  
Collez directement dans la barre d'adresse :  
`about:support`

### 2. Ouvrir le dossier utilisateur
- Sur la page *Informations de dépannage* :  
  **→ Cliquez sur *Ouvrir le dossier***  

⚠️ **Cas particulier** (Firefox Microsoft Store) :  
```bash
%LOCALAPPDATA%\Packages > Mozilla.Firefox... > Profiles
```

---

## 🛠️ **Mise en place**

### 3. Créer le dossier `chrome`
| Système | Méthode |
|---------|---------|
| **Windows** | `Clic droit > Nouveau > Dossier` → Nommez-le `chrome` |
| **Mac** | `Ctrl + clic > Nouveau dossier` → Nommez-le `chrome` |

### 4. Afficher les extensions de fichiers
| Système | Instructions |
|---------|--------------|
| **Windows** | `Onglet Affichage` → ✅ `Extensions de noms de fichiers` |
| **Mac** | `Finder > Préférences > Avancé` → ✅ `Afficher toutes les extensions` |

---

## ⚡ **Installation du style**

### 5. Télécharger userChrome.css
[![Télécharger le fichier](https://img.shields.io/badge/📥-Télécharger_userChrome.css-blue?style=for-the-badge)](https://github.com/Jrdmn/Firefox-Librewolf-userChrome.css/releases)

👉 **Placez le fichier dans :**  
`[dossier profil]/chrome/userChrome.css`

---

## ⚙️ **Activation (Firefox 69+)**
1. Collez dans la barre d'adresse :  
   `about:config` → Confirmez les risques
2. Recherchez :  
   ```css
   toolkit.legacyUserProfileCustomizations.stylesheets
   ```
3. **Double-cliquez** pour passer la valeur à :  
   ✅ **`true`**

🔁 **Redémarrez Firefox pour appliquer les changements**

---

💡 **Astuce** : Créez un raccourci bureau vers le dossier `chrome` pour modifier facilement le CSS plus tard !

```diff
+ Modification visuelle réussie lorsque :
- Les textes des dossiers disparaissent
- Les icônes sont centrées
- Séparation gauche/droite visible
```
