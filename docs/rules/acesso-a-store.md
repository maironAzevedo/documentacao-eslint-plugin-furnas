# Somente páginas devem consumir Stores (acesso-a-store)

As Stores são observadas pelos View Components.

## Detalhes da Regra

Esta regra valida se algum arquivo que não é page realiza a importação e uso de uma Store.

Exemplo de código **incorreto** da regra:

```js

import ProfessorStore from \'../../Store/ProfessorStore\';
  
        class Professor {
  
          criar(professor) {
            ProfessorStore.on('CHANGE', verificaErro());
          }
        }

```

Exemplo de código **correto** da regra:

```js

import ProfessorStore from \'../../Store/ProfessorStore\';
        
        class CadastroPage extends Component {

          constructor(props) {
            super(props);
          };
        
          componentDidMount() {
            ProfessorStore.on('CHANGE', verificaErro());
          }
        }

```
