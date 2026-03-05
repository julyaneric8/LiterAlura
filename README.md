# 📚 LiterAlura

Projeto desenvolvido como desafio da **Alura**, com o objetivo de construir um catálogo de livros utilizando **Java**, **Spring Boot**, **PostgreSQL** e consumo de **API REST**.

A aplicação permite buscar livros em uma API externa, salvar os dados em um banco de dados relacional e realizar diferentes consultas sobre os livros e autores armazenados.

---

# 🚀 Objetivo do Projeto

O projeto LiterAlura foi criado para praticar conceitos importantes de desenvolvimento backend, incluindo:

* Consumo de API REST
* Persistência de dados com Spring Data JPA
* Integração com banco de dados PostgreSQL
* Modelagem de entidades e relacionamentos
* Criação de consultas utilizando repositórios JPA

A aplicação funciona através de um menu no terminal que permite ao usuário interagir com o sistema.

---

# 🧰 Tecnologias Utilizadas

* **Java**
* **Spring Boot**
* **Spring Data JPA**
* **PostgreSQL**
* **Maven**
* **API Gutendex**

---

# 🌐 API Utilizada

A aplicação utiliza a API pública **Gutendex**, que contém dados de mais de 70 mil livros do Projeto Gutenberg.

Exemplo de busca:

```
https://gutendex.com/books/?search=nome_do_livro
```

Os dados retornados incluem:

* Título do livro
* Autor
* Idioma
* Número de downloads

---

# 🗂 Estrutura do Projeto

```
literalura
│
├── src
│   ├── main
│   │   ├── java
│   │   │   └── br.com.alura.literalura
│   │   │       ├── principal
│   │   │       ├── model
│   │   │       ├── repository
│   │   │       └── service
│   │   │
│   │   └── resources
│   │       └── application.properties
│   │
│   └── test
│
└── pom.xml
```

### 📂 Pacotes

**principal**
Classe principal responsável pela execução do programa e interação com o usuário.

**model**
Contém as entidades da aplicação, como:

* Autor
* Livro

**repository**
Interfaces responsáveis pela comunicação com o banco de dados utilizando Spring Data JPA.

**service**
Contém a lógica de negócio da aplicação, incluindo consumo da API e processamento dos dados.

---

# ⚙️ Funcionalidades do Sistema

O sistema possui um menu interativo com as seguintes opções:

### 1️⃣ Buscar livro pelo título

Busca um livro na API Gutendex e salva no banco de dados.

### 2️⃣ Listar livros registrados

Exibe todos os livros armazenados no banco.

### 3️⃣ Listar autores registrados

Mostra os autores cadastrados e seus respectivos livros.

### 4️⃣ Listar autores vivos em determinado ano

Permite informar um ano e retorna autores que estavam vivos naquele período.

### 5️⃣ Listar livros por idioma

Lista livros armazenados no banco de acordo com o idioma selecionado.

Idiomas disponíveis:

* PT (Português)
* EN (Inglês)
* ES (Espanhol)
* FR (Francês)

---

# 🗄 Configuração do Banco de Dados

No arquivo `application.properties`, configure a conexão com o PostgreSQL:

```
spring.datasource.url=jdbc:postgresql://localhost:5432/literalura
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.format-sql=true
```

O Hibernate irá criar automaticamente as tabelas necessárias no banco de dados.

---

# ▶️ Como Executar o Projeto

1. Clone o repositório

```
git clone https://github.com/seu-usuario/literalura.git
```

2. Abra o projeto em uma IDE (IntelliJ ou Eclipse)

3. Configure o banco de dados PostgreSQL

4. Execute a classe principal do projeto

5. Utilize o menu no terminal para interagir com o sistema

---

# 📖 Aprendizados do Projeto

Durante o desenvolvimento deste projeto foi possível praticar:

* Arquitetura básica com Spring Boot
* Consumo de APIs externas
* Conversão de JSON para objetos Java
* Persistência de dados com JPA
* Relacionamentos entre entidades
* Consultas personalizadas em banco de dados

---

# 📌 Possíveis Melhorias

Algumas funcionalidades extras que podem ser implementadas:

* Top 10 livros mais baixados
* Estatísticas sobre downloads
* Busca de autor por nome
* Filtros mais avançados de livros

---

# 👨‍💻 Autor

Projeto desenvolvido como parte do desafio **LiterAlura** da plataforma **Alura**.
