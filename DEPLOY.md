# Deployment Instructions for stiri-simple.github.io

## 🚀 Prima Publicare

### 1. Creează repository-ul pe GitHub

**IMPORTANT**: Repository-ul TREBUIE să se numească exact `stiri-simple.github.io`

```bash
# Pe GitHub:
# 1. Du-te la https://github.com/stiri-simple
# 2. Click "New repository"
# 3. Nume: stiri-simple.github.io (EXACT acest nume!)
# 4. Public repository
# 5. NU adăuga README, .gitignore sau license (le avem deja)
```

### 2. Inițializează și publică

```bash
cd /path/to/stiri-simple.github.io
git init
git add .
git commit -m "Initial commit: Știri Simple portal"
git branch -M main
git remote add origin https://github.com/stiri-simple/stiri-simple.github.io.git
git push -u origin main
```

### 3. Verifică GitHub Pages

GitHub Pages se activează AUTOMAT pentru repository-uri numite `[org-name].github.io`:
- Site-ul va fi disponibil la: https://stiri-simple.github.io
- Durează ~10 minute pentru prima publicare

## 📝 Actualizări Zilnice

După ce generezi conținut nou:

```bash
cd /path/to/stiri-simple.github.io
git add .
git commit -m "Update: $(date '+%Y-%m-%d') știri"
git push
```

## 🔧 Troubleshooting

### Site-ul nu apare?
1. Verifică numele repository-ului: TREBUIE să fie `stiri-simple.github.io`
2. Verifică Settings → Pages → Source: ar trebui să fie setat automat pe `main` branch
3. Așteaptă 10 minute pentru propagare

### Erori 404?
- Verifică că `index.html` există în root
- Verifică că repository-ul este public

## 🌐 URL-uri

- **Direct**: https://stiri-simple.github.io
- **Cu portal**: https://stiri-simple.github.io/?portal=https://zeeguu.github.io/portal

---
*Pentru organizații GitHub, repository-ul `[org-name].github.io` este automat servit ca GitHub Pages*