# CLAUDE.md — DECORANDOCOMCLASSESHOP

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** DECORANDOCOMCLASSESHOP
**Nicho:** Casa e Decoração
**Keywords:** Ola somos o maior comercio eletronico de decoracao da regiao sul do
**Paleta de cores:** sunset | **Fonte:** playfair

Olá, somos o maior comércio eletrônico de decoração da região sul do Brasil. Nossa empresa está no mercado há mais de 10 anos e nos orgulhamos de nossa ampla seleção de produtos de alta qualidade e atendimento ao cliente que é inigualável. Nossa equipe se dedica a trazer a você a melhor experiência de compra possível, portanto, não hesite em nos contatar se você tiver alguma dúvida ou comentário. Obrigado por escolher nossa loja!



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-C |
| Hero | Hero-H |
| Features | Features-H |
| About Section | About-B |
| Posts | Posts-J |
| Footer | Footer-F |
| Página Sobre | Sobre-G |
| Página Contato | Contato-B |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
