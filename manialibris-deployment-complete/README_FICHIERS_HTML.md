# 📋 LISTE DES FICHIERS HTML REQUIS
## Pour le Déploiement Mania Libris - Correction Liens Amazon

---

## 🎯 OBJECTIF

Ce document liste les **12 fichiers HTML** que vous devez avoir dans le dossier de staging avant de lancer le déploiement.

**Dossier cible :**
```
C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris\
```

---

## 📚 FICHIERS HTML DES LIVRES (6 fichiers)

### 🇧🇷 Livres en Portugais (Amazon BR)

#### 1. **tua-vontade.html**
- **Titre :** Tua Vontade
- **Amazon :** amazon.com.br
- **ASIN :** B0FY3TR5MD
- **URL Amazon :** https://www.amazon.com.br/dp/B0FY3TR5MD
- **Langue :** Portugais

#### 2. **o-lado-de-adao.html**
- **Titre :** O Lado de Adão
- **Amazon :** amazon.com.br
- **ASIN :** B0G1HNZQKH
- **URL Amazon :** https://www.amazon.com.br/dp/B0G1HNZQKH
- **Langue :** Portugais

#### 3. **aprendi-a-estar-contente.html**
- **Titre :** Aprendi a Estar Contente
- **Amazon :** amazon.com.br
- **ASIN :** B0G1L1VTW5
- **URL Amazon :** https://www.amazon.com.br/dp/B0G1L1VTW5
- **Langue :** Portugais

---

### 🇫🇷 Livres en Français (Amazon FR)

#### 4. **ta-volonte.html**
- **Titre :** Ta Volonté
- **Amazon :** amazon.fr
- **ASIN :** B0FY3ZT7P5
- **URL Amazon :** https://www.amazon.fr/dp/B0FY3ZT7P5
- **Langue :** Français

#### 5. **le-cote-d-adam.html**
- **Titre :** Le Côté d'Adam
- **Amazon :** amazon.fr
- **ASIN :** B0G1HP942H
- **URL Amazon :** https://www.amazon.fr/dp/B0G1HP942H
- **Langue :** Français

#### 6. **jai-appris-a-etre-content.html**
- **Titre :** J'ai Appris à Être Content
- **Amazon :** amazon.fr
- **ASIN :** B0G1L1VTW5
- **URL Amazon :** https://www.amazon.fr/dp/B0G1L1VTW5
- **Langue :** Français

---

## 🏠 FICHIERS HTML PRINCIPAUX (6 fichiers)

### Pages d'Accueil

#### 7. **index.html**
- **Description :** Page d'accueil principale (Portugais)
- **Contenu :** Présentation de Mania Libris
- **Navigation :** Vers catalogo.html, recursos.html
- **Langue :** Portugais

#### 8. **index-fr.html**
- **Description :** Page d'accueil française
- **Contenu :** Présentation de Mania Libris
- **Navigation :** Vers catalogue-fr.html, ressources.html
- **Langue :** Français

---

### Pages de Catalogue

#### 9. **catalogo.html**
- **Description :** Catalogue des livres (Portugais)
- **Contenu :** Liste de tous les livres avec miniatures
- **Liens vers :** tua-vontade.html, o-lado-de-adao.html, aprendi-a-estar-contente.html
- **Langue :** Portugais

#### 10. **catalogue-fr.html**
- **Description :** Catalogue des livres (Français)
- **Contenu :** Liste de tous les livres avec miniatures
- **Liens vers :** ta-volonte.html, le-cote-d-adam.html, jai-appris-a-etre-content.html
- **Langue :** Français

---

### Pages de Ressources

#### 11. **recursos.html**
- **Description :** Page des ressources théologiques (Portugais)
- **Contenu :** Articles, études, liens utiles
- **Navigation :** Intégrée au menu principal
- **Langue :** Portugais

#### 12. **ressources.html**
- **Description :** Page des ressources théologiques (Français)
- **Contenu :** Articles, études, liens utiles
- **Navigation :** Intégrée au menu principal
- **Langue :** Français

---

## ✅ CHECKLIST DE PRÉPARATION

Avant de lancer le script de déploiement, vérifiez que vous avez :

### Fichiers des Livres Portugais
- [ ] tua-vontade.html (avec ASIN B0FY3TR5MD)
- [ ] o-lado-de-adao.html (avec ASIN B0G1HNZQKH)
- [ ] aprendi-a-estar-contente.html (avec ASIN B0G1L1VTW5)

### Fichiers des Livres Français
- [ ] ta-volonte.html (avec ASIN B0FY3ZT7P5)
- [ ] le-cote-d-adam.html (avec ASIN B0G1HP942H)
- [ ] jai-appris-a-etre-content.html (avec ASIN B0G1L1VTW5)

### Fichiers Principaux
- [ ] index.html
- [ ] index-fr.html
- [ ] catalogo.html
- [ ] catalogue-fr.html
- [ ] recursos.html
- [ ] ressources.html

**Total : 12 fichiers** ✅

---

## 🔍 COMMENT VÉRIFIER LES ASIN

Pour vous assurer que vos fichiers HTML contiennent les bons ASIN, ouvrez CMD et exécutez :

### Vérifier les fichiers portugais (Amazon BR)
```cmd
cd "C:\Users\Stéphane CASSANI\Downloads\1-Mise à jour Site manialibris"

type tua-vontade.html | findstr "B0FY3TR5MD"
type o-lado-de-adao.html | findstr "B0G1HNZQKH"
type aprendi-a-estar-contente.html | findstr "B0G1L1VTW5"
```

### Vérifier les fichiers français (Amazon FR)
```cmd
type ta-volonte.html | findstr "B0FY3ZT7P5"
type le-cote-d-adam.html | findstr "B0G1HP942H"
type jai-appris-a-etre-content.html | findstr "B0G1L1VTW5"
```

**Si une commande n'affiche rien :** Le fichier ne contient pas le bon ASIN ! Corrigez-le avant de déployer.

---

## 📊 RÉCAPITULATIF DES ASIN

### Amazon BR (Brésil) - amazon.com.br
```
B0FY3TR5MD  →  Tua Vontade
B0G1HNZQKH  →  O Lado de Adão
B0G1L1VTW5  →  Aprendi a Estar Contente
```

### Amazon FR (France) - amazon.fr
```
B0FY3ZT7P5  →  Ta Volonté
B0G1HP942H  →  Le Côté d'Adam
B0G1L1VTW5  →  J'ai Appris à Être Content
```

---

## 🎨 CARACTÉRISTIQUES COMMUNES DES FICHIERS HTML

Tous vos fichiers HTML doivent avoir :

### Design
- Palette de couleurs : **Or (#DAA520)** sur **Noir (#000000)**
- Police : **Georgia** (serif)
- Responsive design (mobile/tablet/desktop)

### Navigation
- Menu cohérent sur toutes les pages
- Liens vers catalogue (PT ou FR selon langue)
- Liens vers ressources (PT ou FR selon langue)
- Sélecteur de langue (PT ↔ FR)

### Structure HTML
- Encodage : **UTF-8**
- DOCTYPE HTML5
- Meta tags (description, keywords, author)
- Titre de page approprié

### Boutons Amazon
- Ouvrent dans un **nouvel onglet** (target="_blank")
- Style cohérent (bouton or sur fond noir)
- Texte en langue appropriée :
  - PT: "Comprar na Amazon"
  - FR: "Acheter sur Amazon"

---

## 🚨 ERREURS COURANTES À ÉVITER

### ❌ Mauvais noms de fichiers
```
✖ Tua_Vontade.html         → Majuscules et underscore
✖ tua vontade.html          → Espaces
✖ tuavontade.html           → Pas de tirets
✔ tua-vontade.html          → CORRECT
```

### ❌ Mauvaises extensions
```
✖ tua-vontade.htm
✖ tua-vontade.HTML
✔ tua-vontade.html          → CORRECT (minuscules)
```

### ❌ ASIN incorrects
```
✖ amazon.com.br/dp/B0FY3ZT7P5    → ASIN FR sur site BR
✖ amazon.fr/dp/B0FY3TR5MD        → ASIN BR sur site FR
✔ amazon.com.br/dp/B0FY3TR5MD    → CORRECT
```

### ❌ Liens cassés dans le catalogue
```
✖ <a href="TuaVontade.html">      → Majuscules
✖ <a href="tua_vontade.html">     → Underscore
✔ <a href="tua-vontade.html">     → CORRECT
```

---

## 🛠️ SI VOUS DEVEZ CRÉER/MODIFIER UN FICHIER

Si un fichier est manquant ou incorrect, vous pouvez :

1. **Demander à Claude de le créer/corriger**
   - Spécifiez le titre du livre
   - Indiquez la langue (PT ou FR)
   - Donnez l'ASIN correct

2. **Modifier manuellement avec un éditeur**
   - Utilisez Notepad++ ou VS Code
   - Encodage UTF-8 obligatoire
   - Vérifiez les liens Amazon

3. **Copier depuis un fichier existant**
   - Prenez un fichier qui fonctionne
   - Modifiez le contenu (titre, description, ASIN)
   - Sauvegardez sous le nouveau nom

---

## 📞 BESOIN D'AIDE ?

Si vous ne savez pas :
- Où trouver vos fichiers HTML
- Comment vérifier les ASIN
- Comment corriger un fichier

**Revenez dans Claude avec votre question !**

---

## 🎯 PROCHAINE ÉTAPE

Une fois que vous avez **LES 12 FICHIERS HTML** dans votre dossier :

1. ✅ Vérifiez avec la **CHECKLIST_VERIFICATION.md**
2. ✅ Lisez le **GUIDE_INSTALLATION.md** (méthode complète)
3. ✅ OU lisez le **GUIDE_RAPIDE_CMD.md** (commande unique)
4. 🚀 Lancez le déploiement avec **DEPLOY_MANIALIBRIS.bat**

---

## 🌐 RÉSULTAT FINAL

Après le déploiement, vos visiteurs pourront :

✅ Voir tous vos livres sur **manialibris.com**
✅ Cliquer sur "Acheter sur Amazon"
✅ Être redirigés vers le **bon Amazon** (BR ou FR)
✅ Voir le **bon livre** avec le bon ASIN
✅ Acheter immédiatement !

**Bonne chance avec votre déploiement !** 🚀

---

**Version :** 2.0 - Correction Liens Amazon  
**Date :** Novembre 2025  
**Auteur :** Claude pour Mania Libris
