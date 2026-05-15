# Publicacao segura da landing

Este repositorio/pasta e somente da landing page do Flux Studio AI.

Regra principal:

- Nao editar o app principal `fluxstudio-app` sem autorizacao explicita.
- Nao mexer em Mercado Pago, creditos, login, geracao, banco ou Render do app.
- A landing deve apenas apontar o botao "Entrar no App" para `https://fluxstudio-app.onrender.com`.

## Estrutura recomendada

- Codigo da landing no GitHub: `Carlospeixoto238/fluxstudio-landing`
- Site estatico no Render: novo Static Site separado
- Videos no R2/CDN: `https://media.fluxstudioai.com.br/landing/...`

## Videos esperados no R2

Subir estes arquivos na pasta `landing/` do bucket publico:

- `hero-flux-studio.mp4`
- `apresentacao-rapida.mp4`
- `fluxstudio-4-completo.mp4`
- `modelo-1.mp4`
- `modelo-2.mp4`
- `modelo-3.mp4`

URLs que a landing usa:

- `https://media.fluxstudioai.com.br/landing/hero-flux-studio.mp4`
- `https://media.fluxstudioai.com.br/landing/apresentacao-rapida.mp4`
- `https://media.fluxstudioai.com.br/landing/fluxstudio-4-completo.mp4`
- `https://media.fluxstudioai.com.br/landing/modelo-1.mp4`
- `https://media.fluxstudioai.com.br/landing/modelo-2.mp4`
- `https://media.fluxstudioai.com.br/landing/modelo-3.mp4`

## Render

Criar um novo Static Site separado do app:

- Repositorio: `Carlospeixoto238/fluxstudio-landing`
- Branch: `main`
- Build command: deixar vazio
- Publish directory: `.`

Nao conectar este static site ao repositorio `fluxstudio-app`.
