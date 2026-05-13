# Aceslan — Página de descarga

Esta web estática sirve como página de descarga de la aplicación **Aceslan** para Android.
Está pensada para publicarse en **GitHub Pages** y puede acompañarse de un código QR que apunte a dicha URL.

---

## Cómo actualizar la URL del APK

Cuando publiques una nueva release en GitHub:

1. Ve a la release en GitHub y copia la URL directa al archivo `.apk`.
2. Abre `index.html` y busca la línea:

   ```html
   <!-- Sustituye PENDIENTE_URL_RELEASE_APK por la URL del APK publicada en GitHub Releases -->
   <a ... href="PENDIENTE_URL_RELEASE_APK" ...>
   ```

3. Reemplaza `PENDIENTE_URL_RELEASE_APK` con la URL copiada. Por ejemplo:

   ```
   https://github.com/TU_USUARIO/TU_REPO/releases/download/v1.0.0/aceslan.apk
   ```

4. Haz commit y push. GitHub Pages se actualizará automáticamente.

---

## Código QR

El QR debe apuntar a la **URL pública de la página en GitHub Pages**
(p. ej. `https://TU_USUARIO.github.io/TU_REPO/`),
**no** directamente a la URL del APK.

De esta forma, si en el futuro cambias la URL del APK o añades más información,
el QR ya impreso o distribuido seguirá siendo válido.

---

## Archivos

| Archivo               | Descripción                              |
|-----------------------|------------------------------------------|
| `index.html`          | Página principal de descarga             |
| `styles.css`          | Estilos de la página                     |
| `logo_consorcio.webp` | Logotipo del Consorcio                   |
| `logo_cabildo.webp`   | Logotipo del Cabildo                     |
