# 🏎️ TurboGarage

O **TurboGarage** é uma aplicação web desenvolvida em **Java** com **Spring Boot** para o gerenciamento de serviços, cadastros e usuários de uma oficina mecânica/garage. O sistema oferece autenticação, controle de acesso administrativo e uma interface web intuitiva para gerenciamento de dados.

---

## 🚀 Funcionalidades

- **Autenticação & Sessões:** Login e logout seguros com controle de permissões de acesso (Interceptores Spring).
- **Gestão de Cadastros:** Criação, listagem e gerenciamento de registros e serviços.
- **Painel Administrativo:** Restrição de rotas e funcionalidades exclusivas para administradores.
- **Carga de Dados Iniciais:** Inicialização de banco de dados com usuários e registros padrão ao subir a aplicação.
- **Interface Web Integrada:** Páginas interativas construídas com HTML5, CSS3 e JavaScript.

---

## 🛠️ Tecnologias Utilizadas

- **Back-end:** Java 17+, Spring Boot, Spring MVC, Spring Data JPA.
- **Banco de Dados:** H2 Database / MySQL (SQL customizado `schema.sql` e `banco.sql`).
- **Front-end:** HTML5, CSS3, JavaScript (Fetch API).
- **Gerenciamento de Dependências:** Apache Maven.

---

## 📁 Estrutura do Projeto

```text
turbogarage/
├── src/
│   ├── main/
│   │   ├── java/com/example/demo/
│   │   │   ├── config/          # Interceptores e inicialização de dados
│   │   │   ├── controller/      # Controladores REST e de navegação
│   │   │   ├── dto/             # Objetos de Transferência de Dados (DTOs)
│   │   │   ├── model/           # Entidades JPA (Usuario, Cadastro)
│   │   │   ├── repository/     # Interfaces de acesso ao banco
│   │   │   ├── service/        # Regras de negócio
│   │   │   └── util/           # Utilitários (criptografia de senha, etc.)
│   │   └── resources/
│   │       ├── static/          # Páginas HTML, CSS, Imagens e JavaScript
│   │       ├── application.properties
│   │       └── schema.sql
├── banco.sql
└── pom.xml
