# Os arquivos de assets devem estar no subdiretório correto (diretorio-assets)

O arquivo asset deve estar no subdiretório Assets/*nome do tipo de aquivo*/*arquivo com extensão correta*.

## Detalhes da Regra

Os arquivos de assets devem estar nas pastas de acordo com sua extensão corretamente.

Exemplo de código **incorreto** da regra:

```js

"src/Componentes/Assets/fonts/assetTeste.css"
"src/Componentes/Assets/assetTeste.css"
"src/Componentes/Assets/fonts/assetTeste.txt"

```

Exemplo de código **correto** da regra:

```js

"src/Componentes/Assets/assetTeste.js"
"src/Componentes/Assets/fonts/assetTeste.eot"
"src/Componentes/Assets/css/assetTeste.css"

```
