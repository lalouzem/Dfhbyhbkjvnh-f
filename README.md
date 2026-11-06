# Mes délais.

Choisissez une situation (amende, achat en ligne, préavis, licenciement…), entrez une date : le site calcule les échéances et exporte un fichier calendrier (.ics) avec rappels à J-14, J-7 et J-2.

- Site statique (HTML/CSS/JS pur), aucune dépendance, aucune donnée envoyée ni enregistrée
- Fonctionne hors connexion après la première visite (HTTPS requis)
- Règles version 2026-11-06.2, vérifiées le 6 novembre 2026 : voir `SOURCES.md`. Un bandeau d'alerte s'affiche seul 90 jours après la date de vérification (constante `VERIF_ISO` dans `index.html`).

**Statut : version de test.** Règles vérifiées sur sources officielles, mais non validées par un juriste et export calendrier non testé sur Apple Calendrier, Google Agenda et Outlook. Ne pas présenter comme calculateur juridique fiable avant ces validations. Une « date prudente » n'est pas la date limite légale.

## Publier sur GitHub Pages
1. Créez un dépôt GitHub (ex. `mes-delais`).
2. Envoyez-y tous les fichiers du ZIP à la racine.
3. Dépôt → **Settings** → **Pages**.
4. *Build and deployment* : Source = **Deploy from a branch**, Branch = **main**, dossier **/ (root)** → **Save**.
5. Après 1 à 2 minutes : `https://<votre-nom>.github.io/<depot>/`.

## Avant de partager largement
- Ce site donne de l'information, pas un conseil juridique : le texte l'indique. Gardez cette mention.
- Les règles changent (ex. réforme du droit de rétractation du 19 juin 2026) : revérifiez chaque règle au moins tous les trimestres, et à chaque évolution annoncée sur service-public.gouv.fr.
- Idéalement, faites relire `SOURCES.md` et les règles de `index.html` (constante `RULES`) par un juriste.
- Après modification d'`index.html`, incrémentez `CACHE` dans `sw.js` pour forcer le nettoyage du cache.

## Ajouter une règle
Dans `index.html`, ajoutez un objet à `RULES` : `calc` accepte `days`, `months` ou `quarter2y`; `report: true` n'est à utiliser que si le report au jour ouvrable suivant est confirmé par le texte applicable.
