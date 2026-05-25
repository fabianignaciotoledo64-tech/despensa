# 🛒 Despensa — App de compras del hogar

App PWA para gestionar el stock de casa y generar la lista de compras.
Se instala en el celular y la notebook sin App Store ni Play Store.

---

## 📲 INSTALACIÓN

### Opción A — GitHub Pages (RECOMENDADA, gratis y con sincronización)

1. Creá una cuenta en https://github.com si no tenés
2. Creá un repositorio nuevo llamado `despensa` (público)
3. Subí todos estos archivos al repositorio:
   - index.html
   - manifest.json
   - sw.js
   - icons/icon-192.png
   - icons/icon-512.png
4. Andá a Settings → Pages → Source: "main branch" → Save
5. Tu app va a estar en: https://TU_USUARIO.github.io/despensa/
6. Abrí esa URL desde el celular y la notebook

**Para instalar en Android:**
- Abrí Chrome → tocá los 3 puntitos → "Agregar a pantalla de inicio"

**Para instalar en iPhone:**
- Abrí Safari → tocá el botón compartir (□↑) → "Agregar a pantalla de inicio"

**Para instalar en notebook (Chrome/Edge):**
- Abrí la URL → aparece un ícono de instalar en la barra de direcciones → hacé clic

---

### Opción B — Servidor local en la notebook

Si tenés Python instalado:
```bash
cd despensa-pwa
python3 -m http.server 8080
```
Luego abrí: http://localhost:8080

Para que el celular acceda, reemplazá localhost por la IP local de tu notebook
(ej: http://192.168.1.100:8080)

---

### Opción C — VS Code con Live Server

Instalá la extensión "Live Server" en VS Code,
abrí la carpeta y hacé clic en "Go Live".

---

## 🔄 SINCRONIZACIÓN

En la versión PWA instalada, los datos se guardan **localmente en cada dispositivo**
con localStorage. Para sincronización real entre vos y tu esposa, la opción es
usar GitHub Pages (ambos acceden a la misma URL) — los datos se guardan en
el propio dispositivo pero la app es la misma.

Para sincronización en tiempo real entre dispositivos, podés usar la versión
en Claude.ai que usa storage compartido.

---

## 📁 Archivos incluidos

- `index.html` — App completa (91 productos cargados)
- `manifest.json` — Configuración PWA
- `sw.js` — Service Worker (funciona offline)
- `icons/` — Íconos de la app
- `README.md` — Este archivo
