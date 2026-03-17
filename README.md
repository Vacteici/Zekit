# zekit.fr — Site officiel ZEKIT v1

Site statique deployé sur GitHub Pages avec domaine custom zekit.fr.

## Structure
- `index.html` — Site principal
- `callback.html` — Redirect OAuth Discord
- `CNAME` — Domaine custom zekit.fr
- `download/` — Dossier pour l'EXE (à créer)

## Configuration DNS pour zekit.fr
Ajoute ces enregistrements chez ton registrar :
```
A     @    185.199.108.153
A     @    185.199.109.153
A     @    185.199.110.153
A     @    185.199.111.153
CNAME www  TON_PSEUDO.github.io
```

## Déploiement
1. Push sur la branche `main`
2. GitHub Actions déploie automatiquement
3. Active GitHub Pages dans Settings → Pages → Source: GitHub Actions

## Config Discord Developer Portal
- Redirect URI OAuth2 : `https://zekit.fr/callback`
