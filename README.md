# Neon Breaker — Assistance et confidentialité

Site public bilingue d’assistance et de confidentialité pour **Neon Breaker: Station 88**. Ce dépôt contient uniquement les pages statiques et leur documentation de maintenance, sans code ni ressources de l’application.

## Fichiers

| Fichier | Rôle |
| --- | --- |
| `index.html` | Accueil et choix de langue |
| `fr/support.html` | Assistance en français |
| `fr/privacy.html` | Confidentialité en français |
| `en/support.html` | Assistance en anglais |
| `en/privacy.html` | Confidentialité en anglais |
| `style.css` | Style local commun, responsive et sans police externe |
| `.nojekyll` | Publication directe des fichiers, sans traitement Jekyll |

## Maintenance

Modifier les deux langues ensemble et actualiser leurs dates de mise à jour ou d’effet, ainsi que celle de l’accueil. Conserver des liens relatifs pour la navigation et la feuille de style, afin que le site fonctionne dans un sous-répertoire GitHub Pages.

Les pages ne doivent ajouter ni JavaScript, cookies, traceurs, formulaires, publicité, dépendances de compilation ou contenus intégrés distants. Conserver la politique CSP restrictive dans chaque document HTML. Les journaux de sécurité de GitHub Pages, dont l’enregistrement des adresses IP, doivent rester clairement distingués des données locales du jeu dans les deux politiques de confidentialité.

Avant publication, contrôler les coordonnées de l’éditeur, l’équivalence FR/EN, les liens locaux, les ancres, les dates et l’affichage sur petit écran et au clavier. Ne publier ni secrets ni autres fichiers que ceux du site.

Pour un aperçu local avec Python 3 :

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Ouvrir `http://127.0.0.1:8000/`, puis parcourir les quatre pages et leurs liens de changement de langue. Arrêter le serveur avec `Ctrl+C`.

## Publication

Les modifications passent par une pull request vers `main`. Dans **Settings → Pages**, la source est **Deploy from a branch**, branche **main**, dossier **/ (root)**. Garder **Enforce HTTPS** activé. Aucun domaine personnalisé ni workflow de compilation personnalisé n’est nécessaire.

Après fusion, attendre la réussite du déploiement GitHub Pages, puis vérifier anonymement en HTTPS l’accueil, les quatre pages localisées et `style.css`.

© 2026 Mouhamadou DIALLO. Tous droits réservés. Aucune licence open source n’est accordée.
