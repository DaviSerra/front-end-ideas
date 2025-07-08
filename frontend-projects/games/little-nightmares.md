# Little Nightmares - Web Experience
**Next.js + TypeScript + Tailwind CSS**

"Welcome to a world of nightmares where childhood innocence meets terror"

## Ideias Principais

### Landing Page Interativa
- Atmosfera sombria com Framer Motion para animações ao scroll
- Seções: Personagens • História • Galeria • Trilha Sonora
- Paleta: Tons escuros com acentos amarelos e vermelhos
- Background paralax com efeitos de partículas usando Canvas API

### Galeria de Personagens
- Cards interativos: Six • Mono • The Janitor
- Hover effects com Framer Motion revelando informações secretas
- Animações inspiradas nos movimentos únicos do jogo
- Modais com React Portal para lore detalhado

### Timeline da História
- Cronologia visual dos eventos de Little Nightmares I & II
- Navegação horizontal com scroll cinematográfico
- useIntersectionObserver para animações de entrada
- Transições dramáticas entre seções

### Elementos Visuais
- Background: Efeito paralax com useScroll do Framer Motion
- Partículas: Sistema de partículas com useEffect e RAF
- Iluminação: Sombras dramáticas com Tailwind CSS
- Tipografia: Google Fonts (Creepster, Nosifer)

## Stack Tecnológico

| Tecnologia | Uso |
|------------|-----|
| Next.js | Pages Router |
| TypeScript | Tipagem estática |
| Tailwind CSS | Estilização utility-first |
| Framer Motion | Animações e transições |
| State management |

## Estrutura de Arquivos

```
src/
├── app/
│   ├── layout.tsx
│   ├── page.tsx
│   ├── personagens/[slug]/page.tsx
│   ├── historia/page.tsx
│   └── galeria/page.tsx
├── components/
│   ├── ui/ (Button, Card, Modal)
│   ├── layout/ (Header, Footer, Navigation)
│   ├── sections/ (Hero, Characters, Timeline)
│   └── effects/ (ParallaxBg, ParticleSystem, AudioPlayer)
├── lib/
│   ├── types.ts
│   ├── constants.ts
│   └── utils.ts
├── hooks/
│   ├── useScrollAnimation.ts
│   ├── useAudio.ts
│   └── useIntersectionObserver.ts
└── styles/globals.css
```

## Design System

### Paleta de Cores (Tailwind Config)
```javascript
colors: {
  'nightmare-black': '#1a1a1a',
  'shadow-gray': '#2d2d2d',
  'yellow-light': '#ffdb4d',
  'blood-red': '#8b0000',
}
```

### Tipografia
- Creepster/Nosifer para títulos principais
- Inter para textos de leitura
- Fontes carregadas via next/font

## Funcionalidades

### Interatividade
- Player de áudio customizado com Web Audio API
- Tema sombrio por padrão (useTheme hook)
- Animações de loading temáticas
- Efeitos sonoros nos hover/click com Howler.js

### Performance
- Imagens otimizadas com next/image
- Lazy loading para seções pesadas
- Code splitting por rotas
- Preload de assets críticos

## Roadmap

### Phase 1: Setup & Design
- Configuração Next.js + TypeScript
- Design System com Tailwind
- Protótipo das principais seções

### Phase 2: Desenvolvimento Core
- Componentes base e layout
- Sistema de roteamento
- Animações básicas com Framer Motion

### Phase 3: Interatividade
- Hooks customizados
- Sistema de áudio
- Micro-interações

### Phase 4: Polimento
- Responsive design
- Performance optimization
- SEO e acessibilidade

## Inspirações
- Site oficial do jogo
- Portfolios de desenvolvedores indie
- Interfaces de horror/thriller games
- Animações cinematográficas
