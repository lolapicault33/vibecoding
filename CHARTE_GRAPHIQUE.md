# Charte graphique — Stanley « Pop & Fantaisie »

> Projet : refonte originale du site de la gourde **Stanley**.
> Inspiration : l'énergie colorée et ludique d'un site comme Air Up, **sans jamais copier** ni son design, ni ses textes, ni ses visuels, ni le site officiel Stanley.

---

## 1. Intention créative

- **Ambiance** : joyeuse, colorée, pleine de fantaisie, qui donne envie de boire de l'eau et d'emporter sa gourde partout.
- **Mots-clés** : pop, gourmand, joueur, robuste, aventurier, accessible.
- **Promesse** : « Une gourde increvable, une personnalité très colorée. »
- **Ce qu'on garde de Stanley** : le logo original, l'esprit robuste et durable du produit.
- **Ce qu'on invente** : tout le reste (couleurs, formes, typos, illustrations, ton, animations).

## 2. Logo (INTOUCHABLE)

- Utiliser **uniquement le logo Stanley original**, fourni en fichier officiel (SVG de préférence).
- Interdit : le recolorer hors versions officielles, le déformer, le pivoter, lui ajouter une ombre/contour/effet, le redessiner.
- **Zone de protection** : espace libre autour du logo = hauteur de la lettre « S ».
- **Taille minimale** : 80 px de large (écran), 20 mm (impression).
- **Fonds autorisés** : crème `#FFF6E5`, blanc, vert Stanley, noir encre. Sur fond coloré vif, utiliser la version blanche ou noire du logo.
- Emplacement : en haut à gauche du header, cliquable vers l'accueil.

## 3. Palette de couleurs

### Couleurs de marque
| Nom | HEX | Usage |
|---|---|---|
| Vert Stanley | `#2E5E4E` | Couleur héritée du logo, ancrage de marque, footer, boutons secondaires |
| Mangue | `#FFB627` | Couleur d'énergie, accents, badges, surlignages |
| Framboise | `#FF3D7F` | CTA principal, promos, éléments « wow » |
| Lagon | `#19C3C0` | Fraîcheur, liens, états actifs |
| Prune | `#6B3FA0` | Fonds de sections, bundles, premium |
| Pistache | `#B6E36B` | Succès, éco / durable, stickers |

### Neutres
| Nom | HEX | Usage |
|---|---|---|
| Crème | `#FFF6E5` | Fond principal du site |
| Blanc | `#FFFFFF` | Cartes, formulaires |
| Encre | `#1B1B2F` | Texte principal, contours |
| Brume | `#E9E4D8` | Bordures, séparateurs |
| Gris doux | `#6E6A7C` | Texte secondaire |

### États (back-office et formulaires)
- Succès `#2E9E5B` · Alerte `#F5A300` · Erreur `#D92D4A` · Info `#2F7DE1`

### Règles d'usage
- Proportions : 60 % neutres (crème/blanc) · 30 % couleurs de marque · 10 % accents vifs.
- **Maximum 3 couleurs vives par écran** pour garder la lisibilité.
- Contraste texte/fond conforme **WCAG AA** (4.5:1 minimum). Texte clair sur Framboise, Prune et Vert ; texte Encre sur Mangue, Lagon, Pistache.
- Chaque gamme de gourde a sa couleur-signature qui teinte sa page produit.

## 4. Typographies

| Rôle | Police (Google Fonts, libres de droits) | Réglages |
|---|---|---|
| Titres (H1/H2) | **Bagel Fat One** — ronde, joueuse | Casse normale, interligne 1.05 |
| Sous-titres / boutons | **Fredoka** (600) | Interligne 1.2 |
| Texte courant | **DM Sans** (400/500) | 16–18 px, interligne 1.6 |
| Accent manuscrit (rare) | **Caveat** | Annotations, stickers, flèches |

- Échelle : 14 / 16 / 20 / 28 / 40 / 56 / 80 px (version mobile : -25 %).
- Un seul titre H1 par page.
- Interdit : plus de 3 polices, texte justifié, titres tout en majuscules sur plus de 3 mots.
- Prévoir `font-display: swap` et une police de secours (`system-ui, sans-serif`).

## 5. Formes, illustrations et fantaisie

- **Formes** : coins très arrondis (rayon 24 px cartes, 999 px boutons), blobs organiques, vagues, gouttes, bulles.
- **Stickers & mascotte** : petites étoiles, gouttes souriantes, éclaboussures ; illustrations vectorielles originales créées pour le projet.
- **Séparateurs de sections** : vagues SVG colorées plutôt que lignes droites.
- **Contours** : trait Encre 2–3 px sur cartes/boutons pour un effet « sticker » avec ombre décalée (`4px 4px 0 Encre`).
- **Photos** : gourdes en situation (rando, sport, bureau, voyage) sur fonds colorés unis ; ambiance lumineuse, saturée mais naturelle. Jamais de photos extraites d'autres sites.
- **Icônes** : un seul jeu cohérent (trait 2 px, bouts arrondis).

## 6. Composants UI

### Boutons
- **Primaire** : fond Framboise, texte blanc, contour Encre, ombre décalée ; au survol, il « se soulève » (translate -2 px).
- **Secondaire** : fond Vert Stanley, texte blanc.
- **Tertiaire** : texte souligné ondulé, sans fond.
- Hauteur minimale 48 px (zone tactile), texte à l'impératif et court (« Je craque », « Composer mon bundle »).

### Cartes produit
- Fond blanc, bordure Encre, visuel de la gourde sur fond de la couleur de la gamme, pastille de prix, badge « Nouveau » / « -20 % » en sticker incliné (-6°).

### Formulaires
- Champs arrondis, label toujours visible, erreur en texte + icône (jamais la couleur seule).

### Navigation
- Header collant, logo à gauche, menu central, icônes compte/panier à droite ; menu burger sur mobile.

## 7. Mouvement et interactions

- Durées : 150–300 ms, courbe `ease-out` ; rebond léger autorisé sur les stickers et boutons.
- Animations autorisées : gourde qui flotte, bulles qui montent, vagues qui ondulent, confettis à l'ajout au panier.
- **Respecter `prefers-reduced-motion`** : désactiver les animations non essentielles.

## 8. Ton éditorial

- Tutoiement chaleureux, phrases courtes, humour léger, jeux de mots autour de l'eau.
- Pas de jargon, pas de promesses santé non prouvées.
- Exemples : « Ta gourde, ton humeur. » · « Hydrate-toi, fais pas ton cactus. »

## 9. Déclinaison par page

| Page | Ambiance visuelle |
|---|---|
| **Accueil + éléments originaux** | Héro plein écran multicolore, gourde flottante, carrousel de gammes, bandeau défilant, section « Quelle gourde es-tu ? », avis clients en bulles |
| **Page produit / service** | Fond teinté de la couleur de la gamme, galerie photo, sélecteur de couleur en pastilles, caractéristiques en icônes, FAQ, produits associés |
| **Landing page bundle** | Fond Prune, composeur de bundle interactif (gourde + accessoires), prix barré/économie bien visibles, compte à rebours, un seul CTA |
| **Compte client + éléments communs** | Tons plus calmes (crème/blanc) pour la clarté, tableau de bord commandes, adresses, favoris ; header, footer, panier, modales et notifications partagés |
| **Socle + back-office** | Interface sobre et lisible (neutres + vert Stanley), pastilles de statut colorées, tableaux, formulaires de gestion produits/commandes/stocks, touches de fantaisie limitées (mascotte sur états vides) |

## 10. Accessibilité et responsive

- Mobile d'abord ; points de rupture : 480 / 768 / 1024 / 1440 px.
- Alternatives textuelles sur toutes les images, navigation clavier complète, focus visible (anneau Lagon 3 px).
- Cibles tactiles ≥ 44 × 44 px.

## 11. Tokens de design (référence code)

```css
:root {
  --vert-stanley: #2E5E4E;
  --mangue: #FFB627;
  --framboise: #FF3D7F;
  --lagon: #19C3C0;
  --prune: #6B3FA0;
  --pistache: #B6E36B;
  --creme: #FFF6E5;
  --encre: #1B1B2F;
  --brume: #E9E4D8;
  --rayon-carte: 24px;
  --rayon-bouton: 999px;
  --ombre-sticker: 4px 4px 0 var(--encre);
  --font-titre: "Bagel Fat One", system-ui, sans-serif;
  --font-ui: "Fredoka", system-ui, sans-serif;
  --font-texte: "DM Sans", system-ui, sans-serif;
}
```

## 12. Interdits (rappel)

- Reproduire le site officiel Stanley ou le site Air Up (mise en page, textes, images, mascottes).
- Modifier le logo Stanley.
- Utiliser des images ou polices sans licence.
- Dépasser 3 couleurs vives par écran ou sacrifier la lisibilité pour la fantaisie.
