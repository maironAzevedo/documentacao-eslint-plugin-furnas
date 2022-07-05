# Somente Actions devem importar de Serviço (acesso-a-servicos)

Somente arquivos Actions podem importar Serviços.

## Detalhes da Regra

Esta regra valida se algum Serviço é importado por um arquivo que não é Action.

Exemplo de código **incorreto** da regra:

```js

import ProfessorService from \'../../Servicos/ProfessorService\';
  
        class ProfessorStore {
  
          criar(professor) {
            ProfessorService.criar(professor);
          }
        }

```

Exemplo de código **correto** da regra:

```js

import ProfessorService from \'../../Servicos/ProfessorService\';
  
        class ProfessorActions {
  
          criar(professor) {
            ProfessorService.criar(professor);

          }
        }

```
