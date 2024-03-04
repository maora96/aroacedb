# The AroAce Database

## O Projeto

A AroAce Database foi meu primeiro projeto pós-bootcamp. Começou apenas para testar meus conhecimentos em algo real, mas com o passar dos anos fui modificando-o pouco a pouco para refletir meus novos conhecimentos.

A AroAce Database consiste uma webapp de armazenamento de personagens arromânticos e/ou assexuais na literatura especulativa. A ideia é que seja possível:

- Buscar por um personagem (busca simples)
- Buscar por personagens baseado em filtros (busca avançada)
- Ver personagens recentemente adicionados
- Favoritar personagem
- Recomendar um personagem para o admin
- Recomendar um livro para um personagem já existente para o admin
- Como admin, aceitar ou reprovar personagens
- Como admin, aceitar ou reprovar livros
- Como admin, editar ou deletar personagens
- Como admin, editar ou deletar livros
- Como admin, permitir ou não que usuários sugiram livros e personagens

Essa seria a terceira versão do backend desse projeto, adaptado da segunda.

- [Primeira versão (2021).](https://github.com/maora96/aroacedb-back)
- [Segunda versão (2023).](https://github.com/maora96/aroacedb-back-v2)

E a segunda versão do front-end.

- [Primeira versão (2021).](https://github.com/maora96/aroacedb-front)
- [Segunda versão (2023).](https://github.com/maora96/aroacedb-front-v2/tree/feat/tailwind-branch/src)

Atualmente a versão online usa o front end 1.0 e o back end 2.0. Minha ideia é dar uns últimos toques nessa nova versão, construída para o teste da Incentive.me, e eventualmente colocá-la online.

## Pontos de discussão

- Modelagem do banco de dados (personagens & livros).
- Filtragem
- Clean Architecture
- React Query
- Acessibilidade
- Hospedagem pelo Digital Ocean
- Tailwind vs Ant Design (vs MUI?)

## Instalação

```bash
$ cd api

$ npm install
```

Criar um arquivo na pasta `api/src/utils` chamada constants.ts para exportar o secret do JWT

```ts
export const jwtConstants = {
  secret: "secretjwt",
};
```

## Rodando a app

```bash
$ cd api

# development
$ npm run start:dev

# production
$ npm run start:prod
```

## Test

```bash
# unit tests
$ npm run test
```
