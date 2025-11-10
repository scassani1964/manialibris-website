# ✅ CHECKLIST DE VÉRIFICATION
## Correction des Liens Amazon - 12 Fichiers HTML

---

## 📦 CONTENU ATTENDU DU DOSSIER

Votre dossier `1-Mise à jour Site manialibris` doit contenir :

```
📁 C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris\
   
   📄 FICHIERS HTML (12 total)
   ☐ tua-vontade.html
   ☐ ta-volonte.html
   ☐ o-lado-de-adao.html
   ☐ le-cote-d-adam.html
   ☐ aprendi-a-estar-contente.html
   ☐ jai-appris-a-etre-content.html
   ☐ index.html
   ☐ index-fr.html
   ☐ catalogo.html
   ☐ catalogue-fr.html
   ☐ recursos.html
   ☐ ressources.html
   
   📄 SCRIPT DE DÉPLOIEMENT
   ☐ DEPLOY_MANIALIBRIS.bat
   
   📄 GUIDES (4 total)
   ☐ GUIDE_INSTALLATION.md
   ☐ GUIDE_RAPIDE_CMD.md
   ☐ CHECKLIST_VERIFICATION.md (ce fichier)
   ☐ README_FICHIERS_HTML.md
```

**Total attendu : 17 fichiers**
- 12 fichiers HTML
- 1 script .bat
- 4 guides .md

---

## 🔍 COMMANDE DE VÉRIFICATION RAPIDE

Ouvrez CMD et exécutez :

```cmd
cd "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris"
dir
```

Vous devriez voir **exactement 17 fichiers** listés.

---

## 🎯 COMMANDE ULTIME DE VÉRIFICATION

Copiez-collez cette commande dans CMD pour tout vérifier en une seule fois :

```cmd
cd "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris" && echo. && echo ========== FICHIERS HTML (12 attendus) ========== && dir /b *.html && echo. && echo ========== NOMBRE DE FICHIERS HTML ========== && dir /b *.html | find /c /v "" && echo. && echo ========== SCRIPT BAT (1 attendu) ========== && dir /b *.bat && echo. && echo ========== GUIDES MD (4 attendus) ========== && dir /b *.md && echo. && echo ========== NOMBRE DE GUIDES MD ========== && dir /b *.md | find /c /v "" && echo. && echo ✅ Verifiez les totaux ci-dessus !
```

**Résultat attendu :**
```
========== FICHIERS HTML (12 attendus) ==========
aprendi-a-estar-contente.html
catalogo.html
catalogue-fr.html
index-fr.html
index.html
jai-appris-a-etre-content.html
le-cote-d-adam.html
o-lado-de-adao.html
recursos.html
ressources.html
ta-volonte.html
tua-vontade.html

========== NOMBRE DE FICHIERS HTML ==========
12

========== SCRIPT BAT (1 attendu) ==========
DEPLOY_MANIALIBRIS.bat

========== GUIDES MD (4 attendus) ==========
CHECKLIST_VERIFICATION.md
GUIDE_INSTALLATION.md
GUIDE_RAPIDE_CMD.md
README_FICHIERS_HTML.md

========== NOMBRE DE GUIDES MD ==========
4

✅ Verifiez les totaux ci-dessus !
```

---

## ✅ VÉRIFICATION DÉTAILLÉE PAR TYPE DE FICHIER

### 1. FICHIERS HTML DES LIVRES (6 fichiers)

**Portugais (Amazon BR) :**
- [ ] **tua-vontade.html** - Contient ASIN B0FY3TR5MD
- [ ] **o-lado-de-adao.html** - Contient ASIN B0G1HNZQKH
- [ ] **aprendi-a-estar-contente.html** - Contient ASIN B0G1L1VTW5

**Français (Amazon FR) :**
- [ ] **ta-volonte.html** - Contient ASIN B0FY3ZT7P5
- [ ] **le-cote-d-adam.html** - Contient ASIN B0G1HP942H
- [ ] **jai-appris-a-etre-content.html** - Contient ASIN B0G1L1VTW5

**Vérifier les ASIN dans les fichiers :**
```cmd
REM Vérifier les ASIN BR
type tua-vontade.html | findstr "B0FY3TR5MD"
type o-lado-de-adao.html | findstr "B0G1HNZQKH"
type aprendi-a-estar-contente.html | findstr "B0G1L1VTW5"

REM Vérifier les ASIN FR
type ta-volonte.html | findstr "B0FY3ZT7P5"
type le-cote-d-adam.html | findstr "B0G1HP942H"
type jai-appris-a-etre-content.html | findstr "B0G1L1VTW5"
```

Chaque commande doit afficher au moins une ligne contenant l'ASIN.

---

### 2. FICHIERS HTML PRINCIPAUX (6 fichiers)

- [ ] **index.html** - Page d'accueil portugais
- [ ] **index-fr.html** - Page d'accueil français
- [ ] **catalogo.html** - Catalogue portugais
- [ ] **catalogue-fr.html** - Catalogue français
- [ ] **recursos.html** - Ressources portugais
- [ ] **ressources.html** - Ressources français

**Vérifier la présence des fichiers :**
```cmd
dir index*.html
dir catalog*.html
dir recurs*.html
dir ressources.html
```

---

### 3. SCRIPT DE DÉPLOIEMENT

- [ ] **DEPLOY_MANIALIBRIS.bat** - Script automatique

**Vérifier le contenu du script :**
```cmd
type DEPLOY_MANIALIBRIS.bat | findstr "git"
```
**Résultat attendu :** Plusieurs lignes contenant "git"

**Vérifier qu'il copie les 12 fichiers :**
```cmd
type DEPLOY_MANIALIBRIS.bat | findstr "copy"
```
**Résultat attendu :** 12 lignes avec "copy"

---

### 4. GUIDES DE DOCUMENTATION

- [ ] **GUIDE_INSTALLATION.md** - Guide détaillé complet
- [ ] **GUIDE_RAPIDE_CMD.md** - Commandes CMD rapides
- [ ] **CHECKLIST_VERIFICATION.md** - Ce fichier
- [ ] **README_FICHIERS_HTML.md** - Liste des fichiers HTML

**Vérifier la présence :**
```cmd
dir *.md
```
**Résultat attendu :** 4 fichiers .md

---

## 📋 CHECKLIST PRÉ-DÉPLOIEMENT

Avant de lancer le script, vérifiez :

### Environnement Windows
- [ ] Windows 10 ou 11
- [ ] Droits d'administrateur (optionnel mais recommandé)
- [ ] Connexion Internet active

### Git Installé
- [ ] Git installé : `git --version` fonctionne
- [ ] Version 2.x.x ou supérieure

**Commande de vérification :**
```cmd
git --version
```
**Résultat attendu :** `git version 2.x.x`

### Configuration Git
- [ ] Nom configuré : `git config user.name`
- [ ] Email configuré : `git config user.email`

**Commandes de vérification :**
```cmd
git config user.name
git config user.email
```
**Résultats attendus :**
```
Stephane Cassani
info@manialibris.com
```

Si vide, configurez avec :
```cmd
git config --global user.name "Stephane Cassani"
git config --global user.email "info@manialibris.com"
```

### Dossier de Travail
- [ ] Tous les 17 fichiers présents
- [ ] Aucun fichier corrompu (taille > 0)
- [ ] Script .bat non modifié
- [ ] Fichiers HTML contiennent les bons ASIN

**Vérifier les tailles :**
```cmd
dir *.html
```
Aucun fichier ne doit avoir 0 octets.

---

## 🚀 SI TOUT EST OK

Si vous voyez bien **17 fichiers** dans votre dossier et que toutes les vérifications sont ✅, vous êtes prêt !

### Option 1 : Commande unique complète (RECOMMANDÉE)
```cmd
git config --global user.name "Stephane Cassani" && git config --global user.email "info@manialibris.com" && cd "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris" && DEPLOY_MANIALIBRIS.bat
```

### Option 2 : Lancer le script manuellement
```cmd
cd "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris"
DEPLOY_MANIALIBRIS.bat
```

---

## ❌ SI IL MANQUE DES FICHIERS

### Fichiers HTML manquants ?

Si vous n'avez pas les 12 fichiers HTML, vous devez :
1. Récupérer vos fichiers HTML corrigés avec les bons liens Amazon
2. Les placer dans le dossier de staging
3. Recommencer la vérification

**Liste exacte des fichiers HTML nécessaires :**
```
tua-vontade.html
ta-volonte.html
o-lado-de-adao.html
le-cote-d-adam.html
aprendi-a-estar-contente.html
jai-appris-a-etre-content.html
index.html
index-fr.html
catalogo.html
catalogue-fr.html
recursos.html
ressources.html
```

### Script .bat manquant ?

➡️ **Solution :**
1. Retournez dans Claude
2. Re-téléchargez le fichier DEPLOY_MANIALIBRIS.bat
3. Placez-le dans le dossier
4. Recommencez la vérification

---

## 📋 CHECKLIST PENDANT LE DÉPLOIEMENT

Pendant l'exécution du script, vérifiez :

### Étape 1 : Clonage/Mise à jour du repo
- [ ] Repository cloné ou mis à jour sans erreur
- [ ] Dossier `C:\Users\Stéphane CASSANI\Documents\manialibris-website` créé

### Étape 2 : Copie des fichiers
- [ ] 12 messages `[OK] fichier.html` affichés
- [ ] Aucun message `[SKIP] fichier.html non trouve`

Si des fichiers sont SKIP, arrêtez (Ctrl+C) et vérifiez qu'ils sont dans le dossier.

### Étape 3 : Backup
- [ ] Message `Backup cree : ...` affiché
- [ ] Dossier backup créé avec horodatage

### Étape 4 : Vérification Git
- [ ] `git status` affiche les 12 fichiers modifiés
- [ ] `git diff --stat` affiche les statistiques

### Étape 5 : Confirmation
- [ ] Résumé des modifications affiché
- [ ] Question "Voulez-vous continuer ? (O/N)" apparaît

**À CE MOMENT :**
- Tapez **O** pour déployer
- Tapez **N** pour annuler

### Étape 6 : Déploiement
- [ ] `git add .` exécuté
- [ ] `git commit` créé avec message
- [ ] `git push` réussi vers GitHub
- [ ] Message "DEPLOIEMENT REUSSI !" affiché

---

## 📋 CHECKLIST POST-DÉPLOIEMENT

Après exécution du script :

### Vérifications Immédiates (0 minute)
- [ ] Script terminé sans erreur
- [ ] Message "DEPLOIEMENT REUSSI !" affiché
- [ ] Liste des liens Amazon affichée
- [ ] Backup créé (dossier backup_YYYYMMDD_HHMMSS)

### Vérifications GitHub (1 minute)
- [ ] Commit visible : https://github.com/scassani1964/manialibris-website/commits/main
- [ ] Message de commit : "Correction des liens Amazon - Tous les ASIN corriges pour BR et FR"
- [ ] 12 fichiers modifiés visibles

**Commande pour vérifier localement :**
```cmd
cd C:\Users\Stéphane CASSANI\Documents\manialibris-website
git log --oneline -1
```

### Vérifications Netlify (2 minutes)
- [ ] Build lancé sur https://app.netlify.com
- [ ] Build en cours (orange) puis réussi (vert)
- [ ] Status "Published"
- [ ] Aucune erreur de build

### Vérifications Site Live (3 minutes)

**Pages des livres portugais (Amazon BR) :**
- [ ] https://manialibris.com/tua-vontade.html
  - Bouton Amazon mène vers B0FY3TR5MD
- [ ] https://manialibris.com/o-lado-de-adao.html
  - Bouton Amazon mène vers B0G1HNZQKH
- [ ] https://manialibris.com/aprendi-a-estar-contente.html
  - Bouton Amazon mène vers B0G1L1VTW5

**Pages des livres français (Amazon FR) :**
- [ ] https://manialibris.com/ta-volonte.html
  - Bouton Amazon mène vers B0FY3ZT7P5
- [ ] https://manialibris.com/le-cote-d-adam.html
  - Bouton Amazon mène vers B0G1HP942H
- [ ] https://manialibris.com/jai-appris-a-etre-content.html
  - Bouton Amazon mène vers B0G1L1VTW5

**Pages principales :**
- [ ] https://manialibris.com/ (index portugais)
- [ ] https://manialibris.com/index-fr.html (index français)
- [ ] https://manialibris.com/catalogo.html (catalogue portugais)
- [ ] https://manialibris.com/catalogue-fr.html (catalogue français)
- [ ] https://manialibris.com/recursos.html (ressources portugais)
- [ ] https://manialibris.com/ressources.html (ressources français)

### Tests Fonctionnels
- [ ] Navigation fonctionne (menu, liens)
- [ ] Design or/noir préservé (#DAA520 / #000000)
- [ ] Responsive design fonctionne (mobile/tablet/desktop)
- [ ] Tous les boutons Amazon ouvrent dans un nouvel onglet
- [ ] URLs Amazon correctes (BR vs FR)

---

## 🎯 VALIDATION DES LIENS AMAZON

**CRITIQUE :** Testez CHAQUE bouton Amazon manuellement !

### Amazon BR (Portugais)
```
✅ Tua Vontade
   Cliquer sur le bouton → Doit ouvrir :
   https://www.amazon.com.br/dp/B0FY3TR5MD
   
✅ O Lado de Adão
   Cliquer sur le bouton → Doit ouvrir :
   https://www.amazon.com.br/dp/B0G1HNZQKH
   
✅ Aprendi a Estar Contente
   Cliquer sur le bouton → Doit ouvrir :
   https://www.amazon.com.br/dp/B0G1L1VTW5
```

### Amazon FR (Français)
```
✅ Ta Volonté
   Cliquer sur le bouton → Doit ouvrir :
   https://www.amazon.fr/dp/B0FY3ZT7P5
   
✅ Le Côté d'Adam
   Cliquer sur le bouton → Doit ouvrir :
   https://www.amazon.fr/dp/B0G1HP942H
   
✅ J'ai Appris à Être Content
   Cliquer sur le bouton → Doit ouvrir :
   https://www.amazon.fr/dp/B0G1L1VTW5
```

---

## ✨ TEMPS ESTIMÉ

- **Préparation des fichiers :** 5 minutes
- **Vérification (cette checklist) :** 3 minutes
- **Exécution du script :** 2 minutes
- **Déploiement GitHub + Netlify :** 2 minutes
- **Tests finaux :** 5 minutes

**Total : ~17 minutes du début à la fin !**

---

## 🎉 VALIDATION FINALE

Une fois toutes les cases cochées ✅, votre mise à jour est complète !

**Résultat attendu :**
```
✅ 12 fichiers HTML déployés
✅ Tous les liens Amazon corrects
✅ Amazon BR pointe vers amazon.com.br avec bons ASIN
✅ Amazon FR pointe vers amazon.fr avec bons ASIN
✅ Site live et fonctionnel
✅ Navigation cohérente
✅ Design préservé
✅ Backup créé (possibilité de rollback)
```

**Bravo !** 🎊

Vos visiteurs peuvent maintenant acheter vos livres avec les bons liens Amazon !

---

## 🆘 EN CAS DE PROBLÈME

Si une case reste ❌ :

1. **Notez quelle étape a échoué**
2. **Copiez le message d'erreur**
3. **Consultez le GUIDE_INSTALLATION.md section Dépannage**
4. **Ou revenez dans Claude avec les détails**

---

## 💾 SAUVEGARDE CETTE CHECKLIST

**Gardez cette checklist pour les prochaines mises à jour !**

Chaque déploiement futur pourra utiliser ce même processus de vérification.

---

**Version :** 2.0 - Correction Liens Amazon  
**Date :** Novembre 2025  
**Auteur :** Claude pour Mania Libris
