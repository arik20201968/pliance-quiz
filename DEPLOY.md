# 🚀 Guía de Despliegue

## GitHub Pages

Para desplegar este quiz en GitHub Pages:

### 1. Subir a GitHub
```bash
git remote add origin https://github.com/TU_USUARIO/TU_REPOSITORIO.git
git push -u origin main
```

### 2. Activar GitHub Pages
1. Ve a tu repositorio en GitHub
2. Haz clic en **Settings** (Configuración)
3. Scroll hacia abajo hasta **Pages**
4. En **Source**, selecciona **Deploy from a branch**
5. Selecciona la rama **main** y carpeta **/ (root)**
6. Haz clic en **Save**

### 3. Acceder al sitio
Tu quiz estará disponible en:
```
https://TU_USUARIO.github.io/TU_REPOSITORIO/pliance.html
```

## Otros Servicios de Hosting

### Netlify
1. Arrastra la carpeta del proyecto a [netlify.com/drop](https://app.netlify.com/drop)
2. Tu sitio estará disponible inmediatamente

### Vercel
1. Conecta tu repositorio de GitHub en [vercel.com](https://vercel.com)
2. El despliegue será automático

### Surge.sh
```bash
npm install -g surge
surge
```

## Configuración Personalizada

### Dominio Personalizado (GitHub Pages)
1. Crea un archivo `CNAME` en la raíz del proyecto
2. Agrega tu dominio personalizado
3. Configura los DNS de tu dominio

### HTTPS
GitHub Pages incluye HTTPS automáticamente. Para otros servicios, asegúrate de activar SSL/TLS.

## Optimizaciones para Producción

### Minificación (Opcional)
Si quieres optimizar el archivo para producción:

1. **CSS**: Usa herramientas como `cssnano`
2. **JavaScript**: Usa herramientas como `terser`
3. **HTML**: Usa herramientas como `html-minifier`

### CDN (Opcional)
Para mejor rendimiento global, considera usar un CDN como:
- Cloudflare
- AWS CloudFront
- Google Cloud CDN

## Monitoreo

### Google Analytics (Opcional)
Agrega este código antes del `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_TRACKING_ID');
</script>
```

### Uptime Monitoring
Servicios recomendados:
- UptimeRobot (gratuito)
- Pingdom
- StatusCake

---

¡Tu quiz estará disponible 24/7 para estudiantes de todo el mundo! 🌍