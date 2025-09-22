
# LogsUp: Painel de Gestão de Produtos e Usuários

Projeto de exemplo que consiste em um **Painel de Produtos** e uma **API de Back-end** para gerenciar produtos e usuários.

---

## 💻 Visão Geral

O **LogsUp** é uma aplicação completa, dividida em duas partes principais que trabalham em conjunto:

* **API de Servidor (`ServerAPIs`)**: O coração do projeto. Responsável por fornecer dados, executar operações CRUD (Criar, Ler, Atualizar, Excluir) em produtos e usuários, e gerenciar a autenticação.
* **Painel Front-end (`meu-painel-de-produtos`)**: Uma interface simples e intuitiva para visualizar, criar, editar e excluir produtos.

O objetivo principal é oferecer um sistema básico, mas funcional, para a gestão de produtos e usuários, ideal para ser usado como base para projetos maiores ou como um portfólio.

---

## ✨ Funcionalidades

O LogsUp oferece as seguintes funcionalidades principais:

* **Listagem de Produtos**: Visualização de todos os produtos cadastrados.
* **Gestão de Produtos**:
    * Criação de novos produtos.
    * Edição de produtos existentes.
    * Exclusão de produtos.
* **Autenticação e Autorização**: Sistema de login para acesso seguro ao painel.
* **Scripts SQL**: Consultas personalizadas para manipulação do banco de dados.

---

## 📂 Estrutura do Projeto

A estrutura de pastas foi organizada para separar claramente o front-end do back-end, facilitando a navegação e a manutenção do código.

## 🏗️ Estrutura do Projeto  

```bash
LogsUp-Projeto/
├── ServerAPIs/                  # 🌐 Backend (API)
│   ├── src/
│   │   ├── controllers/         # 🎯 Lógica de negócio das rotas
│   │   ├── models/              # 🗄️ Modelos de dados e banco de dados
│   │   ├── routes/              # 🛤️ Definição das rotas da API
│   │   └── index.js             # 🚀 Ponto de entrada da API
│   ├── package.json
│   └── ...
│
├── meu-painel-de-produtos/      # 🖥️ Front-end / Painel de Gerenciamento
│   ├── public/                  # 🌍 Arquivos estáticos (index.html, favicon, etc.)
│   ├── src/
│   │   ├── components/          # 🧩 Componentes reutilizáveis
│   │   ├── pages/               # 📄 Páginas da aplicação (Login, Dashboard, etc.)
│   │   ├── services/            # 🔗 Lógica de comunicação com a API
│   │

```


---

## 🛠️ Tecnologias

A aplicação foi construída utilizando tecnologias modernas e amplamente utilizadas no mercado:

* **Backend**: [Node.js](https://nodejs.org/) e [Express](https://expressjs.com/)
* **Banco de Dados**: Qualquer banco de dados SQL (ex: MySQL, PostgreSQL, SQL Server)
* **Frontend**: [React](https://react.dev/), [Vite](https://vitejs.dev/) e [Bootstrap](https://getbootstrap.com/)
* **Comunicação HTTP**: [Axios](https://axios-http.com/)

---

## 🚀 Pré-requisitos

Antes de iniciar, certifique-se de que você tem instalado em sua máquina:

* **Node.js** (versão 14.x ou superior)
* **npm** ou **yarn**
* Um **servidor de banco de dados SQL** configurado (como MySQL, PostgreSQL, etc.)

---

## ⚙️ Instalação e Execução

Siga os passos abaixo para configurar e rodar o projeto em sua máquina local.

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/gabrielsantiag0/LogsUp-Projeto.git](https://github.com/gabrielsantiag0/LogsUp-Projeto.git)
    cd LogsUp-Projeto
    ```

2.  **Instale as dependências do back-end:**
    ```bash
    cd ServerAPIs
    npm install
    ```

3.  **Instale as dependências do front-end:**
    ```bash
    cd ../meu-painel-de-produtos
    npm install
    ```

4.  **Configure o banco de dados:**
    * Crie um banco de dados vazio.
    * Execute o script `SQLQuery2.txt` para criar as tabelas necessárias.

5.  **Configure as variáveis de ambiente:**
    * Crie um arquivo `.env` dentro da pasta `ServerAPIs`.
    * Preencha-o com as suas credenciais do banco de dados e a chave JWT.

    ```bash
    DB_SERVER=seu_servidor_de_banco_de_dados
    DB_USER=seu_usuario
    DB_PASSWORD=sua_senha
    DB_DATABASE=SistemaProdutos
    JWT_SECRET=sua_chave_secreta_jwt
    ```
    ⚠️ **Importante**: Mude `sua_chave_secreta_jwt` para uma string mais segura.

6.  **Execute os projetos:**
    * Na pasta raiz do projeto (`LogsUp-Projeto`), rode o comando para iniciar os dois servidores simultaneamente:

    ```bash
    npm run start-all
    ```
    * O back-end será iniciado na porta padrão (geralmente `3000`) e o front-end na porta `5173`. Acesse `http://localhost:5173` no seu navegador para ver o painel.

---

## 🔑 Credenciais de Teste

Utilize as seguintes credenciais para acessar o painel de administração:

* **E-mail**: `admin@email.com`
* **Senha**: `admin`

---

## 🤝 Contribuição

Sinta-se à vontade para contribuir com o projeto! Siga os passos abaixo para começar:

1.  Faça um **fork** deste repositório.
2.  Crie uma nova branch para sua feature: `git checkout -b minha-nova-feature`.
3.  Faça o commit das suas alterações: `git commit -m "feat: Adiciona minha nova feature"`.
4.  Envie suas alterações para o repositório original: `git push origin minha-nova-feature`.
5.  Abra um **Pull Request**.

---

## ✒️ Autor

* **Gabriel Santiago**
* **GitHub**: [https://github.com/gabrielsantiag0](https://github.com/gabrielsantiag0)
* **LinkedIn**: [https://www.linkedin.com/in/gabrielmsantiago/](https://www.linkedin.com/in/gabrielmsantiago/)

---

## 📜 Licença

Este projeto está licenciado sob a Licença MIT.
