# Projeto NestJS com Prisma e Validação de Autenticação

Este projeto é um exemplo básico de uma API utilizando NestJS com Prisma, validação de entrada e autenticação via JWT (JSON Web Token).

## Sumário

- [Instalação](#instalação)
- [Configuração](#configuração)
- [Executar](#executar)
- [Endpoints](#endpoints)
- [Autenticação](#autenticação)

## Instalação

Para começar, clone este repositório e instale as dependências:

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
npm install
```

## Configuração

Crie um arquivo .env na raiz do projeto e configure as variáveis de ambiente necessárias, incluindo o token de autenticação

## Executar

Suba o container do banco de dados com Docker:

```bash
docker-compose up -d
```

Execute as migrations do Prisma para configurar o banco de dados:

```bash
npx prisma migrate dev
```

Inicie a aplicação:

```bash
npm run start:dev
```

## Endpoints

Os endpoints disponíveis podem ser acessados a partir do arquivo api.http utilizando a extensão REST Client do VS Code.

## Autenticação

Todas as requisições devem incluir o cabeçalho X-Api-Token com o valor do token definido no .env.


