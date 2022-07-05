# Actions só devem ser chamadas por páginas (acesso-a-actions)

As actions (Exemplo: LoginAction.js) só devem ser chamadas por páginas (Exemplo: LoginPage.js)

## Detalhes da Regra

Esta regra valida se uma action está sendo importada por um arquivo que não é uma page.

Exemplo de código **incorreto** dessa regra:

```js

import ProfessorActions from \'../../Servicos/ProfessorService\'
  
        class Professor {
  
          criar(professor) {
            ProfessorActions.criar(professor);
          }
        }

```

Exemplo de código **correto** dessa regra:

```js

import ProfessorActions from \'../../Servicos/ProfessorService\'
  
        class CadastroPage extends Component {
  
          metodo(professor) {
            ProfessorActions.criar(professor);
          }
        }

```
