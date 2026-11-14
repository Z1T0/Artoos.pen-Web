# Artools · Pigmentum

Landing page de produto para a caneta **Artools Pigmentum**, com animação de vídeo controlada pelo scroll.

## Destaques

- **Hero com scroll-scrubbing**: os frames do vídeo são extraídos para um `<canvas>` e avançam conforme a rolagem (GSAP + ScrollTrigger), evitando os travamentos de buscar `video.currentTime` a cada evento.
- **Seções com animação de entrada** e vídeo em loop na seção de fluxo.
- **Design system** documentado em `design_system.html` (cores, tipografia, componentes).
- Página estática: sem build, sem dependências locais.

## Estrutura

```
.
├── index.html            # Landing page
├── design_system.html    # Guia de estilo / design system
└── assets/
    ├── video/            # hero.mp4 (scroll do hero) · flow.mp4 (seção de fluxo)
    └── ds/               # Fontes (Inter) e imagens do design system
```

## Como rodar

Abra `index.html` direto no navegador ou sirva a pasta localmente (recomendado, por causa dos vídeos):

```bash
npx serve .
# ou
python -m http.server 8000
```

## Tecnologias

HTML · Tailwind CSS (CDN) · GSAP + ScrollTrigger · Iconify
