---
title: "EduSync"
draft: false
language: pt-br
featured_image: images/featured/EduSync.png
summary: Plataforma acadêmica inteligente que conecta professores e alunos, permitindo o lançamento de notas e frequência, acompanhamento de desempenho e visualização de resultados em tempo real.
author: Unifil
categories: Blog
tags: ["CC", "ES", "ADS", "Educação", "Tecnologia"]
linkweb: https://plataforma-academica.vercel.app/

---

# EduSync — Plataforma Acadêmica Inteligente

O **EduSync** é uma plataforma acadêmica web desenvolvida para facilitar a comunicação e o acompanhamento escolar entre professores e alunos. Por meio de uma interface simples e intuitiva, o sistema centraliza o gerenciamento de notas e frequência, tornando o processo educacional mais transparente e eficiente.

---

## Sobre o Projeto

O EduSync surgiu da necessidade de digitalizar e simplificar o acompanhamento acadêmico em instituições de ensino. A plataforma oferece dois perfis distintos de acesso — **Professor** e **Aluno** — cada um com funcionalidades específicas para atender às demandas do dia a dia escolar.

---

## Funcionalidades

### 👨‍🏫 Perfil Professor
- Lançamento e edição de **notas** por aluno e por matéria
- Registro e atualização de **frequência** individual
- Visão geral da turma com todos os alunos cadastrados
- Gerenciamento de múltiplas disciplinas simultaneamente

### 👨‍🎓 Perfil Aluno
- Visualização das **notas por matéria**
- Acompanhamento da **média geral**
- Monitoramento do percentual de **frequência**
- **Gráfico de desempenho** individual para análise visual do progresso

---

## Tecnologias Utilizadas

| Camada | Tecnologia |
| ------ | ---------- |
| Backend | Python + Flask |
| Banco de Dados | SQLite |
| Frontend | HTML + Tailwind CSS |
| Deploy | Vercel |

---

## Matérias Suportadas

A plataforma gerencia notas e frequência nas seguintes disciplinas:

- Matemática
- Português
- História
- Geografia
- Física
- Química
- Biologia
- Inglês

---

## Como Acessar

A plataforma está disponível online pelo link:

🔗 [https://plataforma-academica.vercel.app/](https://plataforma-academica.vercel.app/)

### Credenciais de Demonstração

| Usuário | Senha | Perfil |
| ------- | ----- | ------ |
| carlos | 123 | Professor |
| joao | 123 | Aluno |
| maria | 123 | Aluno |
| pedro | 123 | Aluno |
| ana | 123 | Aluno |

---

## Estrutura do Sistema

```
edusync/
├── app.py              ← Backend Flask + SQLite
├── requirements.txt    ← Dependências do projeto
├── edusync.db          ← Banco de dados (criado automaticamente)
└── templates/
    ├── index.html      ← Tela de Login
    ├── professor.html  ← Painel do Professor
    └── aluno.html      ← Painel do Aluno
```

---

## Como Rodar Localmente

```bash
# 1. Instalar dependências
pip install -r requirements.txt

# 2. Iniciar o servidor
python app.py
```

Acesse: [http://localhost:5000](http://localhost:5000)

---

> O EduSync é um projeto acadêmico desenvolvido com foco em praticidade e usabilidade, conectando a comunidade escolar de forma digital e organizada.
