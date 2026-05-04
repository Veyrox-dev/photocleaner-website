# 🚀 GitHub Pages Setup - Schritt für Schritt

## 1️⃣ GitHub Repository erstellen

1. Gehe zu: https://github.com/new
2. Repository Name: **`BestShot-website`** (oder einen kreativen Namen!)
   - Vorschläge für "komische" Namen:
     - `photo-wizard-landing`
     - `snap-cleaner-web`
     - `pic-perfect-site`
     - `image-declutter-page`
3. ✅ **Public** auswählen (wichtig für kostenlose GitHub Pages!)
4. ❌ NICHT "Initialize with README" anklicken (haben wir schon)
5. Klicke "Create repository"

## 2️⃣ Code hochladen

Im Terminal (PowerShell) ausführen:

```powershell
cd "C:\Users\chris\projects\BestShot-website"

# Dateien hinzufügen
git add .

# Commit erstellen
git commit -m "Initial commit: BestShot Website"

# Remote hinzufügen (ERSETZE <username> durch deinen GitHub Username!)
git remote add origin https://github.com/<username>/BestShot-website.git

# Hochladen
git branch -M main
git push -u origin main
```

## 3️⃣ GitHub Pages aktivieren

1. Gehe zu deinem Repository auf GitHub
2. Klicke auf **Settings** (oben rechts)
3. Links im Menü: **Pages**
4. Bei "Build and deployment":
   - **Source**: Deploy from a branch
   - **Branch**: `main` auswählen
   - **Folder**: `/ (root)` auswählen
5. Klicke **Save**

## 4️⃣ Fertig! 🎉

Nach 1-2 Minuten ist deine Website live unter:

```
https://<username>.github.io/BestShot-website/
```

GitHub zeigt die URL oben im Pages-Bereich an!

---

## 🔄 Updates veröffentlichen

Wenn du Änderungen an der Website machst:

```powershell
cd "C:\Users\chris\projects\BestShot-website"
git add .
git commit -m "Update: Beschreibung der Änderung"
git push
```

GitHub Pages baut die Website automatisch neu (dauert ~1 Minute).

---

## 💡 Bonus: Eigene Domain (optional)

Wenn du später eine eigene Domain willst (z.B. `BestShot.de`):

1. Kaufe Domain bei einem Anbieter (Namecheap, Cloudflare, etc.)
2. Erstelle eine `CNAME`-Datei im Repository mit deiner Domain
3. Konfiguriere DNS-Einträge beim Domain-Anbieter
4. In GitHub Settings → Pages: Custom domain eintragen

Details: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

---

## ⚠️ Wichtig zu wissen

- ✅ GitHub Pages ist **100% kostenlos** für Public Repositories
- ✅ Automatische HTTPS/SSL-Verschlüsselung
- ✅ Automatisches Deployment bei jedem `git push`
- ✅ Keine Build-Tools nötig (pure HTML/CSS/JS)
- ⚠️ FormSubmit.co muss beim ersten Absenden bestätigt werden (Email-Check)
