# FOCUS. — Lista de espera

Landing independiente de la app FOCUS. para captar interesados antes del
lanzamiento. Una sola página (`index.html`), sin build ni dependencias locales:

- Escena 3D con Three.js (CDN): cámara compacta estilo G7X con órbita tipo
  dron que acaba mirando por el objetivo, y transición de enfoque al formulario.
- El formulario guarda nombre + email en Firestore del proyecto
  `focus-app-2746d`, colección `waitlist/{email}` (el email como ID evita
  duplicados). Las Security Rules de esa colección viven en el repo de la app
  (`firestore.rules`) y se publican en la consola de Firebase.
- Los apuntados se consultan en la consola de Firebase → Firestore → `waitlist`.

Deploy: GitHub Pages (Settings → Pages → Deploy from branch → main, carpeta `/`).
