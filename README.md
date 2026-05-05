# QR Code Generator - datas wca

Générateur de QR Codes personnalisés avec logo pour la Banque mondiale.

## Fonctionnalités

- ✅ Génération de QR Codes vCard (carte de visite)
- ✅ Personnalisation des couleurs (points, coins, fond)
- ✅ Ajout de logo personnalisé
- ✅ Styles de points (arrondi, doux, carré)
- ✅ Ajustement de la taille du QR Code
- ✅ Ajustement de l'arrondi des modules
- ✅ Export PNG haute résolution (300-600 DPI)
- ✅ Couleurs par défaut : Banque mondiale

## Couleurs par défaut (Banque mondiale)

| Élément | Couleur | Code Hex |
|---------|--------|---------|
| Points | Bleu Banque mondiale | #003F87 |
| Coins | Rose Banque mondiale | #E2007A |
| Fond | Blanc | #FFFFFF |

---

## Installation

### Installation locale (Mac/Windows/Linux)

#### Methode 1 :Avec le script inclus (Mac)

```bash
cd QRCode
chmod +x serve.command
./serve.command
```

Puis ouvrez : http://localhost:8080/qrcode2.html

#### Methode 2 : Python (tous OS)

```bash
cd QRCode
python3 -m http.server 8080
```

Puis ouvrez : http://localhost:8080/qrcode2.html

#### Methode 3 : VS Code (Live Server)

1. Installez l'extension **Live Server** dans VS Code
2. Faites clic droit sur `qrcode2.html` > **Open with Live Server**

#### Methode 4 : Node.js

```bash
cd QRCode
npx serve
```

### Arrêter le serveur

```bash
# Methode 1 : Terminal
pkill -f "python3 -m http.server"

# Methode 2 : Activity Monitor (Mac)
# Ouvrez Activity Monitor > Cherchez python3 > Quit

# Methode 3 : Gestionnaire des tâches (Windows)
# Ouvrez Gestionnaire > python.exe > Fin de tâche
```

---

## Déploiement en ligne

### Option 1 : GitHub Pages (Gratuit)

#### Étape 1 : Créer un repo GitHub
1. Allez sur [github.com](https://github.com)
2. Cliquez **New repository**
3. Nommez-le : `qrcode-generator`
4. Cochez **Public**
5. Cliquez **Create repository**

#### Étape 2 : Uploader les fichiers
1. Cliquez **Upload an existing file**
2. Glissez les fichiers :
   - `qrcode2.html`
   - `logo.png` (ou `logo.jpg`)
   - `README.md`
3. Cliquez **Commit changes**

#### Étape 3 : Activer GitHub Pages
1. Allez dans **Settings** > **Pages**
2. Sous **Build and deployment** > **Source**, sélectionnez **Deploy from a branch**
3. Sous **Branch**, choisissez :
   - Branch : `main`
   - Folder : `/(root)`
4. Cliquez **Save**
5. Attendez 1-2 minutes

#### Accéder à votre QR Code Generator
```
https://votre-utilisateur.github.io/qrcode-generator/qrcode2.html
```

---

### Option 2 : GitLab Pages (Gratuit)

#### Étape 1 : Créer un projet GitLab
1. Allez sur [gitlab.com](https://gitlab.com)
2. Cliquez **New project**
3. Nommez-le : `qrcode-generator`
4. Cliquez **Create project**

#### Étape 2 : Uploader les fichiers
1. Cliquez **Upload file**
2. Glissez :
   - `qrcode2.html`
   - `logo.png`
3. Cliquez **Commit changes**

#### Étape 3 : Créer fichier .gitlab-ci.yml
1. Cliquez **New file**
2. Nommez-le : `.gitlab-ci.yml`
3. Ajoutez :
```yaml
pages:
  script:
    - echo "Deploying to GitLab Pages"
  artifacts:
    paths:
      - qrcode2.html
      - logo.png
      - logo.jpg
  only:
    - main
```

4. Cliquez **Commit changes**

#### Accéder à votre QR Code Generator
```
https://votre-utilisateur.gitlab.io/qrcode-generator/qrcode2.html
```

---

### Option 3 : Netlify (Gratuit, Open-source)

1. Allez sur [netlify.com](https://netlify.com)
2. Connectez-vous avec GitHub
3. Faites **Drag and drop** du dossier `QRCode` complet
4. C'est déployé immédiatement !
5. Renommez le site si souhaité

---

### Option 4 : Vercel (Gratuit)

```bash
# Installez Vercel
npm i -g vercel

# Déployez
cd QRCode
vercel --prod
```

Suivez les instructions à l'écran.

---

## Fichiers du projet

| Fichier | Description |
|---------|-------------|
| qrcode2.html | Application principale |
| logo.png | Logo (format recommandé) |
| logo.jpg | Logo (alternative) |
| serve.command | Script de lancement local |
| README.md | Documentation |
| LICENCE | Licence du projet |

## Navigateurs supportés

- Chrome (dernière version)
- Firefox (dernière version)
- Safari (dernière version)
- Edge (dernière version)

---

## Licence

MIT License

Copyright (c) 2026 dataswca

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
