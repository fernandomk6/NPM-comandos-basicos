# npm list

`npm ls nome_do_pacote`

## alias: 

list

## Descrição

Lista todos as dependencias instaladas no projeto. Pode especificar `-g` para listar
as dependencias globais.

## Exemplos

`npm ls` ou `npm list` listará todas as dependencias instaladas localmente.

`npm ls -g` ou `npm list -g` listará todas as dependencias instaladas globalmente.

## Parametros adicionais

Você pode especificar `--all` para que toda a árvore de dependencias seja listada. Ou seja
listará suas dependencias e as dependencias de suas dependencias.

Pode especificar `--json` para listar as dependencias em formato json.

Pode especificar `--long` para ter um maior espaçamento na arvore de dependencias.