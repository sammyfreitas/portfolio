# Portfólio — Anthony Freitas

Nova versão unificada do portfólio, construída a partir de `portfolio-v2` e `portfolioSite`.

## Versão 4.1

Ao abrir o site, confira o selo **VERSÃO 4.1** no início da página. Se aparecer “4 frentes” em vez de “9 frentes”, você está visualizando uma compilação antiga.

- tema escuro como padrão inicial e tema claro em azul;
- ícones reais para redes sociais e categorias;
- projetos com capturas das páginas, plataforma, tecnologias, demo e repositório;
- selo da Vitrine de Projetos para o Prêmio LED 2027;
- métricas de trajetória e medidores para front-end, back-end, dados, jogos, infraestrutura e educação;
- duas linhas do tempo: trajetória profissional/projetos e formação acadêmica;
- cards profissionais separados para CarrierWeb e FleetDesk;
- carrossel curado de projetos, área de jogos e espaço reservado para o Campus Mobile;
- seção de escrita e publicações, incluindo Rio de Letras 2027;
- foto carregada do perfil do GitHub para acompanhar futuras atualizações.
- cards com bordas arredondadas;
- catálogos navegáveis para Front-end, Back-end, Dados, Jogos, Mobile, Integrações, Infraestrutura, Educação e Narrativas;
- painéis detalhados para a atuação na CarrierWeb e no FleetDesk;
- carrossel automático com setas e indicadores;
- catálogo autoral com 35 crônicas e links para o blog.

## Desenvolvimento

```bash
npm install
npm run dev
```

Para conferir a versão compilada:

```bash
npm run build
npm run preview
```

## Publicação

O workflow em `.github/workflows/deploy.yml` publica o projeto no GitHub Pages a cada envio para a branch `main`. Em **Settings → Pages**, selecione **GitHub Actions** como fonte.

## Curadoria e atualização

Os projetos são curados nos arrays `featured` e `moreProjects`, em `src/App.jsx`. Assim, exercícios simples usados em aula não aparecem automaticamente no portfólio. Para incluir um novo projeto, adicione a captura em `public/projects` e registre seus dados em um desses arrays.

Os catálogos por área e os textos autorais ficam em `src/content.js`.

### Classificação recomendada para novos repositórios

Use tópicos do GitHub e mantenha no README um pequeno bloco padronizado:

```md
<!-- portfolio
area: front-end
status: publicado
site: https://...
destaque: sim
-->
```

Áreas sugeridas: `front-end`, `back-end`, `dados`, `dashboard`, `jogos`, `mobile`, `integracoes`, `infraestrutura`, `educacao` e `narrativas`. Um script futuro poderá consultar a API do GitHub, ler esse bloco e atualizar o catálogo sem incluir exercícios que não devem aparecer no portfólio.
