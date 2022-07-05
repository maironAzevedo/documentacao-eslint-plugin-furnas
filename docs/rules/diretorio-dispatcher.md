# O arquivo Dispatcher.js deve estar na pasta Dispatcher (diretorio-dispatcher)

Deve haver na aplicação um diretório chamado _Dispatcher_ para armazenar o arquivo _Dispatcher.js_

## Detalhes da Regra

Esta regra valida se o arquivo Dispatcher.js está dentro de uma pasta chamada Dispatcher, caso não, haverá erro.

Exemplo de código **incorreto** da regra:

```js
filename: "src/Actions/Dispatcher.js"
```

Exemplo de código **correto** da regra:

```js

filename: "src/Dispatcher/Dispatcher.js"

```