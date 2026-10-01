# ⚽ Reservas Canchas — Sistema web (Firebase)

Proyecto: `reservas-canchas-2026` | Demo: https://reservas-canchas-2026.web.app

## Requisitos
- Node.js 20+ y `npm i -g firebase-tools`
- Cuenta Google con acceso al proyecto Firebase

## Instalación y despliegue
```bat
cd reservas-canchas
firebase login
firebase use reservas-canchas-2026
firebase deploy --only firestore:rules,hosting
```

## Cuentas de prueba
- Dueño: login con tu correo aprobado (rol `dueno`)
- Registro: `/registro.html` (cliente/encargado/dueño, el dueño aprueba)

## Estructura
- `public/index.html` → catálogo + reserva + panel
- `public/catalogo.html` → solo clientes (sin login)
- `public/login.html`, `public/registro.html`
- `firestore.rules` → roles y permisos
- `firebase.json`, `.firebaserc`

## Git (dúo)
```bat
git init
git add .
git commit -m "Sistema reservas canchas v1"
git branch -M main
git remote add origin URL_DEL_REPO
git push -u origin main
```
Cada integrante trabaja en su rama y hace Pull Request para que el historial muestre a ambos.
