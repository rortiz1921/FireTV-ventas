# Fire TV Ventas — Firebase + Vercel

Este proyecto ya está configurado para el proyecto Firebase `firetv-782bd`.

## Subir a GitHub
1. Crea un repositorio nuevo en GitHub.
2. Sube estos archivos: `index.html` y `firebase-config.js`.
3. No cambies los nombres.

## Publicar en Vercel
1. Entra a Vercel y pulsa Add New Project.
2. Importa el repositorio de GitHub.
3. Pulsa Deploy.
4. No necesitas Build Command.

## Firebase
La aplicación usa Authentication (correo/contraseña) y Cloud Firestore.
Las reglas recomendadas son las que protegen `users/{uid}/...` para que cada usuario solo acceda a sus propios datos.

## Importante
El archivo `firebase-config.js` contiene configuración pública de una app web de Firebase; no es una clave privada de servidor. Nunca subas claves de cuentas de servicio (`serviceAccountKey.json`) al repositorio.
