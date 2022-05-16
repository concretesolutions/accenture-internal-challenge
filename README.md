# Desafio Interno Accenture

## Introdução

Este é um desafio para que possamos ver as suas habilidades como Developer (seja backend, cloud ou fullstack).

Nesse desafio você irá desenvolver uma REST API que utilizará os dados do projeto [Space Flight News](https://api.spaceflightnewsapi.net/v3/documentation), uma API pública com informações relacionadas a voos espaciais.

- Poderá também utilizar um projeto ja existente nestes moldes para fazer a entrega. (Opcional)

O projeto a ser desenvolvido por você tem como objetivo exibir os dados dos artigos, com o título, imagem (link para backend), resumo e data de publicação. 

**[SOMENTE PARA FULLSTACK]** Atente-se, ao desenvolver a aplicação front-end, para conceitos de usabilidade.

### Instruções iniciais obrigatórias

- O projeto **back-end** deverá ser desenvolvido com uma das tecnologias a seguir: **JVM Java/Kotlin/Scala | Go Lang | Python | Node.js | C# .NET Core**;
- Criar um banco de dados em memoria
- Ou banco de dados grátis **MongoDB** usando Atlas: https://www.mongodb.com/cloud/atlas 
- Ou banco de dados grátis **MySQL** no Heroku: https://elements.heroku.com/addons/jawsdb
- Ou banco de dados grátis **Postgres** no Heroku: https://elements.heroku.com/addons/heroku-postgresql;

### Modelo de Dados:

Para a definição do modelo consulte a rota [GET]/articles da API, nesta rota você pode ver a estrutura como o exemplo:

```json
{
    "id": 0,
    "featured": false,
    "title": "string",
    "url": "string",
    "imageUrl": "string",
    "newsSite": "string",
    "summary": "string",
    "publishedAt": "string",
    "launches": [
      {
        "id": "string",
        "provider": "string"
      }
    ],
    "events": [
      {
        "id": "string",
        "provider": "string"
      }
    ]
  }
```

### Back-End:

Nessa etapa você deverá construir uma API Restful com as melhores práticas de desenvolvimento, baseada na API [Space Flight News](https://api.spaceflightnewsapi.net/v3/documentation). Para isso você deve executar os passos a seguir:

**Obrigatório 1** - Você deverá desenvolver as seguintes rotas:

- `[GET]/: ` Retornar um Status: 200 e uma Mensagem "Desafio Interno Accenture - Space Flight News"
- `[GET]/articles/:`   Listar todos os artigos da base de dados, utilizar o sistema de paginação na resposta do endpoint para não sobrecarregar a REQUEST
- `[GET]/articles/{id}:` Obter a informação somente de um artigo
- `[POST]/articles/:` Adicionar um novo artigo

**Obrigatório 1** - Para alimentar o seu banco de dados você deve criar um script para armazenar os dados de todos os artigos na Space Flight News API. 

**Obrigatório 2** - Escrever Unit Test

**Diferencial 1** - Configurar Docker no Projeto para facilitar o Deploy da equipe de DevOps;

**Diferencial 2** - Descrever a documentação da API utilizando o conceito de Open API 3.0;

**Diferencial 3** - Escrever Contract Testes para os endpoints da API;

**Diferencial 4** - Escrever rotas para criar, atualizar e deletar artigos;

- `[PUT]/articles/{id}:` Atualizar um artigo baseado no `id`
- `[DELETE]/articles/{id}:` Remover um artigo baseado no `id`

### Front-End (Somente para Fullstack):

Nessa etapa você deverá desenvolver uma aplicação web para consumir a API que você criou. Você deve limitar o `request` para exibir apenas 10 resultados.

Para o desenvolvimento você pode utilizar algum framework CSS ou criar seu proprio estilo.

**Obrigatório 1** - Desenvolver a funcionalidade do buscador para que seja possível listar artigos que contenham as palavras no título;

**Obrigatório 2** - Desenvolver a funcionalidade para ordenar os artigos por data, da mais antiga para a mais nova e da mais nova para a mais antiga;

**Obrigatorio 3** - Desenvolvar a funcionalidade de criar artigos.

**Diferencial 1** Desenvolver as funcionalidades para atualizar e remover artigos.

**Diferencial 2** Escrever Unit Tests ou E2E Test. Escolher a melhor abordagem e biblioteca;

**Diferencial 3** Configurar Docker no Projeto para facilitar o Deploy da equipe de DevOps;

## Readme do repositório

- Deve conter o título do projeto
- Uma descrição sobre o projeto em frase
- Deve conter uma lista com linguagem, framework e/ou tecnologias usadas
- Como instalar e usar o projeto (instruções)
- Não esqueça o [.gitignore](https://www.toptal.com/developers/gitignore)

## Finalização e instruções para a apresentação

Avisar sobre a finalização e enviar para correção.

1. Verifique se o README está bom e faça o PR;
3. Coloque o link do PR no email para o RH;
4. Envie e aguarde as instruções para seguir no processo. Sucesso e boa sorte. =)
