# Apenas serviço deve acessar a biblioteca FurnasRequest (acesso-a-furnasrequest)

Somente serviços podem importar a biblioteca FurnasRequest

## Detalhes da Regra

Esta regra valida se um arquivo sem ser um serviço realiza a importação da biblioteca FurnasRequest.

Exemplo de código **incorreto** da regra:

```js

import FurnasRequest from \'@furnas/frontend-framework/FurnasRequest\';

        class ProfessorStore {
            //...
        }

```

Exemplo de código **correto** da regra:

```js

import FurnasRequest from \'@furnas/frontend-framework/FurnasRequest\';
  
        class ProfessorService {
            //... 
        }

```
