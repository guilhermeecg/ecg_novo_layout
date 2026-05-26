# ECG Sistemas — Redesign de Landing Page

> Proposta de novo layout para o site institucional da **ECG Sistemas**, empresa catarinense com 16+ anos no mercado de software para vidraçarias, esquadrias de alumínio e indústrias de têmpera.

**[Ver demo ao vivo →](https://amazingbits.github.io/ecg_novo_layout/)**

---

## Sobre o projeto

A ECG Sistemas é referência no setor vidreiro brasileiro, com mais de **4.000 usuários ativos**, **241 cidades atendidas** e múltiplos prêmios do Jornal do Vidro. O objetivo deste redesign foi modernizar a presença digital da empresa com uma landing page de alto impacto, mantendo a credibilidade e identidade consolidada da marca.

### Problema

O site anterior não comunicava adequadamente o posicionamento premium da empresa nem destacava os diferenciais competitivos dos dois principais produtos: **ECG Glass** e **ECG Temper**. A experiência mobile era deficiente e não havia elementos visuais modernos que transmitissem inovação tecnológica.

### Solução

Landing page completamente nova, desenvolvida com HTML, CSS e JavaScript puros (zero dependências de framework), otimizada para conversão e com atenção a cada detalhe de UX.

---

## Destaques técnicos

### Modelo 3D interativo
O hero da página apresenta o logotipo da ECG em **3D interativo**, renderizado diretamente no browser com a Web Component `<model-viewer>` do Google. O usuário pode rotacionar o modelo com touch/mouse.

Dois modelos disponíveis, alteráveis via query string:

| Parâmetro URL | Modelo carregado |
|---|---|
| `?vidro=glass` (padrão) | `modelo_ecg_vidro.glb` — versão translúcida |
| `?vidro=normal` | `modelo_ecg.glb` — versão opaca |


### Performance e SEO
- **Zero frameworks** — HTML/CSS/JS puros, carregamento instantâneo
- Fontes carregadas com `preconnect` + `display=swap`
- Schema.org estruturado (Organization + FAQPage) para rich results no Google
- Open Graph completo para compartilhamento em redes sociais
- Meta tags de SEO semântico com keywords do setor

### Design system
- CSS custom properties para consistência total de tokens (cores, sombras, raios, transições)
- Paleta azul institucional (`#05377B`) com accent em sky blue
- Tipografia: **Plus Jakarta Sans** (títulos) + **Inter** (corpo)
- Glassmorphism sutil em cards e elementos flutuantes

### Animações e interações
- Contador animado de números (scroll-triggered com `IntersectionObserver`)
- Scroll reveal progressivo em todas as seções
- Carrossel de depoimentos com snap scrolling e navegação por teclado
- Mapa interativo do Brasil com destaque dos estados atendidos
- Menu mobile com animação de hambúrguer → ✕
- Modelo 3D com loading state personalizado (spinner circular)

### Seções da página

| Seção | Descrição |
|---|---|
| **Hero** | Título principal, CTA duplo, modelo 3D, prova social |
| **Números** | Contadores animados com vídeo de fundo sutil |
| **Produtos** | Tabs ECG Glass / ECG Temper com feature lists |
| **Diferenciais** | Grid de funcionalidades com ícones |
| **Prêmios** | Newswall estilo jornal com coberturas do Jornal do Vidro |
| **Depoimentos** | Carrossel de clientes reais com avatares |
| **Cobertura** | Mapa SVG do Brasil com estados atendidos |
| **FAQ** | Accordion com perguntas frequentes + Schema.org |
| **CTA final** | Chamada para teste grátis de 10 dias |
| **Rodapé** | Grid com navegação, soluções, contato e redes sociais |

---

## Stack

```
HTML5 · CSS3 (custom properties, grid, flexbox, animations)
JavaScript ES6+ (vanilla, sem frameworks)
@google/model-viewer (Web Component para 3D)
Google Fonts (Inter + Plus Jakarta Sans)
```

---

## Como rodar localmente

Abra via algum servidor local válido, como o Live Server no VSCode.

---

## Sobre o autor

Desenvolvido por **Guilherme Andrade** como proposta de redesign para a ECG Sistemas.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/devguiandrade/)
