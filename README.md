# Foto de carnet

App web para hacer fotos de carnet con el móvil: cámara selfie o trasera, guías de encuadre y descarga de la foto suelta o de una hoja 10×15 cm con varias copias lista para imprimir.

Todo se procesa en el navegador; las fotos no se suben a ningún servidor.

## Funciones

- **Cámara en directo** (frontal o trasera) con guía de encuadre y temporizador de 3 s. Si el navegador no da acceso, usa la cámara nativa del móvil.
- **Galería**: también puedes partir de una foto que ya tengas.
- **Tamaños**: España (DNI, NIE, pasaporte · 26×32 mm), UE/Schengen y Reino Unido (35×45), EE. UU. (2×2 in), Canadá (50×70), China (33×48) y medida libre.
- **Ajustes**: mover, zoom (también con pellizco), inclinación, espejo, brillo y contraste.
- **Exportación** a 300 ppp en JPG: foto individual u hoja 10×15 cm con líneas de corte.

## Publicar con GitHub Pages

1. Crea un repositorio nuevo en GitHub y sube el contenido de esta carpeta (o `git push`).
2. En el repositorio: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, rama `main`, carpeta `/ (root)`.
3. En un minuto estará en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

La cámara en directo necesita HTTPS, que GitHub Pages ya da. Desde el móvil puedes usar «Añadir a pantalla de inicio» para tenerla como app.

```bash
git init
git add .
git commit -m "Foto de carnet"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/foto-carnet.git
git push -u origin main
```

## Probar en local

```bash
python3 -m http.server 8000
```

Abre `http://localhost:8000`. En `localhost` la cámara también funciona.

## Aviso

Las medidas son las habituales de cada documento. Comprueba los requisitos actuales del organismo que pide la foto (fondo, expresión, gafas, etc.).

## Licencia

MIT
