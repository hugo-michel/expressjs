# ExpressJS

Ce repo contient une appli express.js de type 'hello world' pour tester le deploiement.

## Installation en local

```bash
git clone https://github.com/hugo-michel/expressjs
cd expressjs
npm install
```

### Utilisation

```bash
node app.js
```

[http://localhost:3000](http://localhost:3000)

## Deploiement sur render.com

Prérequis: un compte Github.

- (optionnel) Forkez un repository ou creez-en un nouveau sur Github si nécessaire.
- Creez un compte sur [https://render.com](https://render.com).
- Creez un nouveau web service en claiquant sur l'icone "+"
- Choisissez l'option "Build and deploy from a GitHub repo"
- Cliquez sur "Connect account" dans la section "GitHub" à droite
- Vous vous retrouverez sur le site de GitHub
- Tapez votre mot de passe GitHub
- Selectionnez le repository que vous voulez publier
- Confirmez les permissions accordées
- Vous revenez sur le site de Render
- Cliquez sur le bouton "Connect" du repository que vous voulez publier
- Remplissez les champs avec les données suivantes :

```
	Name: [sous-domaine-de-votre-appli]
	Region: Frankfurt (EU Central)
	Branch: main
	Root Directory: <nc>
	Build Command: npm install
	Start Command: node app.js
	Instance Type: Free
```

Remplacez `[sous-domaine-de-votre-appli]` par le sous domaine souhaité.
Exemple : `foo` donnera `https://foo.onrender.com`

- Validez la configuration puis visitez le lien quand le build est terminé

### Mise à jour sur render.com

- Mettez le code à jour en local
- Commitez votre code avec `git add` et `git commit`
- Poussez votre code sur Github avec `git push`
- Verifiez que le code est à jour sur render.com
