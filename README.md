# 🧹 **Nettoyage des marque-pages Firefox**  
*Personnalisation de la barre personnelle avec userChrome.css*

**Ce fichier CSS permet de :**
- Masquer le texte des dossiers
- Centrer les marque-pages
- Séparer visuellement dossiers (à gauche) et favoris (à droite)
  

![Prévisualisation](https://user-images.githubusercontent.com/83400726/233775520-7a18aefc-4d55-4834-adda-a2b84da42311.png)


##**Installation du style**

### 1. Accéder au dossier de profil
Menu Firefox (☰) > Aide > Plus d'informations de dépannage

**OU**  
Collez directement dans la barre d'adresse :  
```bash
about:support
```

- Sur la page *Informations de dépannage* :  
  **→ Cliquez sur *Ouvrir le dossier***  

⚠️ **Cas particulier** (Firefox Microsoft Store) :  
%LOCALAPPDATA%\Packages > Mozilla.Firefox... > Profiles


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



### 5. Télécharger userChrome.css
[![Télécharger le fichier](https://img.shields.io/badge/📥-Télécharger_userChrome.css-blue?style=for-the-badge)](https://github.com/Jrdmn/Firefox-Librewolf-userChrome.css/releases)

**Placez le fichier dans :**  
`[dossier profil]/chrome/userChrome.css`


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
