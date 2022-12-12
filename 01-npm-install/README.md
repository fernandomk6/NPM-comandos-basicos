# npm install

- `npm install nome_do_pacote` ou:
- `npm install nome_do_pacote@versao`

## aliases: 

`install` pode ser substituido por qualquer um desses termos:

add, i, in, ins, inst, insta, instal, isnt, isnta, isntal, isntall

## Descrição

Este comando instala um pacote e todos os pacotes dos quais ele depende.

## Production

Com o `--production` argumento, o npm **não** instalará os módulos listados em devDependencies. 

Exemplo: `npm install --production`

Para instalar todos os módulos listados em ambos dependencies e devDependencies ou pacote especifico
use:

- `npm install `: Para instalar todos as dependencias listadas no package.json e remover as não listadas
- `npm install package_name`: Para instalar apenas o pacote especifico.

## Instalando pacote como devDependences

Para instalar um pacote como devDependeces use o argumento `--save-dev` ou `-D`

`npm install typescript --save-dev` ou `npm install typescript -D` para dependencias de desenvolvimento.

`npm install react --save-prod`, `npm install react -P` ou simplesmente `npm install react`, para
dependencias de produção.

- `-D` ou `--save-dev` para dependencias de desenvolvimento
- `-P` ou `--save-prod` para dependencias de produção

## Pacotes globais

Também é possível instalar pacotes globais ou locais.

Pacotes locais ficarão armazenados na pasta `node_modules` do diretório atual, já os globais 
ficarão armazenados na pasta `C:\Users\seu_usuario\AppData\Roaming\npm`.

Por padrão o comando `install` irá instalar as dependencias localmente. Ou seja, as dependencias
serão instaladas dentro da pasta node_modules que está dentro da pasta aonde foi executado o comando.
Caso a node_modules não exista, ela será criada pelo npm.

Para instalar um pacote globalmente utilize o argumento `-g` no comando `install`.

`npm install http-server -g`.

Pacotes instalados globalmente poderão ser executados de qualquer local de sua máquina.
Os pacotes locais só poderão ser executados dentro da pasta aonde está a pasta node_modules.
