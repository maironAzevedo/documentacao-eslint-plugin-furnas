# Apenas Actions e Stores importam dispatcher (acesso-a-dispatcher)

Somente classes Actions e Store devem importar o Dispatcher.

## Detalhes da Regra

Esta regra valida se o Dispatcher está sendo importado por um arquivo que não é Action ou Store.

Exemplo de código **incorreto** da regra:

```js

import Dispatcher from \'@furnas/frontend-framework/Dispatcher\';

        class ProfessorService {
            //...
        }

```

Exemplo de código **correto** da regra:

```js

import Dispatcher from \'@furnas/frontend-framework/Dispatcher\';
  
        class ProfessorActions {
  
          criar(professor) {
            //...
          }
        }

----------------------------------------------

import Dispatcher from \'@furnas/frontend-framework/Dispatcher\';
  
        class ProfessorStore {
            //...
        }

```
