# 📊 Sistema de Inventário de Computadores – Aplicação Web (PHP + SQL)

> [!IMPORTANT]
> **Estado do Projeto:** Atualmente em **Fase Beta (I.0.3 V.27.02.2026)**. O sistema conta com uma interface moderna, pesquisa dinâmica e um painel administrativo robusto.

## 👤 Identificação
- **Nome do aluno:** Daniel
- **Turma:** 2I (Número 14673)
- **Disciplina:** REDES – M6 – Programação de Sistemas de Informação  
- **Curso:** GPSI – 2.º Ano  

---

## 🎯 Objetivo do Projeto
Este projeto consiste no desenvolvimento de uma aplicação web para gestão e consulta de um inventário de computadores de uma sala informática, utilizando PHP para a lógica da aplicação e SQL para a base de dados.

A aplicação permite consultar informações técnicas detalhadas (CPU, RAM, Armazenamento, GPU, SO) e a lista de software instalado, facilitando a administração do parque informático através de uma interface moderna e intuitiva.

---

## 🧱 Estrutura Geral do Projeto
O projeto segue uma arquitetura modular, separando a interface pública da área administrativa e da API de dados.

### 📁 Organização de Ficheiros
O sistema é composto por 11 ficheiros principais:

| Ficheiro | Tipo | Função |
| :--- | :--- | :--- |
| `index.php` | Frontend | Dashboard principal com listagem, filtros por sala e pesquisa. |
| `pesquisa.php` | Frontend | Interface de pesquisa dinâmica (Autocomplete). |
| `api_pesquisa.php` | API | Endpoint JSON que fornece dados em tempo real com ordenação natural. |
| `detalhe.php` | Frontend | Página de especificações técnicas e software instalado. |
| `criar.php` | Frontend | Formulário para submissão de novos pedidos de registo. |
| `solicitar_eliminacao.php`| Frontend | Interface para pedido de remoção de equipamentos. |
| `admin_login.php` | Admin | Autenticação segura para o painel de controlo. |
| `admin_dashboard.php` | Admin | Gestão e aprovação de pedidos pendentes de Salas e PCs. |
| `admins.php` | Admin | Gestão de utilizadores com privilégios de administrador. |
| `config.php` | Core | Centralização da ligação PDO e gestão de sessões. |
| `logout.php` | Core | Encerramento seguro de sessão administrativa. |

### 🗄️ Base de Dados
Estrutura relacional normalizada com tabelas para:
- `computadores`: Dados de hardware.
- `salas`: Localizações físicas.
- `software`: Catálogo de programas.
- `computador_software`: Tabela de ligação (N:M).
- `pedidos`: Sistema de aprovação para novos ativos.
- `admins`: Credenciais encriptadas.

---

## ⚙️ Funcionalidades Desenvolvidas

### 🎨 Design System "Liquid Glass"
- **Efeito Glassmorphism**: Interface baseada em transparências, desfoque de fundo (*backdrop-filter*) e sombras suaves.
- **Modo Escuro Nativo**: Alternância entre temas com persistência via *localStorage*.
- **UX Refinada**: Transições suaves, botões com efeito de brilho e navegação por teclado no autocomplete.

### 🔍 Gestão & Pesquisa
- **Autocomplete Inteligente**: Pesquisa que sugere resultados enquanto o utilizador escreve.
- **Otimização Técnica**: Implementação de *Debounce* (300ms) para reduzir pedidos à API.
- **Ordenação Natural**: Algoritmo SQL que ordena computadores corretamente (1, 2, 3... 10).
- **Fluxo de Aprovação**: Sistema de pedidos onde o Admin deve validar novas inserções ou remoções.

### ✅ Requisitos Cumpridos
- [x] Ligação à base de dados com PHP (PDO) segura.
- [x] Listagem dinâmica e filtros avançados.
- [x] Consulta de hardware e software por equipamento.
- [x] Pesquisa global por nome, processador ou software.
- [x] Painel de administração completo.

---

## 🤖 Utilização da Inteligência Artificial (IA)

### 🔹 Onde utilizei IA
- **Melhoria Visual**: Criação do layout baseado no Design System "Liquid Glass" e CSS para Modo Escuro.
- **Lógica de Pesquisa**: Desenvolvimento da API JSON e da lógica de *Debounce* em JavaScript.
- **Queries Complexas**: Otimização da ordenação natural (tratar números como números no SQL).
- **Resolução de Erros**: Apoio na depuração de sessões PHP e transações SQL.

### 🔹 Como utilizei a IA
A IA (Manus) serviu como um consultor técnico. O processo envolveu pedir sugestões para componentes visuais modernos e algoritmos de pesquisa. Cada sugestão foi analisada, adaptada para o contexto do projeto e testada manualmente para garantir a compatibilidade com o servidor InfinityFree.

---

## ✍️ Trabalho Desenvolvido Manualmente
- **Integração Core**: Toda a ligação entre os ficheiros e a base de dados foi estruturada pelo aluno.
- **Lógica de Aprovação**: A decisão de criar um sistema de "pedidos" antes da inserção final na base de dados.
- **Personalização**: Ajuste de cores, textos e ícones para o contexto escolar.
- **Gestão de Base de Dados**: Criação e manutenção das tabelas no phpMyAdmin.

---

## 🚧 Dificuldades Encontradas
- **Ordenação Natural**: Resolver o problema de o SQL ordenar "PC 10" antes de "PC 2".
- **Sincronização de CSS**: Manter a consistência visual do tema "Glass" em todas as 11 páginas.
- **Transações SQL**: Garantir que a eliminação de um PC também limpava corretamente as suas associações de software.

---

## 📚 Aprendizagens Realizadas
- **Desenvolvimento Fullstack**: Compreensão da ligação entre Frontend (JS/CSS), API (JSON) e Backend (PHP/SQL).
- **Segurança Web**: Importância de *Prepared Statements* e encriptação de passwords.
- **UX/UI**: Como pequenos detalhes visuais e de performance (Debounce) melhoram a experiência do utilizador.
- **Documentação Técnica**: Valor de um README bem estruturado para a manutenção do projeto.

---

## 🔗 Links do Projeto
- **Site Online:** [Inventário - Versão Beta](https://a14673-oficina.infinityfree.me/M6/inventario/?i=1)
