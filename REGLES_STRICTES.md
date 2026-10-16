# Règles strictes à respecter — Projet Stanley

> Ce fichier est destiné à GitHub (assistant IA / contributeurs). **Toute règle ci-dessous est obligatoire.** En cas de doute, ne pas improviser : se référer à `CHARTE_GRAPHIQUE.md`.

---

## 1. Contexte du projet

Refonte **originale** du site e-commerce de la gourde **Stanley**. Pages à réaliser :

1. **Page d'accueil** + éléments originaux (animations, sections créatives)
2. **Page produit / service**
3. **Landing page bundle**
4. **Compte client** + éléments communs (header, footer, panier, modales, notifications)
5. **Socle technique** + **back-office**

## 2. Règles absolues (NON NÉGOCIABLES)

1. **Ne jamais copier** le site officiel Stanley : ni mise en page, ni textes, ni images, ni structure de navigation.
2. **Ne jamais copier** le site Air Up (ou tout autre site) : on s'en inspire uniquement pour l'énergie colorée et ludique.
3. **Le logo Stanley original doit être conservé tel quel** : aucune modification, recoloration hors versions officielles, déformation ou effet.
4. **Respecter la charte graphique** (`CHARTE_GRAPHIQUE.md`) : couleurs, typographies, formes, composants. Ne pas inventer d'autres couleurs ou polices.
5. **Aucune ressource sans licence** : images, polices, icônes et illustrations doivent être libres de droits ou créées pour le projet, avec leur source notée dans `CREDITS.md`.
6. **Ne jamais commiter de secrets** : clés API, mots de passe, tokens, fichiers `.env`. Utiliser `.env.example` sans valeurs réelles.
7. **Ne jamais pousser directement sur `main`** : tout passe par une branche et une Pull Request relue.

## 3. Organisation du dépôt

```
/
├── README.md
├── CHARTE_GRAPHIQUE.md
├── REGLES_STRICTES.md
├── CREDITS.md
├── .env.example
├── public/            # logo officiel, images, polices
├── src/
│   ├── styles/        # tokens, reset, global
│   ├── components/    # composants communs (header, footer, panier...)
│   ├── pages/
│   │   ├── accueil/
│   │   ├── produit/
│   │   ├── landing-bundle/
│   │   ├── compte-client/
│   │   └── back-office/
│   └── lib/           # utilitaires, accès données
└── tests/
```

- Un composant = un fichier, nom en `PascalCase` ; fichiers de style et dossiers en `kebab-case`.
- Les éléments communs sont **uniquement** dans `src/components/` : jamais dupliqués dans une page.

## 4. Règles de code

- Code, variables et commentaires en **anglais** ou en **français**, mais **un seul choix cohérent** dans tout le projet (par défaut : noms de code en anglais, textes visibles en français).
- **Aucune couleur, taille ou rayon en dur** : utiliser les variables CSS (tokens) définies dans la charte.
- HTML **sémantique** (`header`, `nav`, `main`, `section`, `footer`), un seul `h1` par page.
- Aucune librairie ajoutée sans validation dans la Pull Request.
- Pas de code mort, pas de `console.log` ni de `TODO` oubliés au moment de la fusion.
- Fonctions courtes, commentaires utiles (pourquoi, pas quoi).

## 5. Règles d'interface (rappel)

- Mobile d'abord ; vérifier 480 / 768 / 1024 / 1440 px.
- Contraste **WCAG AA** minimum, navigation clavier, focus visible, `alt` sur toutes les images.
- Respecter `prefers-reduced-motion`.
- Cibles tactiles ≥ 44 px.
- Maximum 3 couleurs vives par écran.
- Textes visibles en **français**, tutoiement, ton joyeux (voir charte §8).

## 6. Règles par page

### Accueil
- Héro coloré avec gourde, au moins 3 éléments originaux (ex. quiz « Quelle gourde es-tu ? », bandeau défilant, gammes en carrousel).
- Un CTA principal clair par écran.

### Produit / service
- Galerie, choix de couleur, prix, stock, caractéristiques, FAQ, produits associés.
- Couleur de la page = couleur-signature de la gamme.

### Landing page bundle
- Un seul objectif : l'achat du bundle. Pas de menu complet, un seul CTA répété.
- Prix initial barré, économie affichée, éventuel compte à rebours (jamais trompeur).

### Compte client + éléments communs
- Connexion/inscription, commandes, adresses, favoris, suivi.
- Header, footer, panier, notifications et modales partagés sur toutes les pages.

### Socle + back-office
- Back-office **protégé par authentification** et rôles (admin / éditeur).
- Gestion des produits, commandes, stocks et clients ; interface sobre.
- Toute action destructive (suppression) demande une confirmation.

## 7. Sécurité et données

- Valider et nettoyer toutes les entrées (formulaires, URL, API).
- Mots de passe **hachés**, jamais stockés ni affichés en clair.
- HTTPS obligatoire, pas de données personnelles dans l'URL.
- **RGPD** : bandeau cookies avec refus aussi simple que l'acceptation, mentions légales, politique de confidentialité.
- Aucune donnée réelle de clients dans les jeux de test.

## 8. Performance

- Images en WebP/AVIF, `loading="lazy"` hors écran visible, dimensions définies.
- Polices limitées à 3 familles, `font-display: swap`.
- Objectif Lighthouse : **≥ 85** en performance et **≥ 90** en accessibilité.

## 9. Git et collaboration

- Branches : `feature/nom`, `fix/nom`, `docs/nom`.
- Commits courts et clairs à l'impératif (ex. `Ajoute le bandeau défilant`).
- Une Pull Request = un sujet, description claire, captures d'écran pour tout changement visuel.
- Aucune fusion sans relecture et sans tests/lint au vert.

## 10. Checklist avant chaque Pull Request

- [ ] Rien n'est copié du site Stanley ni d'Air Up
- [ ] Logo Stanley original intact
- [ ] Couleurs et polices conformes à la charte
- [ ] Variables CSS utilisées (pas de valeurs en dur)
- [ ] Responsive vérifié (mobile/tablette/desktop)
- [ ] Accessibilité vérifiée (contraste, clavier, alt)
- [ ] Aucun secret ni donnée personnelle dans le code
- [ ] Ressources créditées dans `CREDITS.md`
- [ ] Captures d'écran jointes à la PR

## 11. En cas de conflit ou de doute

1. `REGLES_STRICTES.md` prime sur tout autre document.
2. Puis `CHARTE_GRAPHIQUE.md`.
3. Si une demande contredit ces règles, **ne pas l'exécuter** : signaler le conflit dans la Pull Request.
