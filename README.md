# API Livraria Innovva

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=JavaScript&logoColor=white) ![JSON](https://img.shields.io/badge/json%20web%20tokens-323330?style=for-the-badge&logo=json-web-tokens&logoColor=pink) ![NodeJS](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white) ![ESLINT](https://img.shields.io/badge/eslint-3A33D1?style=for-the-badge&logo=eslint&logoColor=white) ![EXPRESS](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge) ![SQLite3](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white) ![JEST](https://img.shields.io/badge/Jest-323330?style=for-the-badge&logo=Jest&logoColor=white)

## Aplicativo de Livraria especializada em Livros de Skills baseado em NodeJS

### O aplicativo Nova Livraria é uma loja virtual que vende livros da Casa do Código. Livraria com sistema de cadastro e manejo de livros, autores e editoras. Neste o principal é a realização testes unitários com Jest e testes de integração com Supertest.

### É um MVP que tá só começando e ainda tem muitas funcionalidades novas para serem desenvolvidas.

### Baseado nos cursos de formação para atualização profissional chamado“Node.js: testes unitários e de integração”, disponibilizado pela Alura e ministrado pelo instrutor João Manoel Lima e no curso “Node.js: implementando testes em uma API Rest”, disponibilizado pela Alura e ministrado pelo instrutor Raphael Lucas Girao de Lima. Nesta oportunidade pude atualizar meus conhecimentos em:

#### Primeiro curso:

* Aprender os conceitos de testes e como utilizá-los
* Entender a importância e os benefícios de testar o código
* Fazer os primeiros testes unitários com Jest
* Fazer os primeiros testes de integração com Supertest

#### Segundo curso:

* Criar testes unitarios utilizando padrão triple A
* Desenvolver testes mais organizados e estruturados
* Criar testes de integração
* Criar testes de banco de dados
* Aprender a classificar tipos de testes como caixa branca, caixa preta e E2E
* Implementar testes de imagens e disparo de e-mail em uma API Rest
* Desenvolvimento orientado a testes utilizando o TDD

## 🛠️ Instalação

Este projeto já conta com o código necessário para subir a API em um servidor local:

```
├── .env
├── .eslintrc.cjs
├── .gitignore
├── .nvmrc
├── package.json
├── package-lock.json
├── populate.sql
├── README.md
├── server.js
├── src
│   ├── app.js
│   ├── config
│   │   └── constants.js
│   │   └── nodeMailer.js
│   ├── controllers
│   │   └── aluguelLivroController.js
│   │   └── authController.js
│   │   └── autoresController.js
│   │   └── editorasController.js
│   │   └── livrosController.js
│   │   └── livrosImagensController.js
│   │   └── usuariosController.js
│   ├── db
│   │   └── dbconfig.js
│   │   └── livraria.sqlite
│   ├── middleware
│   │   └── autenticado.js
│   ├── models
│   │   └── aluguel_livro.js
│   │   └── autor.js
│   │   └── editora.js
│   │   └── livro_imagem.js
│   │   └── livro.js
│   │   └── usuario.js
│   ├── routes
│   │   └── aluguelLivroRoutes.js
│   │   └── authRoutes.js
│   │   └── autoresRoutes.js
│   │   └── editorasRoutes.js
│   │   └── index.js
│   │   └── livrosImagensRoutes.js
│   │   └── livrosRoutes.js
│   │   └── usuariosRoutes.js
│   ├── services
│   │   └── aluguelLivroService.js
│   │   └── authService.js
│   │   └── autoresService.js
│   │   └── editorasService.js
│   │   └── livrosImagensService.js
│   │   └── livrosService.js
│   │   └── usuariosService.js
│   ├── test
│   │   │   ├── models
│   │   │   │   └── editora.test.js
│   │   │   ├── routes
│   │   │   │   └── editorasRoutes.test.js
```

### Instalação do projeto

* Baixe o repositório do projeto, navegue via terminal até a pasta e instale as dependências necessárias com `npm install`.
* Confira se a pasta `node_modules` foi criada na raiz do projeto.

### Instalação dos drivers do SQLite (Linux Debian/Ubuntu)

* Este projeto utiliza o SQLite como gerenciador de banco de dados SQL. O SQLite utiliza um arquivo, normalmente de extensão `.sqlite` ou `.db`, para guardar os dados.
* O projeto já conta com uma base de dados configurada e populada com alguns dados iniciais, localizado na pasta `src/db/livraria.sqlite`. Para utilizar estes dados é necessário ter os drivers do SQLite instalados localmente no computador; você pode seguir os passos abaixo para instalar e acessar os dados:

* Instalar o `sqlite` globalmente no computador:
  `sudo apt update`
  `sudo apt install sqlite3`
  
* Verifique a instalação com:
  `sqlite3 --version`

* Utilize o cli do SQLite para acessar o arquivo `src/db/livraria.sqlite` e fazer consultas via terminal:
  `sqlite3 ./src/db/livraria.sqlite`. O terminal deverá exibir a seguinte mensagem (a data e hora do acesso serão as locais do momento em que você acessar):
  ```
  SQLite version 3.31.1 2020-01-27 19:55:54
  Enter ".help" for usage hints.
  sqlite>
  ```
  
### Instalação dos drivers do SQLite (Linux Debian/Ubuntu)

* Este projeto utiliza o SQLite como gerenciador de banco de dados SQL. O SQLite utiliza um arquivo, normalmente de extensão `.sqlite` ou `.db`, para guardar os dados.
* O projeto já conta com uma base de dados configurada e populada com alguns dados iniciais, localizado na pasta `src/db/livraria.sqlite`. Para utilizar estes dados é necessário ter os drivers do SQLite instalados localmente no computador; você pode seguir os passos abaixo para instalar e acessar os dados: 

* Instalar o `sqlite` globalmente no computador:
  `sudo apt update`
  `sudo apt install sqlite3`
  
### Instalação dos drivers do SQLite (Windows)

* Faça o download dos drivers SQLite na página: https://www.sqlite.org/download.html
* Selecione o sistema operacional e faça o download do arquivo [Precompiled binaries for Windows - SQLite Tools](https://sqlite.org/2022/sqlite-tools-win32-x86-3380500.zip)
* Crie uma pasta chamada  ```sqlite3```na unidade C:\ do seu computador. O caminho final será: ``` C:\sqlite3```.
* Insira os arquivos SQLite descompactados na pasta C:\sqlite3 (você deverá extrair os arquivos para a pasta C:\sqlite3)
* Abra "Exibir configurações avançadas do Sistema" (Advanced System Properties). Painel de controle (Control Panel) > Sistema (System) > Configurações avançadas do Sistema (Advanced System Settings).
* Selecione "Variáveis de Ambiente"
* Em variáveis de sistema, selecione a variável PATH e clique em **Editar..** 
* **Adicione C:\sqlite3 ao final** e selecione a opção ok

[![Add sqlite3 to Windows PATH Variable ](https://storage.googleapis.com/static.configserverfirewall.com/images/windows10/sqlite3/sqlite3path.png)](https://storage.googleapis.com/static.configserverfirewall.com/images/windows10/sqlite3/sqlite3path.png)

#### Depois execute o cmd como administrador e rode o comando ```sqlite3```

### Configuração dos drivers SQLite

* Verifique a instalação com:
  `sqlite3 --version`
* Utilize o cli do SQLite para acessar o arquivo `src/db/livraria.sqlite` e fazer consultas via terminal:
  `sqlite3 ./src/db/livraria.sqlite`. O terminal deverá exibir a seguinte mensagem (a data e hora do acesso serão as locais do momento em que você acessar):
  ```
  SQLite version 3.31.1 2020-01-27 19:55:54
  Enter ".help" for usage hints.
  sqlite>
  ```

* Digite os seguintes comandos no terminal do SQLite para verificar se a versão instalada tem suporte a FKs (*foreign keys*):
  ```
  PRAGMA foreign_keys;
  ```

#### Deve retornar `1` se o suporte estiver habilitado e `0` se não estiver.

#### Caso não esteja, insira o seguinte comando no terminal do SQLite para ativar:

  ```
  PRAGMA foreign_keys = ON;
  ```

#### Você pode rodar novamente o comando `PRAGMA foreign_keys;` para verificar novamente se o suporte está habilitado. Agora deve retornar `1`.

### Acesso ao banco de dados

* Você pode utilizar o CLI do SQLite para fazer consultas ao banco e conferir se os dados iniciais estão retornando.
* Utilize o cli do SQLite para acessar o arquivo `src/db/livraria.sqlite`: 
  `sqlite3 ./src/db/livraria.sqlite`
* Digite `.tables` para exibir as tabelas já criadas no banco:
  ```
  sqlite> .tables
  autores   editoras  livros 
  ```

* Digite `SELECT * FROM autores;` para exibir o conteúdo da tabela `autores`:
  ```
  sqlite> SELECT * FROM autores;
  1|JRR Tolkien|sul-africano|2022-06-06 19:30:55
  2|Ursula LeGuin|estadunidense|2022-06-06 19:30:55
  3|Machado de Assis|brasileira|2022-06-06 19:30:55
  sqlite> 
  ```

* Você pode testar os comandos `SELECT * FROM livros;` e `SELECT * FROM editoras;` para conferir os dados destas tabelas que já deixamos prontos para serem usados na API.

* Importante: Usaremos a API para consultar, criar, atualizar e excluir dados do banco. Não utilize o terminal do SQLite para fazer estas alterações direto nas tabelas.

### Como rodar a API

* No terminal, acesse a pasta raiz do projeto e insira o comando `npm run dev` para rodar o projeto em modo de desenvolvimento. Você deverá ver no terminal a seguinte mensagem:
  ```
  > api-js-local@1.0.0 dev
  > nodemon server.js

  [nodemon] 2.0.16
  [nodemon] to restart at any time, enter `rs`
  [nodemon] watching path(s): *.*
  [nodemon] watching extensions: js,mjs,json
  [nodemon] starting `node server.js`
  Servidor escutando em http://localhost:3000
  ```

* Os recursos da API poderão ser acessados a partir da *base URL* `http://localhost:3000`.

* Esta API está programada para ser acessada a partir de `http://localhost:3000`. Certifique-se de que não existem outros recursos ocupando a porta `3000` antes de subir o projeto.

### Endpoints

A API expõe os seguintes *endpoints* a partir da *base URL* `localhost:3000`:

`/auth`

* `POST /login`
* `POST /cadastrar`


`/livros`

* `GET /livros`
* `GET /livros/:id`
* `POST /livros`
* `PUT /livros/:id`
* `DELETE /livros/:id`


`/autores`

* `GET /autores`
* `GET /autores/:id`
* `GET /autores/:id/livros`
* `POST /autores`
* `PUT /autores/:id`
* `DELETE /autores/:id`


`/editoras`

* `GET /editoras`
* `GET /editoras/:id`
* `GET /editoras/:id/livros`
* `POST /editoras`
* `PUT /editoras/:id`
* `DELETE /editoras/:id`


`/aluguel-livro`

* `GET /aluguel-livro`
* `GET /aluguel-livro/:id`
* `POST /aluguel-livro`
* `GET /aluguel-livro/devolver/:id`
* `DELETE /aluguel-livro/:id`


`/livros-imagens`

* `GET /livros-imagens`
* `GET /livros-imagens/:id`
* `POST /livros-imagens`
* `PUT /livros-imagens/:id`
* `DELETE /livros-imagens/:id`


`/usuarios`

* `GET /usuarios`
* `GET /usuarios/:id`
* `PUT /usuarios/:id`
* `DELETE /usuarios/:id`

