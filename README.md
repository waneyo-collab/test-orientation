# Test d'orientation professionnelle (RIASEC + Big Five)

Quiz d'orientation professionnelle autonome — 45 questions, modèle RIASEC (Holland) croisé
avec les 5 grands traits de personnalité, 15 combinaisons de profils.

Ceci est une **copie indépendante** du quiz utilisé sur [L'Accélérateur Digital](https://app.waneyo-formation.com),
conservée dans son propre repo pour pouvoir être déployée, modifiée ou cédée séparément
sans dépendre du reste de la plateforme.

## Structure

- `index.html` — page unique : questions, calcul du score, affichage du résultat
- `orientation-quiz.json` — les 45 questions
- `orientation-scoring.js` — logique de scoring (référence ; la version utilisée par la page
  est celle intégrée directement dans `index.html`, adaptée pour le navigateur)

## Déploiement

Site 100% statique, aucune fonction serveur, aucune dépendance à installer.
Sur Netlify : "Add new site" → pointer sur ce repo → déployer tel quel (`netlify.toml` déjà configuré).

## Personnalisation

Le résultat final oriente vers [waneyo-formation.com](https://www.waneyo-formation.com) (lien
"Retour" et bouton "Démarrer mon parcours"). Si ce quiz est cédé ou réutilisé pour un autre
produit, ces deux liens (dans `index.html`) sont à adapter à la nouvelle destination.
