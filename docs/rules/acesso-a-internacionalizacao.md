# O programa deve possuir a biblioteca de internacionalização i18n (acesso-a-internacionalizacao)

É necessário o uso da biblioteca i18next para a centralização de textos no projeto, de modo a não existir textos hardcoded.

## Detalhes da Regra

Esta regra valida se a aplicação faz uso da biblioteca i18next.

Exemplo de código **incorreto** da regra:

```js

A regra acusará erro somente se em nenhum arquivo da aplicação a biblioteca i18next for importada.

```

Exemplo de **código** correto da regra:

```js

Para que a regra não acuse erro, é necessário conter o código abaixo em pelo menos um arquivo da aplicação:

import i18n from 'i18next';

```
