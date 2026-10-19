<div align="center">

# Aceslan · Android

### Página oficial de distribución del APK de Aceslan

**Web de descarga · Android · GitHub Pages · GitHub Releases**

![HTML5](https://img.shields.io/badge/HTML5-1A1B26?style=for-the-badge&logo=html5&logoColor=E46B79)
![CSS3](https://img.shields.io/badge/CSS3-1A1B26?style=for-the-badge&logo=css3&logoColor=E46B79)
![Android](https://img.shields.io/badge/Android-1A1B26?style=for-the-badge&logo=android&logoColor=E46B79)
![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-1A1B26?style=for-the-badge&logo=github&logoColor=E46B79)

[![Estado](https://img.shields.io/badge/ESTADO-Página_de_descarga-712B39?style=flat-square)](#estado-del-proyecto)
[![Versión](https://img.shields.io/badge/APK-v1.0.0-712B39?style=flat-square)](https://github.com/fmoorenoo/AceslanAndroid/releases/tag/v1.0.0)
[![Código](https://img.shields.io/badge/REPOSITORIO-Código_web-22252C?style=flat-square)](https://github.com/fmoorenoo/AceslanAndroid)

**[Descargar Aceslan.apk](https://github.com/fmoorenoo/AceslanAndroid/releases/download/v1.0.0/Aceslan.apk)** · **[Consultar la release v1.0.0](https://github.com/fmoorenoo/AceslanAndroid/releases/tag/v1.0.0)**

</div>

---

## Sobre el proyecto

**AceslanAndroid** es un sitio web estático diseñado para facilitar la **descarga e instalación de la aplicación Aceslan en dispositivos Android**.

La página reúne un enlace al archivo APK publicado mediante **GitHub Releases**, una guía visual de instalación y los logotipos del **Consorcio de Seguridad y Emergencias de Lanzarote** y del **Cabildo de Lanzarote**.

> **Alcance de este repositorio:** contiene la página de distribución y el enlace al APK, **no el código fuente de la aplicación Android**. Por ello, no se describen ni se atribuyen funcionalidades internas de la aplicación que no puedan verificarse aquí.

## Funcionalidades

- **Descarga del APK:** botón enlazado a una release publicada en GitHub.
- **Instrucciones de instalación:** explicación breve de los pasos para instalar el paquete en Android.
- **Diseño responsive:** composición adaptada a pantallas móviles.
- **Identidad institucional:** incorporación de los logotipos del Consorcio y del Cabildo.
- **Accesibilidad básica:** descripciones alternativas y etiquetas en los elementos principales de la página.
- **Pie de página dinámico:** actualización automática del año mediante JavaScript.
- **Acceso mediante QR:** preparada para utilizar un QR externo dirigido a la URL estable de la página.

## Tecnologías

| Área | Tecnologías |
| --- | --- |
| **Estructura** | HTML5 |
| **Diseño** | CSS3 · media queries |
| **Comportamiento** | JavaScript (año del pie de página) |
| **Distribución de la app** | APK para Android |
| **Alojamiento web previsto** | GitHub Pages |
| **Almacenamiento de versiones** | GitHub Releases |
| **Recursos** | Imágenes WebP |

## Arquitectura

```text
AceslanAndroid/
├── index.html            # Página de descarga e instalación
├── styles.css            # Diseño y adaptación a móviles
├── logo_consorcio.webp   # Identidad visual del Consorcio
├── logo_cabildo.webp     # Identidad visual del Cabildo
└── README.md             # Documentación de la distribución
```

La aplicación Android se distribuye como **asset de GitHub Releases**; no está incluida como código fuente en esta estructura.

## Descargar Aceslan

**Versión publicada verificada en GitHub Releases: `v1.0.0`**.

**[Descargar archivo Aceslan.apk →](https://github.com/fmoorenoo/AceslanAndroid/releases/download/v1.0.0/Aceslan.apk)**

### Instalación en Android

1. Accede a la página de descarga desde tu dispositivo Android.
2. Pulsa **Descargar app**.
3. Abre el archivo `Aceslan.apk` una vez completada la descarga.
4. Si Android lo solicita, autoriza temporalmente la instalación desde esa fuente.
5. Completa la instalación siguiendo las instrucciones del sistema.

**Seguridad:** instala únicamente paquetes de una fuente que consideres fiable. Comprueba el origen del APK antes de conceder permisos de instalación. No se ha auditado el binario Android ni sus permisos durante esta revisión.

## Logotipos incluidos

<div align="center">
  <img src="logo_consorcio.webp" alt="Logotipo del Consorcio de Seguridad y Emergencias de Lanzarote" height="75">
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="logo_cabildo.webp" alt="Logotipo del Cabildo de Lanzarote" height="75">
</div>

Se conservan los recursos visuales incluidos originalmente en la página.

## Actualización de versiones del APK

Cuando se publique una nueva versión de la aplicación:

1. Accede a **GitHub Releases** y crea o selecciona la release correspondiente.
2. Adjunta el nuevo archivo `.apk`.
3. Copia su enlace directo de descarga.
4. Abre `index.html` y actualiza el atributo `href` del enlace con clase `btn-download`.
5. Actualiza, si procede, la versión y el enlace de descarga documentados en este README.
6. Publica los cambios para que la página apunte a la nueva release.

> **Nota:** el README original indicaba un marcador `PENDIENTE_URL_RELEASE_APK`, pero el código actual ya contiene un enlace real a la versión `v1.0.0`. No es necesario reemplazar ningún marcador para esa versión.

## Código QR y GitHub Pages

Si se distribuye un QR mediante carteles o documentación impresa, debe apuntar a la **URL pública estable de la página**, por ejemplo:

```text
https://fmoorenoo.github.io/AceslanAndroid/
```

**No conviene dirigir el QR al enlace del APK**, porque ese enlace cambiará con cada nueva release. Al mantener la página como destino permanente, solo será necesario actualizar el botón de descarga cuando haya una versión nueva.

La ruta de GitHub Pages anterior corresponde al esquema habitual de publicación del repositorio. Su disponibilidad en producción no se ha verificado durante esta auditoría.

## Ejecución local

1. Clona el repositorio:

   ```bash
   git clone https://github.com/fmoorenoo/AceslanAndroid.git
   cd AceslanAndroid
   ```

2. Abre `index.html` directamente en un navegador o ejecuta un servidor HTTP local:

   ```bash
   python -m http.server 8000
   ```

3. Abre `http://localhost:8000/`.

No requiere instalar dependencias, compilar el frontend ni configurar un backend.

## Estado del proyecto

**Página estática de descarga con una release APK publicada.**

Durante la revisión se ha comprobado que la release `v1.0.0` existe en GitHub e incluye el archivo `Aceslan.apk`. **No se ha instalado ni inspeccionado el contenido del APK**, ni se ha verificado la ejecución real de la web en distintos dispositivos.

El proyecto es un canal de distribución web; su contenido no permite verificar las funcionalidades, permisos o arquitectura de la aplicación Android empaquetada.

## Autor

**Fernando Montelongo Moreno** · Full Stack Developer · DAM + DAW

[![GitHub](https://img.shields.io/badge/GitHub-fmoorenoo-22252C?style=flat-square&logo=github)](https://github.com/fmoorenoo)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Perfil_profesional-712B39?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/fernando-montelongo/)

---

<div align="center">
  <sub>Aceslan Android · Página web para la descarga y distribución de la aplicación</sub>
</div>
