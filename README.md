# Zerom Electronique

## 📱 Description

**Zerom Electronique** est un site e-commerce moderne pour la vente d'électronique et d'accessoires. C'est un projet portfolio développé avec HTML5, CSS3, JavaScript vanilla et Bootstrap.

### Caractéristiques principales :
- 🏠 Page d'accueil avec slider de bannière
- 💻 Catalogue de produits (Ordinateurs, Téléphones, Accessoires)
- 📋 Formulaire de contact fonctionnel
- 📱 Design responsive (Mobile First)
- 🎨 Interface moderne et professionnelle
- 🔍 Navigation intuitive

---

## 🛠️ Technologies Utilisées

### Frontend
- **HTML5** : Structure sémantique
- **CSS3** : Styling avancé et animations
- **JavaScript** : Interactions dynamiques
- **Bootstrap** : Framework responsive
- **jQuery** : Manipulations DOM
- **jQuery Plugins** :
  - OwlCarousel (sliders produits)
  - FancyBox (galerie lightbox)
  - NiceScroll (scrollbars personnalisées)
  - jQuery Validate (validation formulaires)

### Polices de caractères
- Poppins (Google Fonts)
- Rajdhani (Google Fonts)
- Baloo Chettan (custom)

---

## 📁 Structure du Projet

```
Zerom Electronique/
├── index.html                 # Page d'accueil
├── computers.html             # Catalogue ordinateurs
├── mans_clothes.html          # Téléphones et accessoires
├── womans_clothes.html        # Autres accessoires
├── contact.html               # Formulaire de contact
├── css/                       # Feuilles de styles
│   ├── style.css             # Styles principaux
│   ├── responsive.css        # Styles responsive
│   ├── bootstrap.min.css     # Framework Bootstrap
│   └── [autres fichiers CSS]
├── js/                        # Scripts JavaScript
│   ├── custom.js             # Scripts personnalisés
│   ├── jquery-3.0.0.min.js   # Bibliothèque jQuery
│   └── [plugins jQuery]
├── images/                    # Ressources images
├── .gitignore               # Fichiers à ignorer
└── README.md               # Ce fichier

```

---

## 🚀 Démarrage Rapide

### Installation
1. Clonez le repository :
```bash
git clone https://github.com/[votre-username]/Zerom-Electronique.git
cd Zerom-Electronique
```

2. Ouvrez le projet dans votre navigateur :
   - Ouvrez `index.html` directement ou
   - Utilisez un serveur local (Live Server VS Code, Python http.server, etc.)

### Utilisation en local
```bash
# Démarrer avec Python 3
python -m http.server 8000

# Ou avec Python 2
python -m SimpleHTTPServer 8000
```

Accédez à : `http://localhost:8000`

---

## 📝 Pages du Site

| Page | URL | Description |
|------|-----|-------------|
| Accueil | `index.html` | Page principale avec slider et catégories |
| Ordinateurs | `computers.html` | Catalogue de produits informatiques |
| Téléphones | `mans_clothes.html` | Téléphones et accessoires mobiles |
| Accessoires | `womans_clothes.html` | Autres accessoires électroniques |
| Contact | `contact.html` | Formulaire de prise de contact |

---

## 🎨 Palette de Couleurs

- **Primaire** : #143a51 (Bleu foncé)
- **Accent** : #ff5d68 (Rose/Rouge)
- **Gris clair** : #f8f9fa
- **Texte** : #666666 (Gris moyen) / #111111 (Gris foncé)

---

## 🔧 Fonctionnalités JavaScript

### Sliders/Carousels
- Banner rotator (OwlCarousel)
- Product slider (OwlCarousel)
- Blog post carousel

### Interactions
- Menu sidebar responsive
- Tooltips Bootstrap
- Sticky header au scroll
- Smooth scroll vers les ancres
- Form validation (jQuery Validate)
- Animation au scroll

### Plugins
- **NiceScroll** : Scrollbars personnalisées
- **MeanMenu** : Menu mobile
- **FancyBox** : Galerie lightbox
- **Swiper** : Mobile-friendly sliders

---

## 📱 Responsive Design

Le site est optimisé pour tous les appareils :
- 📱 **Mobile** : 280px - 599px
- 📱 **Tablet** : 600px - 991px
- 💻 **Desktop** : 992px+

Points de rupture Bootstrap :
- `col-md-4`, `col-md-12`, etc.

---

## 🐛 Dépannage

### Le preloader ne disparaît pas
- Vérifier le timeout dans [custom.js](js/custom.js#L15) (1500ms par défaut)

### Le menu mobile ne fonctionne pas
- Vérifier que l'ID du sidenav est `mySidenav`
- Vérifier les fonctions `openNav()` et `closeNav()`

### Les carousels ne défilent pas
- Vérifier que OwlCarousel est chargé correctement

---

## 📚 Documentation des Plugins

### OwlCarousel
Configuration du slider produits dans [custom.js](js/custom.js#L115+) :
- 1 item sur mobile
- 2 items sur tablette
- 3-4 items sur desktop

### jQuery Validate
Configuration du formulaire de contact dans [custom.js](js/custom.js#L182+) :
- Validation en temps réel
- Messages d'erreur personnalisés

---

## 🤝 Contribution

Les contributions sont bienvenues ! Pour contribuer :

1. Fork le projet
2. Créez une branche pour votre feature (`git checkout -b feature/AmazingFeature`)
3. Committez vos changements (`git commit -m 'Add some AmazingFeature'`)
4. Poussez vers la branche (`git push origin feature/AmazingFeature`)
5. Ouvrez une Pull Request

---

## 📄 Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

---

## 👤 Auteur

**Votre Nom**
- GitHub : [@votre-username](https://github.com/votre-username)
- Email : votre.email@exemple.com

---

## 📞 Support

Pour toute question ou problème, veuillez ouvrir une **Issue** sur le repository GitHub.

---

## 🎯 Roadmap / À venir

- [ ] Intégration backend Node.js/Express
- [ ] Base de données MongoDB/MySQL
- [ ] Système de panier d'achat
- [ ] Authentification utilisateur
- [ ] Paiement en ligne (Stripe)
- [ ] Dashboard administrateur
- [ ] Système de commentaires produits
- [ ] Wishlist utilisateur

---

## 📊 Statistiques

- **Fichiers HTML** : 5
- **Fichiers CSS** : 13+
- **Fichiers JS** : 15+
- **Images** : [À compléter]
- **Responsive** : ✅ 100%

---

**Dernière mise à jour** : Janvier 2026

⭐ Si ce projet vous plaît, n'oubliez pas de laisser une star !
