# Alura_Spring-Boot-API-REST
Curso da Alura: Spring Boot API REST: construa uma API.

# Modulo 1:

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

# Modulo 2:

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
