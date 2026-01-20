# 💻 Inventário de Computadores – Aplicação Web (PHP + SQL)

> [!IMPORTANT]
> **Estado do Projeto:** Este sistema encontra-se atualmente em **fase Preview (Beta)**. Algumas funcionalidades de edição e gestão avançada ainda estão em desenvolvimento.

## 🎯 Objetivo do Projeto
Este projeto consiste no desenvolvimento de uma aplicação web para gestão e consulta de um **inventário de computadores** de uma sala informática. A aplicação permite a consulta rápida de informações técnicas e do software instalado em cada equipamento, facilitando a administração do parque informático.

---

## 🧱 Estrutura do Projeto
O projeto foi desenvolvido seguindo uma estrutura modular para facilitar a manutenção e expansão futura:

| Ficheiro | Função |
| :--- | :--- |
| `config.php` | Configuração da ligação à base de dados via PDO. |
| `index.php` | Dashboard principal com listagem, filtros por sala e pesquisa. |
| `detalhe.php` | Página de detalhe com especificações técnicas e software instalado. |

---

## ⚙️ Funcionalidades (Versão Preview)
- [x] **Ligação Segura:** Conexão à base de dados utilizando PHP PDO com *Prepared Statements*.
- [x] **Listagem Dinâmica:** Visualização de todos os computadores registados.
- [x] **Filtros Avançados:** Filtragem por sala e pesquisa em tempo real por nome ou software.
- [x] **Detalhes Técnicos:** Consulta de CPU, RAM, Armazenamento e GPU de cada unidade.
- [x] **Gestão de Software:** Visualização da lista de software instalado por equipamento.
- [x] **Interface Moderna:** Design System baseado em *Glassmorphism* com suporte a **Modo Escuro**.

---

## 🛠️ Tecnologias Utilizadas
- **Backend:** PHP 8.x
- **Base de Dados:** MySQL / MariaDB
- **Frontend:** HTML5, CSS3 (Custom Properties), JavaScript (Vanilla)
- **Ícones:** Font Awesome 6.5.2
- **Tipografia:** Inter (Google Fonts)

---

## ✍️ Desenvolvimento
Este projeto foi desenvolvido integralmente de forma manual como parte da disciplina de **Programação de Sistemas de Informação**. 

- **Com AI** A parte do visual do trabalho foi feito por uma IA.
- **Foco em UX:** A interface foi desenhada para ser intuitiva, utilizando transições suaves e um layout responsivo.

---

## 🚧 Próximas Implementações
- [ ] Painel de Administração para inserção de novos ativos.
- [ ] Histórico de manutenções técnicas.

---

## 👤 Identificação
- **Disciplina:** REDES – M6 – Programação de Sistemas de Informação
 **Nome** Daniel - 14673 - 2I
