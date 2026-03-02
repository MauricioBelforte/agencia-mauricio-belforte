
# 🔥 Guía Maestra: Configuración Firebase Hosting + GitHub Actions (2026)

Esta guía detalla los pasos exactos desde la limpieza de sesión hasta el despliegue automático.

## 1. Limpieza y Actualización (Opcional pero Recomendado)
Si tienes errores de permisos o versiones viejas, empieza aquí:

```bash
# Actualizar las herramientas de Firebase
npm install -g firebase-tools

# Cerrar sesión y volver a entrar para refrescar tokens
firebase logout
firebase login

```

> **Nota:** En el login, si pregunta por **Gemini**, elige `Y` (Sí). Si pregunta por **Usage Reporting**, elige `n` (No) para ahorrar recursos.

---

## 2. Inicialización del Proyecto

Ubícate en la carpeta raíz de tu proyecto en la terminal (VS Code preferiblemente) y ejecuta:

```bash
firebase init hosting

```

### 📋 Respuestas del Asistente (Paso a Paso):

1. **¿Are you ready to proceed?**
* Respuesta: `Yes`


2. **¿Please select an option?**
* Respuesta: `Use an existing project` (Selecciona tu proyecto de la lista).


3. **¿What do you want to use as your public directory?**
* Si es HTML puro: `public` (Presiona un punto .).
* Si es React/Vite: `dist` (Escribe `dist` y Enter).


4. **¿Configure as a single-page app (rewrite all urls to /index.html)?**
* Si es React/Vite/Angular: `Y` (Yes).
* Si es HTML con varias páginas (.html): `n` (No).


5. **¿Set up automatic builds and deploys with GitHub?**
* Respuesta: `Y` (Yes). **(ESTE ES EL PASO CLAVE)**.



---

## 3. Conexión con GitHub

Tras decir que sí a GitHub, se abrirá el navegador para autorizar. Luego vuelve a la terminal:

1. **¿For which GitHub repository...?**
* Formato: `usuario/nombre-del-repo` (Ej: `mauricio-belforte/mi-portfolio`).


2. **¿Set up the workflow to run a build script before every deploy?**
* Si es HTML puro: `n` (No).
* Si es React/Vite: `y` (Yes). (Comando: `npm ci && npm run build`).


3. **¿Set up automatic deployment to your site's live channel when a PR is merged?**
* Respuesta: `y` (Yes).


4. **¿What is the name of the GitHub branch... (main)?**
* Respuesta: Presiona **Enter** para aceptar `main`.

5. **File ./index.html already exists. Overwrite?**
* Respuesta: `n` (No) para no perder tu contenido. Si pones `y` (Yes), se reemplazará con un template vacío.
---

## 4. El "Vuelo Inicial" (Subir los archivos)

Firebase creó archivos nuevos (`firebase.json`, `.firebaserc` y la carpeta `.github`). Tienes que mandarlos a GitHub para activar el "robot":

```bash
# Agregar todos los archivos nuevos
git add .

# Crear el mensaje de guardado
git commit -m "Configuración Firebase + GitHub Actions finalizada"

# Subir a la nube
git push origin main

```

---

## 5. ¿Cómo saber si funcionó?

1. Ve a tu repositorio en **GitHub.com**.
2. Haz clic en la pestaña **"Actions"**.
3. Verás un proceso llamado "Deploy to Firebase Hosting".
* 🟡 **Amarillo:** Está trabajando.
* ✅ **Verde:** ¡Tu web ya está en vivo!
* ❌ **Rojo:** Algo falló (revisar el log ahí mismo).



---

## 💡 Tips de Oro:

* **Archivos que SIEMPRE se suben:** `firebase.json` y `.firebaserc`. Sin ellos, GitHub no sabe dónde publicar.
* **Reciclar Proyectos:** Si te quedas sin cupo en el Plan Spark, no borres proyectos (tardan 30 días en liberar cupo). Mejor borra el contenido de uno viejo y reutilízalo para el nuevo.

```


```