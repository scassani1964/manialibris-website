# 🚀 GUIDE RAPIDE - COMMANDES CMD POUR MANIA LIBRIS
## Correction des Liens Amazon - Version 2.0

---

## 📋 VÉRIFICATION RAPIDE DU CONTENU

### Voir les fichiers dans le dossier
```cmd
cd "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris"
dir
```

### Compter les fichiers HTML
```cmd
dir *.html | find /c ".html"
```
**Résultat attendu :** 12 fichiers HTML

### Vérifier le script bat
```cmd
dir *.bat
```
**Résultat attendu :** DEPLOY_MANIALIBRIS.bat

---

## 🚀 DÉPLOIEMENT EN UNE COMMANDE

### Commande Complète (Copier-Coller)

```cmd
git config --global user.name "Stephane Cassani" && git config --global user.email "info@manialibris.com" && cd "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris" && DEPLOY_MANIALIBRIS.bat
```

**Cette commande unique fait tout :**
1. ✅ Configure Git (nom + email)
2. ✅ Va dans le bon dossier
3. ✅ Lance le script de déploiement
4. ✅ Clone le repo si nécessaire
5. ✅ Copie les 12 fichiers HTML
6. ✅ Crée un backup automatique
7. ✅ Affiche les modifications
8. ✅ Demande confirmation
9. ✅ Déploie sur GitHub

**Durée totale :** 2-3 minutes

---

## ⚡ COMMANDES INDIVIDUELLES (Si besoin)

### 1. Configurer Git (une seule fois)
```cmd
git config --global user.name "Stephane Cassani"
git config --global user.email "info@manialibris.com"
```

### 2. Naviguer vers le dossier
```cmd
cd "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris"
```

### 3. Lancer le script
```cmd
DEPLOY_MANIALIBRIS.bat
```

---

## 🔍 COMMANDES DE VÉRIFICATION

### Vérifier que Git est installé
```cmd
git --version
```
**Résultat attendu :** `git version 2.x.x`

### Vérifier l'identité Git configurée
```cmd
git config user.name
git config user.email
```
**Résultat attendu :** 
```
Stephane Cassani
info@manialibris.com
```

### Vérifier le repository local
```cmd
cd C:\Users\Stéphane CASSANI\Documents\manialibris-website
git status
```

### Voir les derniers commits
```cmd
cd C:\Users\Stéphane CASSANI\Documents\manialibris-website
git log --oneline -5
```

### Vérifier quels fichiers ont été modifiés
```cmd
cd C:\Users\Stéphane CASSANI\Documents\manialibris-website
git diff --name-only
```

---

## 🔧 COMMANDES DE DÉPANNAGE

### Réinitialiser la config Git
```cmd
git config --global --unset user.name
git config --global --unset user.email
git config --global user.name "Stephane Cassani"
git config --global user.email "info@manialibris.com"
```

### Forcer la mise à jour du repo local
```cmd
cd C:\Users\Stéphane CASSANI\Documents\manialibris-website
git fetch origin
git reset --hard origin/main
```

### Annuler les modifications locales non commitées
```cmd
cd C:\Users\Stéphane CASSANI\Documents\manialibris-website
git restore .
```

### Voir les différences détaillées avant de committer
```cmd
cd C:\Users\Stéphane CASSANI\Documents\manialibris-website
git diff
```

---

## 📊 WORKFLOW MANUEL COMPLET (Alternative au script)

Si le script .bat ne fonctionne pas, voici les commandes manuelles :

```cmd
REM 1. Naviguer vers le repository
cd C:\Users\Stéphane CASSANI\Documents\manialibris-website

REM 2. Mettre à jour
git pull origin main

REM 3. Créer backup
mkdir backup_%date:~-4,4%%date:~-7,2%%date:~-10,2%
copy *.html backup_%date:~-4,4%%date:~-7,2%%date:~-10,2%\

REM 4. Copier les 12 fichiers HTML
copy "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris\tua-vontade.html" .
copy "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris\ta-volonte.html" .
copy "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris\o-lado-de-adao.html" .
copy "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris\le-cote-d-adam.html" .
copy "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris\aprendi-a-estar-contente.html" .
copy "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris\jai-appris-a-etre-content.html" .
copy "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris\index.html" .
copy "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris\index-fr.html" .
copy "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris\catalogo.html" .
copy "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris\catalogue-fr.html" .
copy "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris\recursos.html" .
copy "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris\ressources.html" .

REM 5. Vérifier
git status
git diff --stat

REM 6. Committer
git add .
git commit -m "Correction des liens Amazon - Tous les ASIN corriges pour BR et FR"

REM 7. Pusher
git push origin main
```

---

## 🌐 VÉRIFICATION POST-DÉPLOIEMENT

### 1. Vérifier GitHub (immédiat)
```
https://github.com/scassani1964/manialibris-website/commits/main
```
Cherchez : "Correction des liens Amazon - Tous les ASIN corriges pour BR et FR"

### 2. Vérifier Netlify (1-2 minutes)
```
https://app.netlify.com
```
Attendez que le status soit : **Published** (vert)

### 3. Tester les pages live (2-3 minutes)

**Pages des Livres Portugais :**
```
https://manialibris.com/tua-vontade.html
https://manialibris.com/o-lado-de-adao.html
https://manialibris.com/aprendi-a-estar-contente.html
```

**Pages des Livres Français :**
```
https://manialibris.com/ta-volonte.html
https://manialibris.com/le-cote-d-adam.html
https://manialibris.com/jai-appris-a-etre-content.html
```

**Pages Principales :**
```
https://manialibris.com/
https://manialibris.com/index-fr.html
https://manialibris.com/catalogo.html
https://manialibris.com/catalogue-fr.html
https://manialibris.com/recursos.html
https://manialibris.com/ressources.html
```

### 4. Tester TOUS les boutons Amazon

**Sur chaque page, cliquez sur le bouton "Acheter sur Amazon" et vérifiez :**
- ✅ Le lien s'ouvre dans un nouvel onglet
- ✅ Vous arrivez sur la bonne page produit Amazon
- ✅ Le bon livre est affiché
- ✅ Le bon pays Amazon (BR ou FR)

**ASIN à vérifier dans l'URL :**

Amazon BR (Portugais) :
- Tua Vontade → B0FY3TR5MD
- O Lado de Adão → B0G1HNZQKH
- Aprendi a Estar Contente → B0G1L1VTW5

Amazon FR (Français) :
- Ta Volonté → B0FY3ZT7P5
- Le Côté d'Adam → B0G1HP942H
- J'ai Appris à Être Content → B0G1L1VTW5

---

## 💡 ASTUCES

### Ouvrir CMD rapidement
1. Appuyez sur `Windows + R`
2. Tapez `cmd`
3. Appuyez sur `Entrée`

### Coller dans CMD
- `Ctrl + V` ne fonctionne pas dans CMD classique
- **Clic droit** dans CMD pour coller
- Ou utilisez `Shift + Insert`

### Nettoyer l'écran CMD
```cmd
cls
```

### Quitter le script en cours
```
Ctrl + C
```

### Copier du texte depuis CMD
1. Cliquez dans CMD
2. Sélectionnez le texte avec la souris
3. Appuyez sur `Entrée` (le texte est copié)

### Historique des commandes
- Flèche **↑** = commande précédente
- Flèche **↓** = commande suivante

---

## 🆘 MESSAGES D'ERREUR COURANTS

### "git n'est pas reconnu"
➡️ **Solution :** Git pas installé
```
https://git-scm.com/download/win
```
Installez Git puis relancez CMD

### "Author identity unknown"
➡️ **Solution :** Configurez Git
```cmd
git config --global user.name "Stephane Cassani"
git config --global user.email "info@manialibris.com"
```

### "Permission denied" ou "Authentication failed"
➡️ **Solution :** Authentification GitHub nécessaire
Une fenêtre de navigateur s'ouvrira automatiquement.
Connectez-vous à GitHub et autorisez l'accès.

### "LF will be replaced by CRLF"
➡️ **Info :** WARNING normal sur Windows
Git convertit automatiquement les fins de ligne.
Ce n'est **pas une erreur**, ignorez ce message.

### "fatal: not a git repository"
➡️ **Solution :** Vous n'êtes pas dans le bon dossier
```cmd
cd C:\Users\Stéphane CASSANI\Documents\manialibris-website
```

### "Nothing to commit, working tree clean"
➡️ **Info :** Aucune modification détectée
Vérifiez que vous avez bien copié les nouveaux fichiers.

### "Your branch is behind 'origin/main'"
➡️ **Solution :** Mettez à jour votre repo local
```cmd
git pull origin main
```

---

## 📞 BESOIN D'AIDE ?

Si un message d'erreur apparaît :
1. **Copiez** le message complet (clic droit > Marquer > Sélectionner > Entrée)
2. **Notez** la commande qui a causé l'erreur
3. **Vérifiez** la section Dépannage ci-dessus
4. **Revenez dans Claude** avec ces informations

---

## ✨ COMMANDE FAVORITE À RETENIR

```cmd
git config --global user.name "Stephane Cassani" && git config --global user.email "info@manialibris.com" && cd "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris" && DEPLOY_MANIALIBRIS.bat
```

**💾 Copiez cette commande et gardez-la pour les prochaines mises à jour !**

**Enregistrez-la dans un fichier texte :** `commande_deploy_manialibris.txt`

---

## 🎯 RÉCAPITULATIF EXPRESS

**Pour déployer en 30 secondes :**

1. Ouvrez CMD (`Windows + R` → `cmd`)
2. Collez la commande unique (clic droit)
3. Appuyez sur `Entrée`
4. Tapez `O` quand demandé
5. Attendez 2-3 minutes
6. Testez votre site !

**C'est tout !** 🚀

---

**Version du Guide :** 2.0 - Correction Liens Amazon  
**Date :** Novembre 2025  
**Auteur :** Claude pour Mania Libris
