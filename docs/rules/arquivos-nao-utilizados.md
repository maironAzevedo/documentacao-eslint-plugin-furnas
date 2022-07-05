# Não devem ser criados arquivos não utilizados pela aplicação (arquivos-nao-utilizados)

Não deve existir na aplicação arquivos criados que não são utilizados em nenhum outro arquivo.

## Detalhe da Regra

Esta regra valida se algum arquivo não é utilizado em nenhum outro arquivo da aplicação.

Exemplo de código **incorreto** da regra:

```js

Esta regra acusará erro se o arquivo não for importado por nenhum outro arquivo da aplicação.

```

Exemplo de código **correto** da regra:

```js

A regra não acusará erro se todos os arquivos criados na aplicação forem utilizados de alguma forma por outro(os) arquivo(os).

```
