# Boddies that Feel · Academia IA de Danza Colombiana

Aplicación web interactiva para aprender danza folclórica colombiana con IA.

## 🔥 Firebase
- Proyecto: `danza-dta`
- Base de datos: Firestore
- Documento sincronizado: `playlists/1779524179193`

## 📁 Archivos
- `index.html` — App completa (HTML + CSS + JS en un solo archivo)

## 🚀 Subir a GitHub Pages
1. Sube este repositorio a GitHub
2. Ve a Settings → Pages → Source: `main` branch, carpeta `/root`
3. Tu app estará en: `https://tuusuario.github.io/danza-dta/`

## ⚠️ Reglas de Firestore (desarrollo)
En Firebase Console → Firestore → Reglas:
```
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /playlists/{id} {
      allow read, write: if true;
    }
  }
}
```
