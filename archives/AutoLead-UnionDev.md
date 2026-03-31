---
title: "AutoLead - UnionDev"
summary: Este projeto oferece uma solução automatizada e eficiente para pesquisas de locais, utilizando as poderosas funcionalidades da API do Google Maps integradas com a interação facilitada pelo Telebot. A criação e envio de arquivos CSV proporcionam uma maneira estruturada e acessível de visualizar os resultados, atendendo a diversas necessidades de usuários e empresas.
featured_image: images/featured/AutoLead-UnionDev.png

date: 2025-07-08
draft: false
important: 1
language: pt-br
author: Unifil
categories: Blog
tags: ["CC", "ES","Tecnologia"] 
linkweb: http://150.230.87.220/
linkblog: https://sites.google.com/edu.unifil.br/uniondev/quem-somos
linkvideo: https://youtu.be/0IOKBEtxjPc?feature=shared

---

__Links uteis :smile:__

- __[Git do Projeto](https://github.com/JoaoPipous/UnionDev-AutoLead)__ 
---

# AutoLead: Site de Pesquisa de Locais com Telebot e Google Maps API

## Visão Geral do Projeto

AutoLead é um site inovador que utiliza as bibliotecas `telebot` e `googlemaps` para permitir que os usuários realizem pesquisas de locais próximos a uma localização específica. Este projeto foi desenvolvido para proporcionar uma maneira automatizada e eficiente de obter informações detalhadas sobre estabelecimentos dentro de um raio determinado em uma cidade especificada pelo usuário. Os resultados são organizados em um arquivo CSV, que é enviado de volta ao usuário, facilitando a visualização e armazenamento das informações.

## Funcionalidades do AutoLead

### 1. Interação com Usuários
O Site começa interagindo com os usuários para coletar as informações necessárias para a pesquisa. Ele solicita:
- **Cidade:** O nome da cidade onde os locais devem ser pesquisados.
- **Raio (metros):** A distância em metros a partir da localização central na cidade especificada.
- **Segmento:** O tipo de estabelecimento que o usuário está procurando (por exemplo, restaurantes, lojas, etc.).
- **Nome do Arquivo:** O nome desejado para o arquivo CSV que será gerado com os resultados da pesquisa.

### 2. Busca de Locais
Utilizando a API do Google Maps, o site realiza a busca de locais que correspondem aos critérios fornecidos pelo usuário. A API é chamada para identificar os estabelecimentos dentro do raio especificado na cidade indicada.

### 3. Geração de Arquivo CSV
Uma vez que a busca é concluída, o site organiza os dados obtidos, incluindo o nome, endereço e telefone dos locais encontrados, em um arquivo CSV. Este arquivo é estruturado para facilitar a leitura e o uso das informações.

### 4. Envio do CSV ao Usuário
Finalmente,o site envia o arquivo CSV de volta ao usuário através de um download, proporcionando uma maneira conveniente e eficiente de visualizar e armazenar as informações coletadas.

## Exemplos Visuais

### Interface de Entrada de Dados
Na interface inicial, os usuários são recebidos com um formulário simples onde podem fornecer as informações necessárias para a pesquisa. Abaixo está um exemplo da tela de entrada de dados:

![Interface de Entrada de Dados](https://i.imgur.com/5iucDZQ.jpeg)

### Exemplo de Resultados
Após a busca, o site organiza os resultados em uma tabela e os envia em um arquivo CSV. Abaixo está um exemplo de como os dados são exibidos:

![Exemplo de Resultados](https://i.imgur.com/CQEUsSL.jpeg)  

## Benefícios do AutoLead

- **Facilidade de Uso:** Com uma interface intuitiva, os usuários podem rapidamente fornecer as informações necessárias e obter os resultados desejados.
- **Eficiência:** A integração com a API do Google Maps permite uma busca rápida e precisa de locais.
- **Conveniência:** A geração e envio de arquivos CSV proporcionam uma maneira estruturada de visualizar e armazenar os resultados, atendendo às necessidades de usuários e empresas de forma prática.
- **Automatização:** O site automatiza o processo de busca e organização de dados, economizando tempo e esforço para os usuários.

## Conclusão

AutoLead é uma ferramenta poderosa e eficiente para quem precisa encontrar estabelecimentos próximos a uma localização específica. Com sua interface amigável e integração com a API do Google Maps, ele oferece uma solução prática para a coleta e visualização de dados sobre locais de interesse. Experimente o AutoLead hoje e veja como ele pode facilitar suas pesquisas de locais!

---

Esperamos que você aproveite o AutoLead e suas funcionalidades! Se tiver alguma dúvida ou sugestão, não hesite em nos contactar.
