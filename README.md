# Fire TV Ventas — Firebase + Vercel

## 1. Firebase
- Crea/elige tu proyecto.
- Activa Authentication > Sign-in method > Email/Password.
- Crea Firestore Database.
- Agrega una Web App y copia su firebaseConfig.
- Copia `firebase-config.example.js` como `firebase-config.js` y pega los valores.

## 2. GitHub
Sube `index.html` y `firebase-config.js` al repositorio.

## 3. Vercel
Importa el repositorio desde Vercel y pulsa Deploy. No hace falta build command.

## 4. Seguridad
Antes de usar datos reales, configura reglas de Firestore para que cada usuario solo pueda leer/escribir `users/{uid}/...` cuando `request.auth.uid == uid`.

La app usa Firebase Authentication + Firestore y conserva la copia local como respaldo.
