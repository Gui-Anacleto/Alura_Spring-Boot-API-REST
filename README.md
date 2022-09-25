# Alura_Spring-Boot-API-REST
Curso da Alura: Spring Boot API REST: construa uma API.

# Modulo 1: Introdução ao Spring boot

Classe MAIN roda o projeto.

@Controller - Serve para o spring encontrar e determinar.

@RequestMapping("URL") -  Vai sobre o metodo, para determinar a URL.

@ResponseBody - Usado para devolver a informação do método no corpo do navegador.

    Um resumo da história e evolução do Spring;

    Que, para criar um projeto com Spring Boot, utilizamos o Spring Initialzr, através do site https://start.spring.io;

    Como importar um projeto com Spring Boot na IDE Eclipse;

    Como é o pom.xml de uma aplicação que utiliza o Spring Boot;

    Que, para inicializar o projeto com Spring Boot, devemos utilizar a classe com o método main;

    Que, para criar um controller, utilizamos as anotações @Controller e @RequestMapping.

# Modulo 2: Publicando Endpoints

@RestController - substitui o @Controller e tira  necessidade de ter que colcoar o @ResponseBody sempre.

## No arquivo POM.XML
Adicionar nas dependencias: 

<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-devtools</artifactId>
  <scope>runtime</scope>
</dependency>

Essa dependenvia vai adicionar mais algumas ferramentes inclusive o autorestart do servidor.

    Sobre a API que desenvolveremos ao longo do curso e sobre as classes de domínio dela;

    Que, para um método no controller não encaminhar a requisição a uma página JSP, ou Thymeleaf, devemos utilizar a anotação @ResponseBody;

    Que o Spring, por padrão, converte os dados no formato JSON, utilizando a biblioteca Jackson;

    Que, para não repetir a anotação @ResponseBody em todos os métodos do controller, devemos utilizar a anotação @RestController;

    Que, para não precisar reiniciar manualmente o servidor a cada alteração feita no código, basta utilizar o módulo Spring Boot DevTools;

    Que não é uma boa prática retornar entidades JPA nos métodos dos controllers, sendo mais indicado retornar classes que seguem o padrão DTO (Data Transfer Object);

    Os principais conceitos sobre o modelo arquitetural REST, como recursos, URIs, verbos HTTP, Representações e comunicação stateless.

# Modulo 3: Usando Spring Data

    Para utilizar o JPA no projeto, devemos incluir o módulo Spring Boot Data JPA, que utiliza o Hibernate, por padrão, como sua implementação;

    Para configurar o banco de dados da aplicação, devemos adicionar as propriedades do datasource e do JPA no arquivo src/main/resources/application.properties;

    Para acessar a página de gerenciamento do banco de dados H2, devemos configurar o console do H2 com propriedades no arquivo src/main/resources/application.properties;

    Para mapear as classes de domínio da aplicação como entidade JPA, devemos utilizar as anotações @Entity, @Id, @GeneratedValue, @ManyToOne, @OneToMany e @Enumerated;

    Para que o Spring Boot popule automaticamente o banco de dados da aplicação, devemos criar o arquivo src/main/resources/data.sql;

    Para criar um Repository, devemos criar uma interface, que herda da interface JPARepository do Spring Data JPA;

    Para criar consultas que filtram por atributos da entidade, devemos seguir o padrão de nomenclatura de métodos do Spring, como por exemplo findByCursoNome;

    Para criar manualmente a consulta com JPQL, devemos utilizar a anotação @Query;
