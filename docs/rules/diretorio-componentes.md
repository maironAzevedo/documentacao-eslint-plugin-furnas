# Classes componentes devem estar no diretório Componentes (diretorio-componentes)

Os arquivo de componentes devem estár no diretório de pasta Componentes.

## Detalhesa da Regra

Esta regra valida se um componente está em um pasta diferente de Componentes.

Exemplo de código **incorreto** da regra:

```js

import Dispatcher from \'@furnas/frontend-framework/Dispatcher\';

        class ProfessorPage {
            //...
        }

filename: "src/Actions/professorPage.js"

```

Exemplo de código **correto** da regra:

```js

import Dispatcher from \'@furnas/frontend-framework/Dispatcher\';
  
        class ProfessorPage {
            //...
        }

filename: "src/Componentes/professorPage.js"

```
