# Torn-city-fr-guide

Guide français de Torn City : https://durkskull.github.io/Torn-city-fr-guide/

## Structure du site

Chaque page a **un seul rôle**, et chaque information n'est écrite qu'à
**un seul endroit**. Quand une autre page en a besoin, elle met un lien
au lieu de recopier.

| Page | Rôle unique |
|---|---|
| `index.html` | Accueil et point d'entrée vers les 5 guides |
| `guide-debutant.html` | Parcours du débutant jusqu'au niveau 15 |
| `voyages.html` | Destinations, temps de vol, réductions de temps |
| `fleurs-peluches.html` | Prix d'achat des fleurs et peluches, sets du musée, taxe de vente |
| `contrebande.html` | Prix et marges de la contrebande, conditions de déblocage |
| `gagner-argent.html` | Méthode : choisir, calculer sa marge, checklist avant de partir |

Ordre de lecture conseillé : Débuter → Voyages → Fleurs & peluches →
Contrebande → Gagner de l'argent. Chaque page se termine par un seul lien
« Étape suivante ».

## Règles à garder en tête

- **Prix et marges** : uniquement dans `fleurs-peluches.html` et
  `contrebande.html`. Ne pas les recopier ailleurs, ils changent.
- **Styles** : uniquement dans `css/style.css`. La politique CSP des pages
  (`style-src 'self'`) bloque les balises `<style>` et les attributs
  `style=""`.
- **Images** : uniquement dans `img/` (la CSP n'autorise que les fichiers
  du dépôt). `img/skyline.svg` est une création originale : ne pas y
  mettre d'éléments tirés du jeu.
- **Menu** : identique sur toutes les pages (voir `nav` dans chaque fichier).
- **Nouvelle page** : l'ajouter au menu de chaque page, à `sitemap.xml`
  et à la liste de cartes de `index.html`.
