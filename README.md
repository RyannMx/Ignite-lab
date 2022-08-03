<h1 align="center">
   <img src="https://user-images.githubusercontent.com/71537090/175778147-98b5c4aa-c762-43c4-8b19-751031281978.png" alt="Logo Ignite Lab" />
</h1>

<p align="center" margin-top="25px" >
  <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/Azanniel/event-platform-ignite-lab?color=00875F">

  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/Azanniel/event-platform-ignite-lab?color=00875F">

  <img alt="GitHub" src="https://img.shields.io/github/license/Azanniel/event-platform-ignite-lab?color=00875F">
</p>


![image](https://user-images.githubusercontent.com/71537090/175778135-0ec2b3ca-4f00-45bf-bd66-32d0136eb356.png)

## 🧪 Tecnologias

Esse projeto foi desenvolvido com as seguintes tecnologias:

- [React](https://reactjs.org)
- [Tailwindcss](https://tailwindcss.com)
- [Vite](https://vitejs.dev)
- [TypeScript](https://www.typescriptlang.org)
- [GraphQL](https://graphql.org/)
- [ApolloGraphQL](https://www.apollographql.com/)
- [GraphQL Codegen](https://www.graphql-code-generator.com/)

## 🔖 Layout

Você pode visualizar o layout do projeto através do link abaixo:

- [Layout](https://www.figma.com/file/ONisXOTq10lwwhPSK75xu5/Plataforma-de-evento---Ignite-Lab?node-id=38%3A930)

## ⚙️ Como executar

Para iniciar o projeto é preciso, também, ter uma conta no site [GraphCMS](https://graphcms.com/) e clonar o [Schema](https://app.graphcms.com/clone/3336ac10710646dfa04f524f6062967c?name=Ignite%20Lab%20-%20Leandro%20Azanniel)
para obter todas as colletions necessárias para executar o projeto.

Tendo uma conta e clonando o schema você já pode por meio do GraphCMS utilizar as chaves de conexão com a API. Essa chaves você vai encontrar em `Project Settings -> API Access`.

Ao acessar essa página você encontrará a `Content API` e também a `Permanent Auth Tokens`. Copie esses tokens, pois vamos introduzir em um arquivo de variável de ambiente.

### Inserindo variáveis de ambiente

1. Crie um arquivo chamado `.env.local` na raiz do projeto
2. Utilize as variáveis de exemplo que estão no arquivo `.env.example`
3. Na variável de ambiente `VITE_GRAPHCMS` cole a chave do `Content API`
4. Na variável de ambiente `VITE_GRAPHCMS_TOKEN_API_KEY` cole a chave do `Permanent Auth Tokens`
5. No arquivo `codegen.yml` cole a chave `Content API` no atributo `schema` para posteriormente gerarmos as tipagens do schema do GraphCMS

### Iniciando o projeto

Para iniciar o projeto execute os comandos abaixo:

```sh
# Instale as dependências
$ npm install --force

# Execute o codegen para gerar a tipagem dos schemas
$ npm run codegen

# Execute o projeto utilizando o vite
$ npm run dev
```

Com isso o projeto estará sendo executado na porta 3000.


## 📝 Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE.md) para mais detalhes.
