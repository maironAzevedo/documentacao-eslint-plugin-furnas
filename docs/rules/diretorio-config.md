# O diretório Config deve conter apenas arquivos de configuração (diretorio-config)

O diretório Config deve conter apenas arquivos de configuração.

## Detalhes da Regra

Esta regra valida se algum arquivo que não é de configuração esta dentro do diretório Config.

Exemplo de código **incorreto** da regra:

```js

filename: "src/Config/error.js"

```

Exemplo de código **correto** da regra:

```js

filename: "src/Config/routes.js"

```
