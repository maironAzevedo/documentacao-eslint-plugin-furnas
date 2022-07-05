# As classes Actions devem estar armazenadas dentro de uma pasta &#39;Actions&#39; (diretorio-actions)

Todas as Actions devem estar localizadas dentro da paste "Actions".

## Detlhes da Regra

Esta regra valida se uma Action está dentro de uma pasta cujo nome é diferente de Actions.

Exemplo de código **incorreto** da regra:

```js

 import Dispatcher from \'@furnas/frontend-framework/Dispatcher\';

        class ProfessorActions {

            criar(professor) {}
        }

filename: "src/Services/ProfessorActions.js"

```

Exemplo de código **correto** da regra:

```js

 import Dispatcher from \'@furnas/frontend-framework/Dispatcher\';
  
        class ProfessorActions {
  
          criar(professor) {}
        }

filename: "src/Actions/professorActions.js"

```
