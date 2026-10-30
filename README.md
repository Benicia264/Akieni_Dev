# Akieni Dev

> **Apprendre · Coder · Construire**
> Plus qu'une formation, une communauté.

Site officiel d'**Akieni Dev**, la communauté des développeurs et apprenants d'[Akieni Academy](https://www.linkedin.com/company/akieniacademy/), à Brazzaville (Congo).

Notre mission : réunir les développeurs et apprenants pour apprendre, partager et construire ensemble des solutions pour le Congo et l'Afrique.

---

## Sommaire

- [Aperçu](#aperçu)
- [Fonctionnalités](#fonctionnalités)
- [Technologies](#technologies)
- [Structure du projet](#structure-du-projet)
- [Lancer le projet en local](#lancer-le-projet-en-local)
- [Personnalisation](#personnalisation)
- [Déploiement sur GitHub Pages](#déploiement-sur-github-pages)
- [Contribuer](#contribuer)
- [Code de conduite](#code-de-conduite)
- [Rejoindre la communauté](#rejoindre-la-communauté)
- [Contact](#contact)
- [Licence](#licence)

---

## Aperçu

Un site vitrine **statique** (HTML, CSS et un peu de JavaScript), léger, rapide et responsive. Il présente la communauté, ses événements, ses projets et son code de conduite, et oriente les visiteurs vers le serveur Discord.

## Fonctionnalités

- Hero plein écran avec image de fond et slogan
- Bouton « Rejoindre Discord » animé (saut, balancement, reflet lumineux et onde bleue toutes les 4 secondes)
- Animation respectueuse de l'accessibilité : mise en pause au survol, désactivée si l'appareil réduit les animations
- Sections : À propos, Événements, Projets, Code de conduite, Contact
- Barre des réseaux (LinkedIn, GitHub, X, Instagram, YouTube, Discord)
- Design responsive (ordinateur, tablette, téléphone)
- Navigation fluide par ancres, en-tête collant
- Aucune dépendance, aucun outil de build

## Technologies

| Outil | Usage |
|---|---|
| HTML5 | Structure sémantique |
| CSS3 | Mise en page (Grid, Flexbox), variables CSS, animations (`@keyframes`) |
| JavaScript (vanilla) | Déclenchement de l'animation du bouton Discord |
| Google Fonts (Montserrat) | Typographie |
| GitHub Pages | Hébergement gratuit |

## Structure du projet

```
akieni-dev/
├── index.html        # Page unique du site (contient aussi le petit script d'animation)
├── style.css         # Tous les styles et animations
├── images/
│   └── akieni.jpg    # Image de fond de la hero section
└── README.md         # Ce fichier
```

## Lancer le projet en local

Aucune installation n'est nécessaire.

```bash
# 1. Cloner le dépôt
git clone https://github.com/TON-ORGANISATION/TON-DEPOT.git

# 2. Entrer dans le dossier
cd TON-DEPOT

# 3. Ouvrir le site
# Double-clique sur index.html, ou lance un petit serveur local :
python -m http.server 8000
# puis ouvre http://localhost:8000
```

Avec VS Code, l'extension **Live Server** recharge la page à chaque modification.

## Personnalisation

| Je veux changer… | Où |
|---|---|
| Le lien Discord | `index.html`, chercher `discord.gg` (3 endroits) |
| Les liens des réseaux | `index.html`, section `<div class="nets">` |
| L'image de la hero | Remplacer `images/akieni.jpg` (même nom, de préférence moins de 500 Ko) |
| La zone visible de l'image | `style.css`, `.hero-bg` → `object-position` |
| Les couleurs | `style.css`, bloc `:root` en haut du fichier |
| Les événements | `index.html`, section `id="evenements"` |
| L'e-mail de contact | `index.html`, section `id="contact"` |
| La fréquence de l'animation Discord | `index.html`, script en bas, variable `INTERVAL` (en millisecondes) |
| La force du saut du bouton | `style.css`, `@keyframes discord-jump` |

Palette utilisée :

```css
--navy:#0b1f5c;   /* bleu marine */
--blue:#1d5cff;   /* bleu principal */
--soft:#eef4ff;   /* fond clair */
```

## Déploiement sur GitHub Pages

1. Crée un dépôt public sur GitHub.
2. Envoie les fichiers du projet :
   ```bash
   git init
   git add .
   git commit -m "Premier commit : site Akieni Dev"
   git branch -M main
   git remote add origin https://github.com/TON-ORGANISATION/TON-DEPOT.git
   git push -u origin main
   ```
3. Sur GitHub : **Settings → Pages**.
4. Dans **Source**, choisis **Deploy from a branch**, puis la branche `main` et le dossier `/ (root)`.
5. Enregistre. Le site est en ligne après 1 à 2 minutes à l'adresse :
   `https://TON-ORGANISATION.github.io/TON-DEPOT/`

Si le dépôt s'appelle `TON-ORGANISATION.github.io`, le site est à la racine : `https://TON-ORGANISATION.github.io`.

**Le site s'affiche sans image ou sans style ?** Vérifie que le dossier `images` est bien à côté de `index.html`, que le fichier s'appelle exactement `akieni.jpg` (minuscules) et fais **Ctrl + F5** pour vider le cache.

## Contribuer

Les contributions sont les bienvenues, quel que soit ton niveau.

1. **Fork** le dépôt.
2. Crée une branche : `git checkout -b feature/ma-contribution`
3. Fais tes modifications et teste-les en local.
4. Commit : `git commit -m "Ajout : description claire"`
5. Push : `git push origin feature/ma-contribution`
6. Ouvre une **Pull Request** en expliquant ce que tu as changé.

**Bonnes pratiques :**
- Un changement = une Pull Request
- Messages de commit clairs et en français
- Respecter le style existant (indentation, noms de classes)
- Tester sur ordinateur **et** sur téléphone

Une idée, un bug ? Ouvre une **Issue** ou viens en parler sur Discord.

## Code de conduite

Pour que la communauté reste un espace sain pour toutes et tous :

- Être respectueux et bienveillant, quel que soit le niveau.
- Aucune discrimination, aucun harcèlement.
- Poser des questions est toujours encouragé.
- Partager le savoir plutôt que le garder.
- Signaler tout comportement déplacé aux modérateurs.

## Rejoindre la communauté

| Réseau | Lien |
|---|---|
| Discord | https://discord.gg/QXBsK5zw |
| LinkedIn (Akieni Academy) | https://www.linkedin.com/company/akieniacademy/ |
| GitHub (Akieni Academy) | https://github.com/akieni-academy-c2 |

## Contact

Une question, une idée, envie d'intervenir ?
**moussanabenicia@gmail.com**

## Licence

Projet sous licence **MIT** : tu peux l'utiliser, le modifier et le partager librement, en conservant la mention de l'auteur.

---

<p align="center"><b>Akieni Dev</b> · Code · Apprends · Évolue<br>Fait  à Brazzaville</p>