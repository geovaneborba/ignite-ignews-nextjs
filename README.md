<img width="1920" height="1080" alt="Ignews" src="https://github.com/user-attachments/assets/eeb14c77-eabf-477f-b12b-ef5c2ed070fc" />

<p align="center">
  <img alt="Repo size"  src="https://img.shields.io/github/repo-size/geovaneborba/ignite-ignews-nextjs?color=4f46e5&style=for-the-badge">
  <img alt="GitHub top language"  src="https://img.shields.io/github/languages/top/geovaneborba/ignite-ignews-nextjs?color=4f46e5&style=for-the-badge">
  <img alt="GitHub language count"  src="https://img.shields.io/github/languages/count/geovaneborba/ignite-ignews-nextjs?color=4f46e5&style=for-the-badge">
</p>

<p align="center">
  <a href="#dart-sobre">Sobre</a> &#xa0; | &#xa0;
  <a href="#books-aprendizado">Aprendizado</a> &#xa0; | &#xa0;
  <a href="#rocket-tecnologias">Tecnologias</a> &#xa0; | &#xa0;
  <a href="#warning-pré-requisitos"> Pré requisitos</a> &#xa0; | &#xa0;
  <a href="#checkered_flag-começando">Começando</a> &#xa0;
</p>

<br>

## :dart: Sobre

O **ig.news** é um blog de notícias sobre o mundo da programação com **conteúdo por assinatura**, desenvolvido durante o programa Ignite da Rocketseat. O conteúdo dos posts é gerenciado através de um CMS headless (Prismic), a autenticação é feita via OAuth com NextAuth.js, e o acesso ao conteúdo exclusivo é liberado somente para usuários com assinatura ativa, processada via Stripe.

<p align="right">(<a href="#top">Voltar para o topo</a>)</p>

## :books: Aprendizado

- Autenticação com OAuth utilizando NextAuth.js
- Gerenciamento de conteúdo com CMS headless (Prismic)
- Processamento de pagamentos recorrentes (assinaturas) com Stripe
- Webhooks do Stripe para sincronizar status de assinatura
- Server-side Rendering (SSR) e geração de páginas protegidas por assinatura no Next.js
- Persistência de dados de usuários/assinaturas com MongoDB

<p align="right">(<a href="#top">Voltar para o topo</a>)</p>

## :rocket: Tecnologias

As seguintes tecnologias foram usadas na construção do projeto:

- Next.js
- React
- TypeScript
- NextAuth.js
- Stripe
- Prismic CMS
- MongoDB
- TailwindCSS

Outras dependências e ferramentas utilizadas podem ser encontradas no arquivo [package.json](./package.json)

<p align="right">(<a href="#top">Voltar para o topo</a>)</p>

## :warning: Pré-requisitos

Antes de começar, você precisa ter as seguintes ferramentas instaladas e configuradas:

- [Git](https://git-scm.com)
- [Node.js](https://nodejs.org/en/)
- Uma conta na [Stripe](https://stripe.com/) (modo de teste) com produto/preço de assinatura configurado
- Um repositório de conteúdo configurado no [Prismic](https://prismic.io/)
- Uma instância do [MongoDB](https://www.mongodb.com/) (local ou Atlas)

<p align="right">(<a href="#top">Voltar para o topo</a>)</p>

## :checkered_flag: Começando

```bash
# Clone este repositório
$ git clone https://github.com/geovaneborba/ignite-ignews-nextjs.git

# Entre na pasta e instale as dependências
$ cd ignite-ignews-nextjs && npm i

# Crie um arquivo .env.local com as variáveis de ambiente necessárias
# (credenciais do NextAuth, Stripe, Prismic e MongoDB)
$ cp .env.local.example .env.local

# Em um terminal separado, escute os webhooks do Stripe localmente
$ npm run stripe:listen

# Inicie o projeto
$ npm run dev
```

<p align="right">(<a href="#top">Voltar para o topo</a>)</p>
<p align="center">Feito com ❤️ por <a href="https://github.com/geovaneborba" target="_blank">Geovane Borba</a></p>
