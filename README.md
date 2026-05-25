# Kegel Workbook — Semana 2
## @fisio.aliciaquinones

Esta es una Progressive Web App (PWA) lista para:

---

## 🌐 Opción 1: Web (para agregar al escritorio del iPhone)

### Deploy con Netlify (gratis, 5 minutos):
1. Ve a https://netlify.com y crea cuenta gratuita
2. Arrastra la carpeta `kegel-workbook/` completa al panel de Netlify
3. Netlify genera automáticamente una URL tipo: `https://kegel-semana2.netlify.app`
4. En el iPhone, abre Safari → ve a esa URL → botón "Compartir" → "Agregar a pantalla de inicio"
5. ¡Aparece como app nativa con ícono propio!

### Deploy con Vercel (también gratis):
1. Ve a https://vercel.com
2. "Add New Project" → arrastra la carpeta
3. Misma experiencia

### Deploy con GitHub Pages:
1. Sube los archivos a un repositorio en GitHub
2. Settings → Pages → Source: main branch
3. URL: `https://tu-usuario.github.io/kegel-workbook`

---

## 📱 Opción 2: App Store (iOS nativo)

Para publicar en el App Store se necesita:

### Con React Native / Expo (recomendado para simplificar):
1. Instalar Expo: `npm install -g expo-cli`
2. `expo init kegel-app`
3. Copiar la lógica de ejercicios al componente React Native
4. `expo build:ios`
5. Subir a App Store Connect con cuenta Developer ($99/año)

### Con Capacitor (wrapping de esta WebApp):
1. `npm install @capacitor/core @capacitor/cli @capacitor/ios`
2. `npx cap init "Kegel Workbook" "com.fisioaliciaquinones.kegel"`
3. Copiar archivos HTML/JS/CSS al folder `www/`
4. `npx cap add ios`
5. `npx cap open ios` → Xcode → Archive → App Store

---

## 📂 Archivos incluidos:
- `index.html` — App completa (HTML + CSS + JS)
- `manifest.json` — Configuración PWA (ícono, nombre, colores)
- `sw.js` — Service Worker (modo offline)
- `icon-192.png` — Ícono para Android / navegadores
- `icon-512.png` — Ícono grande
- `README.md` — Este archivo

---

## ✨ Funcionalidades de la app:
- 4 ejercicios de la Semana 2 con guía visual
- Temporizador circular interactivo por fase
- Contador de repeticiones con puntos animados
- Gráfica de patrón de contracción para cada ejercicio
- Funciona offline (Service Worker)
- Diseño optimizado para iPhone (safe areas, tipografía elegante)

---

**Diseñado con amor por Claude para @fisio.aliciaquinones** 🌸
