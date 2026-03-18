# Tutorial para a utilização da versão 7.5 do ORM Prisma

Um pequeno tutorial para explicar como usar a ultima vesão do prisma, recente a bibilioteca atualizou e muita gente enfrentou problemas com essa mudança por ser uma mudança brusca e com muitas alterações no jeito que a bibilioteca funciona

## O que mudou?

- Mudança no tratamento de pacotes, agora o prisma faz do uso do Ecma Script Modules (ESM) (import/export) ao invés de commonJS (CJS) (require/module.exports).
- Para funcionamento pleno do client, é recomendado o uso de um driver adapter dedicado para o provedor de banco de dados selecionado pelo dev (MariaDB, Postgres...)

npm init

npm install prisma@7

npm install @prisma/client@7

npm install @prisma/adapter-mariadb

npx prisma generate 

npx prisma migrate dev

