# WebShop_demo

[EN]

# WebShop

This repository implements an e-commerce application consisting of a backend and a frontend. The content of this file is a public description and does not include routes, URLs, or sensitive data.

## Project description

E-commerce application with two main layers:
- Backend: REST API responsible for business logic, persistence, and administrative operations.
- Frontend: Single Page Application (SPA) for end-user interaction (catalogue, shopping cart, checkout).

The project was developed with a focus on modularity, scalability, and accessibility.

## Implemented features — Backend (high level)

- Authentication and account management (access tokens, password recovery flow).
- Catalogue management: creation, editing, listing and product details (support for variants and images).
- Management of categories and subcategories.
- Secure image upload with type/size validation and unique file name generation.
- Cart and order flow management (includes order statuses and shipping methods).
- Support for coupons/promotions, wish lists, and reviews (features already present or prepared in the API).
- Administrative features for catalogue/stock and profile management.
- Operational utilities: startup scripts, health checks, and maintenance tools for development environments.

## Implemented features — Frontend (high level)

- React SPA with catalogue navigation, product detail page, shopping cart, and checkout flow.
- Communication with the API via HTTP client (with error handling and loading states).
- Scripts for development and build prepared for integration with the local backend.

## Security observed (existing implementations)

- Security headers applied on the server (basic measures configured).
- Rate limiting to reduce the surface area for brute force attacks and abuse of sensitive endpoints.
- Restrictive CORS policies by default for the development environment.
- Input validation on sensitive routes (validation libraries and middleware in use).
- Uploads validated by file type, extension, and size; randomly generated file names to avoid collisions/path traversal.
- Token-based authentication with handling of expired and invalid tokens.

## Technologies used (summary)

- Backend: Node.js, Express, ORM, relational database (PostgreSQL), JWT for authentication, multer for uploads.
- Frontend: React, Vite, axios, react-router-dom, configured styling and build tools.


[PT]

# WebShop 

Este repositório implementa uma aplicação de comércio eletrónico composta por um backend e um frontend. O conteúdo deste ficheiro é uma descrição pública e não inclui rotas, URLs ou dados sensíveis.

## Descrição do projecto

Aplicação de e‑commerce com duas camadas principais:
- Backend: API REST responsável pela lógica de negócio, persistência e operações administrativas.
- Frontend: Single Page Application (SPA) para interação do utilizador final (catálogo, carrinho, checkout).

O projeto foi desenvolvido com foco em modularidade, escalonamento e acessibilidade.

## Funcionalidades implementadas — Backend (alto nível)

- Autenticação e gestão de contas (tokens de acesso, fluxo de recuperação de senha).
- Gestão de catálogo: criação, edição, listagem e detalhe de produtos (suporte a variantes e imagens).
- Gestão de categorias e subcategorias.
- Upload seguro de imagens com validação de tipo/ tamanho e geração de nomes únicos para ficheiros.
- Gestão de carrinho e fluxo de pedidos (inclui estados de pedido e modos de envio).
- Suporte a cupões/promos, wishlist e avaliações (funcionalidades já presentes ou preparadas na API).
- Funcionalidades administrativas para gestão de catálogo/stock e perfis.
- Utilitários operacionais: scripts de inicialização, health-check e ferramentas de manutenção para ambientes de desenvolvimento.

## Funcionalidades implementadas — Frontend (alto nível)

- SPA React com navegação por catálogo, página de detalhe do produto, carrinho e fluxo de checkout.
- Comunicação com a API através de cliente HTTP (com tratamento de erros e estados de carregamento).
- Scripts para desenvolvimento e build preparados para integração com o backend local.

## Segurança observada (implementações existentes)

- Headers de segurança aplicados no servidor (medidas básicas configuradas).
- Rate limiting para reduzir a superfície de ataques por força bruta e abusos de endpoints sensíveis.
- Políticas CORS restritivas por defeito para o ambiente de desenvolvimento.
- Validação de entradas nas rotas sensíveis (bibliotecas e middlewares de validação em uso).
- Uploads validados por tipo de ficheiro, extensão e tamanho; nomes de ficheiro gerados de forma aleatória para evitar colisões/ path traversal.
- Autenticação baseada em tokens com tratamento de tokens expirados e inválidos.

## Tecnologias utilizadas (resumo)

- Backend: Node.js, Express, ORM, base de dados relacional (PostgreSQL), JWT para autenticação, multer para uploads.
- Frontend: React, Vite, axios, react-router-dom, ferramentas de estilização e build configuradas.


