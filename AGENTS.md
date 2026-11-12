# Consignes du projet clinique-ribaucourt.com

Répondre toujours en français.

## Cadre de travail

- Reprendre le développement à partir des fichiers présents dans ce dossier.
- Conserver les contenus et les modifications existantes. La demande du 12 novembre 2026 autorise une refonte du style et de la police inspirée de https://dentaleducation.be/.
- Travailler localement pour l’instant. Ne pas déployer ni modifier le domaine ou ses DNS sans demande explicite.

## Contenu à conserver

- Horaires : du lundi au vendredi, de 9h à 17h.
- Le Dr Zakia Ouzzane est médecin généraliste ET dentiste.
- Garder les prises de sang ; supprimer la mésothérapie si elle réapparaît.
- Conserver les illustrations des huit soins, présentes dans `soins-illustrations.png`.
- Conserver les portraits du Dr Fouad Abarkan (`fouad-abarkan.webp`) et du Dr Omar Al Bairat (`omar-al-bairat.webp`).

## Hébergement et domaine

- Hébergement prévu : Cloudflare, en remplacement de Netlify.
- La migration du domaine n’a pas été confirmée. Ne pas considérer les références à Cloudflare dans les pages comme une preuve de migration effective.

## Prochaine évolution

- Intégrer la réservation Doctoranytime avec son bouton ou widget officiel.
- Le code officiel reste à récupérer ; ne pas inventer de code, de lien ou d’identifiant de réservation.
- Ne pas créer un agenda indépendant avec D1.
- Lors de l’intégration, vérifier les adaptations nécessaires dans `_headers` (politique CSP) et dans la page de confidentialité selon le code officiel reçu.

## Informations manquantes

- Raison sociale.
- Numéro BCE.
- E-mail public.
- Conventionnement du Dr Omar Al Bairat.

Ne pas inventer ces informations ni déduire le conventionnement du Dr Omar de celui des autres praticiens.

## Repères techniques constatés dans les fichiers locaux

- Site statique sans fichier `package.json` ni étape de compilation présente dans le dossier.
- `index.html` : page principale, scripts intégrés, huit soins, équipe, rendez-vous téléphoniques, horaires et contact.
- `mentions-legales.html`, `confidentialite.html` et `404.html` : pages complémentaires utilisant `styles.css`.
- `_headers` : en-têtes de sécurité, dont la politique CSP.
- `robots.txt` et `sitemap.xml` : référencement.
- La carte Google Maps se charge après une action explicite de l’utilisateur.
- Les prises de sang sont présentes et la mésothérapie est absente de la version examinée.
- Aucune intégration Doctoranytime n’est présente dans la version examinée.

## Refonte graphique du 12 novembre 2026

- Feuille de style commune : `styles.css`.
- Inspiration : https://dentaleducation.be/, bleu #3434FF, blanc et bleu nuit, boutons peu arrondis et grands titres.
- Police Plus Jakarta Sans stockée localement dans `fonts/`.
- Contenus, illustrations, portraits et fonctions existantes conservés.
