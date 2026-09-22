# 🚗 Sistema para Oficina Mecânica (mecanica-nome1-nome2)

![Status do Projeto](https://img.shields.io/badge/Status-Em%20Desenvolvimento-green)
![Licença](https://img.shields.io/badge/License-MIT-blue)

## 📖 Contextualização
Este projeto visa solucionar os desafios diários de uma oficina mecânica que atualmente realiza o controle de seus atendimentos de forma manual. A ausência de um sistema informatizado tem gerado perda de reservas, duplicidade de dados e falhas no armazenamento. 

Além da organização, o sistema tem como foco a **Segurança da Informação e adequação à LGPD (Lei Geral de Proteção de Dados)**, garantindo que dados sensíveis dos clientes (como o CPF e senhas) sejam armazenados de forma criptografada e segura.

O objetivo final é entregar uma aplicação intuitiva, segura e bem documentada para o gerenciamento completo da rotina da oficina.

---

## 🚀 Tecnologias Utilizadas

> **Nota aos desenvolvedores:** Atualizem esta seção com as tecnologias e bibliotecas exatas que serão utilizadas no projeto.

* **Front-end:** [Ex: React.js / HTML, CSS, JS / Vue.js]
* **Back-end:** [Ex: Node.js com Express / Java Spring Boot / PHP]
* **Banco de Dados:** [Ex: PostgreSQL / MySQL / SQL Server]
* **Autenticação:** [Ex: JWT (JSON Web Tokens) / Sessões]
* **Criptografia:** [Ex: Bcrypt para senhas e algoritmos AES para dados sensíveis]

---

## ⚙️ Funcionalidades e Regras de Negócio

O sistema foi desenhado para atender às seguintes regras de negócio estabelecidas pelo gestor da oficina:

- [x] **Autenticação e Sessão:** Login seguro com validação de falhas (feedbacks claros ao usuário) e tempo de expiração de sessão.
- [x] **Painel Principal (Dashboard):** Exibição do nome do usuário logado, menu de navegação fácil para os demais recursos e botão de logout seguro.
- [x] **Gestão de Clientes:** Cadastro, edição e listagem. Inclui um recurso de busca dinâmica (após inserir e confirmar o termo, a tabela é atualizada apenas com os registros correspondentes).
- [x] **Gestão de Veículos:** Cadastro e gerenciamento. **Regra crítica:** Todo veículo deve obrigatoriamente estar associado a um cliente existente.
- [x] **Gestão de Agendamentos:** Listagem de todos os serviços agendados, ordenados por data. A visualização deve trazer os dados atrelados do Cliente e do Veículo.
- [x] **Segurança e LGPD:** Criptografia obrigatória no banco de dados para dados sensíveis (ex: CPF do cliente).

---

## 📁 Estrutura de Entregas do Projeto

O repositório deve seguir a estrutura baseada no diretório `seunome_simuladomecanica` contendo os seguintes artefatos:

| Nº | Entrega | Arquivo/Formato |
|:---:|---|---|
| 1 | Documentação de Software | `documentos/documentacao.pdf` |
| 2 | Diagrama Entidade Relacionamento (DER) | `documentos/diagrama_er.png` ou `.pdf` |
| 3 | Script do Banco de Dados (DDL e DML) | `banco/simuladoMecanica_db.sql`* |
| 4 | Código Fonte | Estrutura de pastas do projeto neste repositório |

*\* O script do banco de dados já deve conter a criação das tabelas e a inserção de pelo menos **3 registros iniciais (mock)** para cada tabela (respeitando chaves e tipos de dados).*

---

## 💻 Como executar o projeto localmente

Siga os passos abaixo para rodar a aplicação na sua máquina:

### Pré-requisitos
* [Node.js](https://nodejs.org/) (ou outra tecnologia de backend escolhida)
* [MySQL / PostgreSQL] rodando localmente
* [Git](https://git-scm.com/)

### Passo a Passo

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/usuario/mecanica-nome1-nome2.git
   ```

2. **Acesse a pasta do projeto:**
   ```bash
   cd mecanica-nome1-nome2/seunome_simuladomecanica
   ```

3. **Configuração do Banco de Dados:**
   * Crie um banco de dados no seu SGBD.
   * Execute o script `banco/simuladoMecanica_db.sql` para criar as tabelas e popular os dados iniciais.
   * Configure as variáveis de ambiente (ex: arquivo `.env`) com as credenciais do seu banco local.

4. **Instale as dependências:**
   ```bash
   # Exemplo para Node.js
   npm install
   ```

5. **Execute a aplicação:**
   ```bash
   npm start
   ```

---

## 👥 Autores

* **[Nome do Aluno 1]** - *Desenvolvimento Fullstack* - [GitHub](https://github.com/link1)
* **[Nome do Aluno 2]** - *Desenvolvimento Fullstack* - [GitHub](https://github.com/link2)

*Projeto desenvolvido como atividade prática simulada de engenharia de software.*
