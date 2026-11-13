# CalibreTonCV : mise en ligne

Ce dossier est le site complet. Il n'a besoin d'aucun serveur particulier ni d'aucune base de données : n'importe quel hébergeur de pages web suffit.

## Contenu du dossier

| Fichier | Rôle |
|---|---|
| `index.html` | Le site (analyse, note, SWOT, CV annoté, exports) |
| `mentions-legales.html` | Mentions légales, **à compléter avant la mise en ligne** |
| `vendor/` | Lecteurs PDF et Word, création des fichiers PDF et Word |
| `fonts/` | Polices du site |
| `favicon.svg` | Icône de l'onglet |
| `robots.txt` | Autorise les moteurs de recherche |

Gardez tous les fichiers ensemble, sans les renommer : `index.html` va les chercher par leur nom.

## Avant de publier

1. Ouvrez `mentions-legales.html` dans un éditeur de texte et remplacez chaque passage surligné « À COMPLÉTER ».
   - Un particulier qui édite un site à titre non professionnel peut, selon la loi française, n'afficher que les coordonnées de son hébergeur, à condition de lui avoir communiqué son identité. Dès que le site devient une activité professionnelle, l'identité de l'éditeur doit figurer. En cas de doute, vérifiez sur service-public.fr ou auprès d'un juriste.
2. Faites un essai : déposez un CV, téléchargez le rapport PDF, préparez une réécriture.

## Mettre en ligne

### Le plus rapide : Netlify Drop
1. Allez sur app.netlify.com/drop.
2. Glissez le dossier `calibretoncv-site` entier sur la page.
3. Le site est en ligne en quelques secondes, à une adresse en `netlify.app`.
4. Créez un compte pour conserver le site : sans compte, il est supprimé au bout d'une heure.
5. Pour mettre à jour, glissez le nouveau dossier dans l'onglet des déploiements du site.

### Autres hébergeurs
- **Vercel** (vercel.com/drop), **Cloudflare Pages**, **GitHub Pages** : même principe, on dépose le dossier.
- **Hébergement classique** (OVH, o2switch, Infomaniak) : envoyez le contenu du dossier par FTP dans le répertoire `www` ou `public_html`.

### Nom de domaine
Achetez le nom chez un registraire (OVH, Gandi, Infomaniak), puis reliez-le au site depuis les réglages « Domaines » de votre hébergeur. Le certificat HTTPS est en général fourni automatiquement.

## Ce qui diffère de la version dans Claude

- **Fonctions d'IA** (avis rédigé, réécriture, lettre, LinkedIn, entretien) : le site prépare la demande complète, CV inclus, et le visiteur la colle dans l'assistant IA de son choix. Pour la réécriture, il colle ensuite la réponse dans le site pour la noter et la télécharger en Word.
- **Aucun service tiers** : polices et bibliothèques sont dans le dossier. Le site n'appelle rien d'extérieur.
- **Téléchargements** : les fichiers PDF et Word se téléchargent directement.

Pour une IA intégrée (le visiteur clique et obtient la réécriture dans le site), il faut un petit serveur qui détient une clé d'API et paie chaque utilisation. Ce n'est pas inclus ici.

## Limites à connaître

- La note est une estimation. Elle n'est validée contre aucun logiciel de recrutement réel.
- Les listes de mots-clés (français et anglais) et les formations suggérées ont été rédigées à la main et méritent une relecture par secteur.
- Les CV en allemand sont lus, mais sans liste de mots-clés allemande.
- Le contrôle d'orthographe ne repère que les fautes les plus courantes.
