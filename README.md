# Bravex Systems — sitio web

Sitio oficial de **Bravex Systems**: desarrollo de software, paneles de gestión y automatización operativa. Fundador: Braulio Veron · WhatsApp +54 9 3757 67-1229.

## Estructura

- `index.html` — sitio completo (HTML + Tailwind CSS vía CDN + JS vanilla). Se abre directo en el navegador.
- `Dockerfile` — imagen nginx para servirlo en un VPS (Easypanel / Hostinger).

## Desplegar

```bash
docker build -t bravex-web .
docker run -d -p 80:80 bravex-web
```

En Easypanel: crear App desde este repo → build por Dockerfile → puerto 80.
