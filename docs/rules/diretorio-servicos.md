# Arquivos de serviço devem estar armazenados numa pasta Servicos (diretorio-servicos)

O diretório *Servicos* deve conter apenas arquivos de serviço

## Rule Details

Essa regra valida se o diretório *Servicos* possui apenas arquivos de serviço.

Exemplo de código **incorreto** da regra:

```js

filename: "src/Servicos/ProfessorActions.js"

```

Exemplo de código **correto** da regra:

```js

filename: "src/Servicos/professorService.js",

```