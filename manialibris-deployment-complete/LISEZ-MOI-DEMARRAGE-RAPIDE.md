# 🎉 PACKAGE DE DÉPLOIEMENT MANIA LIBRIS
## Correction des Liens Amazon - Version 2.0

---

## 📦 CONTENU DU PACKAGE

Ce package contient **5 fichiers essentiels** pour déployer vos corrections sur le site Mania Libris :

1. ✅ **DEPLOY_MANIALIBRIS.bat** (8.1 KB)
   - Script automatique de déploiement Windows
   - Clone/met à jour le repository GitHub
   - Copie les 12 fichiers HTML
   - Crée un backup automatique
   - Déploie sur GitHub en quelques clics

2. ✅ **GUIDE_INSTALLATION.md** (10 KB)
   - Guide complet étape par étape
   - Méthode automatique (recommandée)
   - Méthode manuelle (fallback)
   - Section dépannage complète
   - Instructions détaillées pour chaque étape

3. ✅ **GUIDE_RAPIDE_CMD.md** (9.1 KB)
   - Commande unique pour tout déployer
   - Raccourcis CMD essentiels
   - Vérifications rapides
   - Astuces Windows

4. ✅ **CHECKLIST_VERIFICATION.md** (13 KB)
   - Checklist pré-déploiement
   - Vérification des 12 fichiers HTML
   - Validation des ASIN Amazon
   - Checklist post-déploiement

5. ✅ **README_FICHIERS_HTML.md** (7.9 KB)
   - Liste détaillée des 12 fichiers HTML requis
   - ASIN Amazon pour chaque livre
   - Spécifications techniques
   - Erreurs courantes à éviter

---

## 🚀 DÉMARRAGE RAPIDE (3 ÉTAPES)

### ⚠️ IMPORTANT : Vous devez d'abord avoir vos 12 fichiers HTML !

Ce package contient les **outils de déploiement**, mais PAS les fichiers HTML.

**Les 12 fichiers HTML nécessaires :**
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

Consultez **README_FICHIERS_HTML.md** pour plus de détails sur ces fichiers.

---

### Étape 1 : Préparer le Dossier

1. Créez ou videz ce dossier :
   ```
   C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris\
   ```

2. Placez-y **TOUS** les fichiers :
   - Les **12 fichiers HTML** avec liens Amazon corrigés
   - Les **5 fichiers** de ce package (.bat et .md)

3. Vous devriez avoir **17 fichiers au total** dans le dossier

---

### Étape 2 : Vérifier le Contenu

Ouvrez CMD (Windows + R → `cmd`) et vérifiez :

```cmd
cd "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris"
dir
```

**Résultat attendu :**
- 12 fichiers .html
- 1 fichier .bat
- 4 fichiers .md

**Total : 17 fichiers**

---

### Étape 3 : Déployer en 1 Commande

Dans la même fenêtre CMD, copiez-collez cette commande :

```cmd
git config --global user.name "Stephane Cassani" && git config --global user.email "info@manialibris.com" && cd "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris" && DEPLOY_MANIALIBRIS.bat
```

**Cette commande unique fait tout :**
1. ✅ Configure Git
2. ✅ Va dans le bon dossier
3. ✅ Lance le script de déploiement automatique

**Durée totale : 2-3 minutes**

---

## 🎯 CE QUI SERA DÉPLOYÉ

### Livres Portugais (Amazon BR)
- **Tua Vontade** → https://www.amazon.com.br/dp/B0FY3TR5MD
- **O Lado de Adão** → https://www.amazon.com.br/dp/B0G1HNZQKH
- **Aprendi a Estar Contente** → https://www.amazon.com.br/dp/B0G1L1VTW5

### Livres Français (Amazon FR)
- **Ta Volonté** → https://www.amazon.fr/dp/B0FY3ZT7P5
- **Le Côté d'Adam** → https://www.amazon.fr/dp/B0G1HP942H
- **J'ai Appris à Être Content** → https://www.amazon.fr/dp/B0G1L1VTW5

### Pages Principales
- index.html / index-fr.html
- catalogo.html / catalogue-fr.html
- recursos.html / ressources.html

---

## 📚 GUIDES DÉTAILLÉS

### 🆕 Première fois que vous déployez ?
➡️ Lisez **GUIDE_INSTALLATION.md** - Instructions complètes avec captures

### ⚡ Vous connaissez déjà Git ?
➡️ Lisez **GUIDE_RAPIDE_CMD.md** - Commandes essentielles

### ✅ Vous voulez tout vérifier ?
➡️ Suivez **CHECKLIST_VERIFICATION.md** - Validation étape par étape

### 📋 Vous devez créer/corriger des fichiers HTML ?
➡️ Consultez **README_FICHIERS_HTML.md** - Spécifications complètes

---

## ⚡ COMMANDE MAGIQUE (À RETENIR)

```cmd
git config --global user.name "Stephane Cassani" && git config --global user.email "info@manialibris.com" && cd "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris" && DEPLOY_MANIALIBRIS.bat
```

**💾 Copiez cette commande dans un fichier texte pour les prochaines fois !**

---

## 🔧 PRÉREQUIS

Avant de commencer, assurez-vous d'avoir :

### Logiciels
- [ ] **Windows 10 ou 11**
- [ ] **Git installé** : https://git-scm.com/download/win
- [ ] **Connexion Internet** active

### Fichiers
- [ ] **Les 12 fichiers HTML** avec liens Amazon corrigés
- [ ] **Ce package de déploiement** (5 fichiers)

### Configuration
- [ ] **Git configuré** (le script le fait automatiquement)
- [ ] **Compte GitHub** accessible (pour authentification)

---

## 🌐 VÉRIFICATION POST-DÉPLOIEMENT

Après le déploiement, attendez **2-3 minutes** puis testez :

### GitHub (immédiat)
```
https://github.com/scassani1964/manialibris-website/commits/main
```
Cherchez : "Correction des liens Amazon - Tous les ASIN corriges pour BR et FR"

### Netlify (1-2 minutes)
```
https://app.netlify.com
```
Attendez le status "Published" (vert)

### Site Live (2-3 minutes)
```
https://manialibris.com/
```
Testez TOUS les boutons Amazon sur chaque page !

---

## 🆘 EN CAS DE PROBLÈME

### "Git n'est pas reconnu"
➡️ Git pas installé : https://git-scm.com/download/win

### "Author identity unknown"
➡️ La commande magique ci-dessus configure automatiquement Git

### "Permission denied"
➡️ Authentification GitHub nécessaire (navigateur s'ouvrira)

### "LF will be replaced by CRLF"
➡️ WARNING normal sur Windows, ignorez

### Autres erreurs
➡️ Consultez la section Dépannage dans **GUIDE_INSTALLATION.md**

---

## ✨ WORKFLOW COMPLET

```
1. Préparer les 12 fichiers HTML
   ↓
2. Placer tous les fichiers dans le dossier de staging
   ↓
3. Vérifier avec CHECKLIST_VERIFICATION.md
   ↓
4. Exécuter la commande magique
   ↓
5. Confirmer le déploiement (taper O)
   ↓
6. Attendre 2-3 minutes
   ↓
7. Tester tous les liens Amazon
   ↓
8. ✅ TERMINÉ !
```

---

## 📊 TEMPS ESTIMÉ TOTAL

- **Préparation** : 5 minutes
- **Vérification** : 3 minutes
- **Déploiement** : 2 minutes
- **Attente Netlify** : 2 minutes
- **Tests** : 5 minutes

**Total : ~17 minutes** ⏱️

---

## 🎉 RÉSULTAT FINAL

Une fois terminé, vous aurez :

✅ **12 fichiers HTML déployés** sur votre site
✅ **Tous les liens Amazon corrects** (BR et FR)
✅ **Site live** sur https://manialibris.com/
✅ **Navigation cohérente** sur toutes les pages
✅ **Design or/noir** préservé
✅ **Backup automatique** créé (possibilité de rollback)

**Vos visiteurs pourront acheter vos livres avec les bons liens !** 📚

---

## 💡 CONSEIL POUR LE FUTUR

**Gardez ce package et la commande magique !**

Pour les prochaines mises à jour du site, vous pourrez :
1. Mettre vos nouveaux fichiers HTML dans le dossier
2. Relancer la même commande
3. C'est tout ! 🚀

---

## 📞 BESOIN D'AIDE ?

Si vous rencontrez un problème :

1. **Consultez d'abord** les guides (GUIDE_INSTALLATION.md ou GUIDE_RAPIDE_CMD.md)
2. **Vérifiez** la CHECKLIST_VERIFICATION.md
3. **Copiez** le message d'erreur exact
4. **Revenez dans Claude** avec ces informations

---

## 🔗 LIENS UTILES

- **Repository GitHub :** https://github.com/scassani1964/manialibris-website
- **Dashboard Netlify :** https://app.netlify.com
- **Site Live :** https://manialibris.com/
- **Télécharger Git :** https://git-scm.com/download/win

---

## 🌟 CARACTÉRISTIQUES

✨ **Déploiement automatique** en 1 commande
✨ **Backup intégré** avant chaque modification
✨ **Vérification Git** avant push
✨ **Gestion d'erreurs** complète
✨ **Documentation détaillée** (4 guides)
✨ **Workflow optimisé** pour Windows

---

**Version :** 2.0 - Correction Liens Amazon  
**Date :** Novembre 2025  
**Créé par :** Claude pour Mania Libris  
**Stack :** Git + GitHub + Netlify  
**Compatible :** Windows 10/11

---

# 🚀 BONNE CHANCE AVEC VOTRE DÉPLOIEMENT !

**N'oubliez pas de tester tous les boutons Amazon après le déploiement !**

---

*Pour plus de détails, consultez les guides individuels inclus dans ce package.*
