# Test de Personalidad Definitivo™ ⚡ (Proyecto Date)

Una experiencia interactiva y narrativa *mobile-first*, diseñada con estética de terminal/videojuego y desenlace sorpresa.

---

## 📁 Estructura del Proyecto

```
project-date/
├── index.html          # Interfaz semántica y contenedores de las 8 fases
├── package.json        # Configuración y comandos estándar
├── render.yaml         # Configuración automática de despliegue en Render (Static Site)
├── .gitignore          # Archivos excluidos del control de versiones
├── css/
│   └── style.css       # Estilos responsive, diseño mobile-first y temas Cyber/Romantic
└── js/
    ├── config.js       # Configuración centralizada (nombres, preguntas, textos, URL)
    ├── sound.js        # Efectos de audio con Web Audio API (cero dependencias)
    ├── confetti.js     # Motor Canvas de confeti y corazones a 60fps
    └── app.js          # Controlador de flujo y lógica del botón NO esquivo
```

---

## 🚀 Cómo Subir el Proyecto a GitHub

Tienes dos opciones muy sencillas:

### Opción A: Directamente desde la web de GitHub (Sin instalar Git)
1. Entra en [github.com](https://github.com) e inicia sesión.
2. Pulsa en el botón verde **"New"** para crear un nuevo repositorio (por ejemplo, `test-personalidad` o `project-date`).
3. Elige el repositorio como **Public** o **Private** y dale a **"Create repository"**.
4. En la pantalla que aparece, haz clic en el enlace azul **"uploading an existing file"** (subir archivos existentes).
5. Arrastra todos los archivos y carpetas de esta carpeta (`index.html`, `package.json`, `render.yaml`, `.gitignore`, `README.md`, carpeta `css`, carpeta `js`).
6. Pulsa en el botón verde **"Commit changes"**. ¡Listo!

---

### Opción B: Si tienes Git o GitHub Desktop instalado
Abre una terminal en la carpeta del proyecto y ejecuta:

```bash
git init
git add .
git commit -m "Initial commit: Proyecto Date completo"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/TU_REPOSITORIO.git
git push -u origin main
```

---

## 🌐 Cómo Desplegar en Render (onrender.com) Gratis

Render ofrece alojamiento de **Static Sites** 100% gratuito, con certificado SSL (HTTPS) automático y URL pública (ejemplo: `https://test-personalidad.onrender.com`).

### Pasos en Render:
1. Entra en [render.com](https://render.com) e inicia sesión (puedes entrar directamente con tu cuenta de GitHub).
2. En el panel principal (Dashboard), haz clic en el botón azul **"New +"** (arriba a la derecha) y selecciona **"Static Site"**.
3. Conecta tu cuenta de GitHub y selecciona el repositorio que acabas de subir.
4. Completa los siguientes campos (son muy sencillos):
   - **Name**: El nombre que quieras para la URL (por ejemplo: `mision-secreta` o `test-personalidad`).
   - **Branch**: `main`
   - **Build Command**: *(Dejar en blanco o poner `echo 'Listo'`)*
   - **Publish Directory**: `./` *(un punto y una barra, o simplemente un punto `.`)*
5. Haz clic en el botón inferior **"Create Static Site"**.

¡En menos de 1 minuto tendrás tu enlace público de `https://tu-proyecto.onrender.com` listo para enviárselo a quien tú quieras!

---

## ⚙️ Personalización Rápida

Todos los textos, preguntas y nombres están centralizados en `js/config.js`:
- Cambiar el nombre del remitente o de la invitada: `CONFIG.couple.recipientName` / `CONFIG.couple.senderName`
- Cambiar las preguntas o respuestas: `CONFIG.questions`
- Cambiar el enlace de Twitch o apartado oculto: `CONFIG.successScreen.secretSectionUrl`
