# Projeto Blog Pessoal - Bootcamp Generation

Resumo: criação de um projeto de blog pessoal utilizando Spring no Back-end e estilizando o Front-end com React.


## Primeira Etapa

Objetivo: modelar e implementar o banco de dados e criar o projeto Spring no Spring Initializer.

Descrição: 
1. Criação do DER do banco de dados db_blogpessoal.
2. Criação de 4 tabelas: tb_categorias, tb_produtos, tb_temas e tb_postagens.
3. Criação do projeto no Spring Initializr. Dependências utilizadas: Spring WEB, Spring dev tools, Spring data JPA, MySQL driver e validation.
4. Configuração do arquivo application.properties para conectar com o Banco de dados.
5. Criação das Classes Model Postagem e Tema.
6. Criação dos atributos estabelecidos na DER.
7. Criação dos métodos get and set.
8. Criação da Interface Repository CategoriaRepository.

## Segunda Etapa

Objetivo: criar o CRUD do projeto Spring.

Descrição:
1. Criação das Classes Controller PostagemController e TemaController.
2. Criação dos métodos básicos do CRUD: findAll(), findById(), post(), pull() e delete().
3. Criação das Interfaces Repository PostagemRepository e TemaRepository.
4. Criação dos métodos específicos: findAllByTituloContainingIgnoreCase() e findAllByDescricaoContainingIgnoreCase ().
5. Testes das API's no Insomnia.

## Terceira Etapa

Objetivo: colocar CRUD com relacionamento do projeto Spring.

Descrição:
1. Criação da Relação OneToMany na Classe Model Tema com a Classe Model Postagem.
2. Criação da Relação ManyToOne na Classe Model Postagem com a Classe Model Tema.
3. Testes das API's no Insomnia.

## Quarta Etapa

Objetivo: implementação do Spring Security.

Descrição: 
1. Adição das dependências de security na pom.
2. Criação das Classes Model Usuario e UsuarioLogin.
3. Criação dos atributos.
4. Criação dos métodos get and set.
5. Criação da Classe Controller UsuarioController.
6. Criação dos métodos básicos do CRUD: findAll(), findById(), post(), pull() e delete().
7. Criação da Interface Repository UsuarioRepository.
8. Criação do método específico: findByUsuario().
9. Criação do package security com as devidas classes: BasicSecurityConfig, JwtAuthFilter, JwtService, UserDetailsImp, UserDetailsServiceImpl.
10. Criação do package service com a classe UsuarioService.
11. Testes das API's no Insomnia.

## Quinta Etapa

Objetivo: implementação do teste de software JUnit 5.

Descrição: 
1. Atualização da dependência spring-test no arquivo pom.xml para não utilizar as versões antigas do JUnit.
2. Criação da source folder resources em src/test.
3. Criação do arquivo application.properties em src/test/resources.
4. Configuração do banco de dados de teste no arquivo application.properties.
5. Criação do teste para a classe Controller UsuarioControllerTest.
6. Testes no JUnit.

## Sexta Etapa

Objetivo: criação e implantação de aplicações web.

Descrição: 
1. Inserção da Dependência: Spring Docs.
2. Configuração do Spring Docs no arquivo application.properties na Source Folder src/main/resources.
3. Criação da Camada Configuration no pacote principal da aplicação.
4. Na Camada Configuration, criação da Classe SwaggerConfig e configuraçãp dos dados pessoais (Nome, Email, Github e etc).
5. Na Camada Model, do pacote principal, na Classe Usuario, inserção da Anotação @Schema no atributo usuario.
6. Execução da aplicação e teste do API no Navegador da Internet, através do link: http://localhost:8080.
7. Verificação da a página do Swagger.
8. Testes na aplicação com Insomnia antes de efetuar o Deploy.
9. Inserção da dependência: Banco de dados PostgreSQL.
10. Configuração dos Profiles de acesso ao Banco de dados (DEV e PROD).
11. Configuração do perfil PROD como padrão, para conectar ao Banco de dados na nuvem através das variáveis de ambiente.
12. Criação do arquivo Dockerfile na raiz do projeto e configuração do Docker para gerar a aplicação executável (JAR) e a imagem da aplicação.
13. Envio das atualizações para o repositório remoto da aplicação no Github.
14. Criação da conta no Render.
15. Criação do Banco de dados PostgreSQL no Render.
16. Criação do Webservice no Render.
17. Resolução do problema de dependências e do BOM na classe UsuarioControllerTest.
18. Configuração do Webservice para acessar o Repositório no Github.
19. Inserção das variáveis de ambiente no Webservice para conectar com o Banco de dados na Nuvem.
20. Efetuação do Deploy.
21. Testes das APIs na nuvem com o Insomnia.
