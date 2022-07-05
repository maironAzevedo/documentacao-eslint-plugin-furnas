# gerenciamento-de-estados

Esta regra avalia se uma classe faz uso de mais de um gerenciamento de estado, ou seja os react Hooks não podem ser usados em conjunto de classes e vice-versa (gerenciamentos-de-estado)

## Detalhes da regra

A análise é feita da seguinte forma: apontamos para as classes, funções e importações do código e validamos se em toda aplicação existe a declaração de *React Hooks* sendo utilizada juntamente com classes.

Exemplo de código **incorreto** para essa regra:

```js
import {useState} from 'react'
    function StateDaPagina() {
        //...
    }
    class Teste {
        this.state {
            //...
        }
        constructor() {
            //...
        }
    }
```


## Quando não usá-la

A regra só faz sentido em aplicações que possuam a arquitetura flux, ou seja, caso seu projeto utilize de funções, não há porque impedir o uso dos *React Hooks* para gerenciamento de estado das mesmas.

## Aprofunde-se no tema


