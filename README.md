# ContaBeto Landing Page

Landing page para contabeto.zxy.vc

## Archivos

- `index.html` — Landing page principal (single-file, no dependencies)

## Características

- ✅ Mobile-first responsive design
- ✅ WhatsApp CTA integrado (+52 477 337 4008)
- ✅ Planes de precios ($299, $599, $999)
- ✅ FAQ section
- ✅ Sin dependencias externas (excepto Google Fonts)
- ✅ SEO básico con Open Graph tags

## Deployment Options

### Opción 1: GitHub Pages (Recomendado)
```bash
# Crear repo y subir
cd ~/.openclaw/workspace/proyectos/contabeto/landing
git init
git add .
git commit -m "Initial landing page"
gh repo create zxy-ventures/contabeto-landing --public
git push -u origin main

# Configurar custom domain en GitHub Pages settings
# Agregar CNAME: contabeto.zxy.vc
```

### Opción 2: Cloudflare Pages
1. Subir a GitHub/GitLab
2. Conectar con Cloudflare Pages
3. Configurar custom domain

### Opción 3: Vercel
```bash
npm i -g vercel
vercel --prod
# Configurar custom domain en dashboard
```

### Opción 4: Hosting directo
Subir `index.html` a cualquier servidor web estático.

## DNS (GoDaddy)

El CNAME `contabeto` ya está configurado apuntando a `zxy.vc`.
Para usar con GitHub Pages, cambiar a:
```
contabeto CNAME <username>.github.io
```

## Personalización

### Cambiar número de WhatsApp
Buscar y reemplazar `524773374008` con el nuevo número.

### Cambiar colores
Modificar variables CSS en `:root`:
```css
--primary: #25D366;      /* Verde WhatsApp */
--primary-dark: #128C7E;
--dark: #1a1a2e;
```

### Agregar analytics
Agregar antes de `</head>`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXX"></script>
```

## TODO

- [ ] Agregar logo/imagen de Beto
- [ ] Agregar testimoniales cuando tengamos clientes
- [ ] Agregar video demo
- [ ] Configurar Google Analytics
- [ ] Agregar schema.org markup para SEO
