# Guide d'Intégration - Page Cas d'usage AgenticX5

## 📁 Structure des Fichiers

```
votre-site/
│
├── cas-usage-index.html          # Page principale (celle que vous venez de recevoir)
│
└── use-cases/                     # Répertoire des cas d'usage détaillés
    ├── chutes-hauteur/
    │   └── index.html
    ├── bim-4d-5d/
    │   └── index.html
    ├── contacts-electriques/
    │   └── index.html
    ├── tms-canal-carpien/
    │   └── index.html
    ├── espaces-clos/
    │   └── index.html
    ├── protection-oculaire/
    │   └── index.html
    ├── glissades-plain-pied/
    │   └── index.html
    ├── incendie-evacuation/
    │   └── index.html
    ├── formation-outils/
    │   └── index.html
    ├── conditions-meteo/
    │   └── index.html
    ├── acces-urgence/
    │   └── index.html
    └── optimisation-planning/
        └── index.html
```

## 🎨 Caractéristiques du Design (Style Wope)

### Palette de Couleurs
- **Fond** : Gradient sombre (`#0a0a1a` → `#1a0a2e` → `#16213e`)
- **Accent principal** : Gradient violet-rose (`#a78bfa` → `#ec4899`)
- **Texte principal** : `#e0e0e0`
- **Texte secondaire** : `#b0b0b0` / `#b8b8b8`

### Effets Visuels
- **Glassmorphism** : Cartes avec `backdrop-filter: blur(10px)`
- **Étoiles animées** : Animation de scintillement en arrière-plan
- **Hover effects** : Transform, ombres portées, bordures dégradées
- **Transitions fluides** : `cubic-bezier(0.4, 0, 0.2, 1)`

### Typographie
- **Titres H1** : 4rem, text-shadow avec effet glow
- **Titres cartes** : 1.7rem
- **Corps de texte** : 1.05rem, line-height 1.7

## 📊 Cas d'Usage Intégrés (12 au Total)

### 1. **Chutes de hauteur** 🏗️
- **Réduction incidents** : -60%
- **Technologies** : Vision YOLO, Oracle HSE, Wearables
- **Conformité** : RSST Art. 352, CSTC 2.9.1

### 2. **BIM 4D/5D & Jumeaux Numériques** 🏢
- **Réduction incidents phase chantier** : -67%
- **Coûts correctifs évités** : -82%
- **Standards** : ISO 19650, IFC 4.3, buildingSMART

### 3. **Contacts électriques** ⚡
- **Réduction contacts** : -70%
- **Prévention arcs électriques** : -85%
- **Conformité** : CSA Z462, NFPA 70E, RSST Art. 185-195

### 4. **TMS - Syndrome du canal carpien** 🖐️
- **Cas CNESST annuels** : 8,923
- **Réduction potentielle** : -30%
- **Technologies** : Wearables IMU, Score HAL/TLV ACGIH

### 5. **Gestion espaces clos** 🚪
- **Objectif** : Zéro décès
- **Conformité RSST** : 100%
- **Technologies** : PTW Digital, Capteurs gaz, Géolocalisation

### 6. **Protection oculaire - Soudage** 👁️
- **Réduction blessures** : -75%
- **Taux détection** : 97%
- **Standards** : CSA Z94.3, EN 166, ANSI Z87.1

### 7. **Glissades & chutes plain-pied** 💧
- **Chutes annuelles QC** : 34,200+
- **Réduction incidents** : -55%
- **Technologies** : Capteurs IoT, Vision surfaces, AlertX

### 8. **Incendie & évacuation** 🚨
- **Temps évacuation** : <3 minutes
- **Comptage temps réel** : 100%
- **Modules** : Router Agent, AlertX, Dashboard Zones

### 9. **Formation outils électriques** 🔧
- **Amélioration rétention** : +85%
- **Réduction incidents** : -40%
- **Technologies** : BehaviorX, SafetyAgent IA, Gamification

### 10. **Adaptation conditions météo** 🌤️
- **Réduction retards météo** : -45%
- **Conformité CSA** : 100%
- **Technologies** : Simulation 4D, APIs météo, WorkflowX

### 11. **Validation accès d'urgence** 🚑
- **Monitoring** : 24/7
- **Voies dégagées** : 100%
- **Technologies** : BIM 4D Analysis, NFPA Standards

### 12. **Ordonnancement sécuritaire** 📅
- **Réduction conflits sécurité** : -52%
- **Gain efficacité** : +35%
- **Technologies** : WorkflowX Agent, Optimisation ML

## 🔗 Liens de Navigation

Chaque carte contient un lien vers :
```html
<a href="/use-cases/[nom-cas]/index.html" class="card-link">
```

**Important** : Ajustez les chemins selon votre structure :
- Si la page est à la racine : `/use-cases/...`
- Si dans un sous-dossier : `../use-cases/...` ou chemin relatif

## 📱 Responsive Design

La page est **entièrement responsive** :
- **Desktop** : Grille 3 colonnes (min 380px par carte)
- **Tablette** : Grille 2 colonnes
- **Mobile** : Grille 1 colonne

Breakpoint principal : `768px`

## ✨ Fonctionnalités JavaScript

### Animation des Étoiles
```javascript
createStars() // Génère 100 étoiles aléatoires
```

### Intersection Observer
- Détecte l'apparition des cartes dans le viewport
- Animation `fadeInUp` progressive
- Améliore les performances

## 🎯 Appels à l'Action (CTA)

3 boutons principaux :
1. **Demander une Démo** (primary)
2. **Télécharger le Livre Blanc** (secondary)
3. **Nous Contacter** (secondary)

**À configurer** : Remplacez `#demo`, `#whitepaper`, `#contact` par vos URLs réelles

## 📊 Statistiques Globales

Section affichant l'impact mesurable :
- **-67%** Réduction Incidents
- **89.4%** Précision Prédictive
- **<2s** Temps de Réaction
- **+92%** Conformité Réglementaire
- **10+** Cas d'usage Actifs

## 🏢 Footer

Branding :
- **GenAISafety** × **Preventera** × **SquadrAI**
- Standards : ISO 45001, RSST, CSTC, CSA, OSHA, ANSI, C-25
- Validation recherches : MDPI, NIOSH

## 🚀 Installation

### Option 1 : Intégration directe
```html
<!-- Placez cas-usage-index.html à la racine de votre site -->
<a href="/cas-usage-index.html">Voir les cas d'usage</a>
```

### Option 2 : Intégration dans navigation
```html
<nav>
  <a href="/">Accueil</a>
  <a href="/cas-usage-index.html">Cas d'usage</a>
  <a href="/solutions">Solutions</a>
</nav>
```

### Option 3 : Iframe (si nécessaire)
```html
<iframe src="/cas-usage-index.html" 
        width="100%" 
        height="100%" 
        frameborder="0">
</iframe>
```

## 🎨 Personnalisation CSS

### Changer les couleurs d'accent
```css
/* Remplacez les gradients violet-rose */
background: linear-gradient(135deg, #VOTRE_COULEUR1 0%, #VOTRE_COULEUR2 100%);
```

### Ajuster l'espacement
```css
.container {
    max-width: 1400px; /* Modifiez selon vos besoins */
    padding: 40px 20px; /* Ajustez les marges */
}
```

### Modifier la police
```css
body {
    font-family: 'Votre Police', -apple-system, BlinkMacSystemFont, sans-serif;
}
```

## 📈 Performance

### Optimisations incluses :
✅ CSS minimal inline (pas de fichiers externes)  
✅ Animation au scroll (Intersection Observer)  
✅ Images optimisées via émojis (pas de fichiers lourds)  
✅ JavaScript léger (~2KB)  
✅ Compatible tous navigateurs modernes

## 🔒 Conformité & Standards

Le code respecte :
- ✅ **HTML5 Sémantique** (`<article>`, `<section>`, `<header>`, `<footer>`)
- ✅ **Accessibilité** (contraste, taille texte, navigation clavier)
- ✅ **SEO-friendly** (balises meta, structure H1-H2)
- ✅ **Mobile-first** (responsive design)

## 📞 Support

Pour toute question sur l'intégration :
- **GenAISafety** : [contact@genaisafety.com]
- **Preventera** : [info@preventera.ca]
- **Documentation** : Voir les connaissances du projet AgenticX5

---

**Version** : 1.0  
**Date** : Octobre 2025  
**Auteur** : Claude (Anthropic) pour GenAISafety × Preventera  
**Licence** : Propriétaire GenAISafety