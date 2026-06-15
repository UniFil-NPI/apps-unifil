---
date: 2026-06-15
title: "ServiceGO"
draft: false
language: pt-br
featured_image: images/featured/ServiceGo.png 
summary: O ServiceGO é uma plataforma brasileira de marketplace de serviços que conecta clientes a prestadores autônomos locais, contando com um sistema inovador de geolocalização e acompanhamento de rota ativa em tempo real, desenvolvido sob rígidos padrões de privacidade e segurança da LGPD.
author: Gustavo Gabriel, Romulo Gusso, João Nagata e João Bueno
categories: Blog
tags: ["ADS", "ES", "CC", "Tecnologia", "Educação"]
linkweb: servicego.online
GitHub: https://github.com/GustLobato/ServiceGO
---


# ServiceGO: Conexão Segura e Rastreamento de Serviços

O **ServiceGO** é um marketplace brasileiro que revoluciona a contratação de prestadores de serviços autônomos (encanadores, eletricistas, pintores, diaristas, técnicos e reformadores). O projeto foi concebido e aprimorado como um **Projeto de Extensão Universitária (UniFil)**, unindo conceitos avançados de engenharia de software à realidade social, entregando uma ferramenta com alta usabilidade, interatividade e conformidade legal.

---

## Principais Funcionalidades

### 1. Mini Mapa e Rastreamento em Tempo Real
O coração visual do ServiceGO é o seu **Mini Mapa de Acompanhamento Interativo**, que opera em dois modos distintos:
* **Modo Radar de Busca (Sem pedido ativo):** O mapa localiza o usuário (via GPS ou manualmente) e renderiza múltiplos prestadores ativos ao redor em tempo real. Cada pino laranja é clicável e exibe dados como avaliações, quantidade de serviços e um botão para iniciar uma contratação simulada.
* **Modo Acompanhamento de Rota (Contratação ativa):** Ao selecionar um profissional ou clicar no painel de contratação, o mapa limpa a tela e traça um trajeto curvilíneo em SVG. Um carrinho animado desloca-se em tempo real na tela, enquanto cartões flutuantes calculam a **distância restante (km)** e a **estimativa de chegada (ETA)** de forma decrescente. O *stepper* inferior acompanha cada etapa (Solicitada ➔ A caminho ➔ Chegando ➔ Concluído).

### 2. Busca Geolocalizada com Raio de Distância
Os clientes podem buscar profissionais baseando-se em:
* **Nome ou Categoria** de atuação.
* **Cidade / Região** digitada manualmente ou geolocalizada via GPS.
* **Filtro de Distância Limitador:** Busca refinada por raios de `Até 2 km`, `Até 5 km`, `Até 10 km`, `Até 25 km` ou `Qualquer distância`.
* Cada card de profissional exibe um badge contextual informando a distância estimada (ex: *`2.4 km de você`*) ou *`Atende sua região`*.

### 3. Conformidade Rígida com a LGPD (Privacidade por Design)
Todo o fluxo de coleta e exibição de dados pessoais foi planejado para resguardar a privacidade do usuário:
* **Consentimento de GPS Explicativo:** A geolocalização nunca é ativada de forma abusiva. Ao clicar no botão de GPS, um modal claro explica a finalidade dos dados (estimar distância) e garante que as coordenadas exatas não serão salvas em banco de dados ou exibidas publicamente.
* **Privacidade do Endereço:** O endereço completo e o número de contato do cliente **só são liberados para o profissional contratado após a aceitação formal** e confirmação do agendamento, mantendo o anonimato na fase de buscas.
* **Controle Granular de Cookies:** Banner de cookies em conformidade com as regras europeias e brasileiras. Permite ao usuário aceitar todos, recusar opcionais ou configurar preferências individuais (Essenciais, Preferências, Análise e Marketing).
* **Exclusão Definitiva de Conta e Dados:** Direto no painel do perfil, tanto clientes quanto prestadores têm o canal e a estrutura técnica para solicitar a exclusão total da conta, com alertas detalhados sobre prazos regulatórios exigidos pelo Marco Civil da Internet (Lei 12.965/14).

---

##  Stack Tecnológica

O projeto foi construído utilizando práticas modernas de desenvolvimento web de alto desempenho:

| Tecnologia | Descrição |
| :--- | :--- |
| **React 18** | Biblioteca para construção da interface SPA reativa. |
| **Vite v8** | Ferramenta de build rápida com HMR (Hot Module Replacement) instantâneo. |
| **TypeScript** | Tipagem estática para robustez e redução de bugs de compilação. |
| **Tailwind CSS** | Estilização ágil baseada em classes utilitárias e design fluido. |
| **Leaflet & CartoDB** | Biblioteca leve de mapas com tiles Positron minimalistas de alto contraste. |
| **Framer Motion** | Micro-animações fluidas nos badges, modais e transições de tela. |
| **React Query** | Gerenciamento de estado assíncrono e cache de dados de API. |
| **Lucide Icons** | Conjunto de ícones vetoriais modernos e leves. |

---

## Estrutura de Páginas e Rotas

O sistema dispõe de rotas otimizadas por *lazy loading*, reduzindo drasticamente o tamanho do bundle inicial:

1. **`Landing Page (/)`**: Hero impactante, mini mapa simulador interativo, como funciona, seções de categorias de profissionais, depoimentos e chamadas para ação.
2. **`Cadastro (/cadastro)`**: Criação de contas segmentadas para Clientes ou Prestadores, com validação de força de senha em tempo real e caixas de seleção obrigatórias de aceitação dos Termos.
3. **`Login (/login)`**: Login seguro com controle de sessão.
4. **`Dashboard (/dashboard)`**: Painel administrativo protegido por guardas de rotas, contendo:
   * **Home do Painel:** Estatísticas resumidas e solicitações recentes.
   * **Buscar Serviços:** Busca avançada com geolocalização, categorias e filtros de raio.
   * **Solicitações:** Acompanhamento de serviços pendentes, aceitos e em andamento.
   * **Avaliações:** Gestão de reviews de serviços concluídos.
   * **Perfil:** Edição de dados, configurações de segurança e painel de privacidade de dados (LGPD).
5. **`Política de Privacidade (/privacy)`**: Documento em linguagem simples explicando a coleta, termos de GPS e DPO (`privacidade@servicego.com.br`).
6. **`Termos de Uso (/terms)`**: Direitos de interposição, limitações da plataforma e regras de convivência.

