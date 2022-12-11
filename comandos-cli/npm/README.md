# NPM Comando

## Descrição

npm é o gerenciador de pacotes para a plataforma Node JavaScript. 
Ele coloca os módulos no lugar para que o node possa encontrá-los e gerencia 
os conflitos de dependência de forma inteligente.

É extremamente configurável para suportar uma variedade de casos de uso. 
Mais comumente, você o usa para publicar, descobrir, instalar e desenvolver programas em node.

Execute npm help para obter uma lista de comandos disponíveis.

## Basicos

| Comandos | Descrição | 
| --- | --- | 
| npm install | install all the dependencies in your project | 
| npm install `<foo>` |  add the `<foo>` dependency to your project | 
| npm test | run this project's tests | 
| npm run `<foo>` | run the script named `<foo>` | 
| npm `<command>` -h | quick help on `<command>` | 
| npm -l | display usage info for all commands | 
| npm help `<term>` | search for help on `<term>` (in a browser) | 
| npm help npm | more involved overview (in a browser) | 
| npm list | lista todas as dependencias instaladas |
| npm list -g | lista todas as dependecias instaladas globalmente |
| npm remove `<foo>` | remove uma dependencia |
| npm remove -g `<foo>` | remove uma dependecia global |


## Todos os comandos

- access
- adduser
- audit
- bugs
- cache
- ci
- completion
- config
- dedupe
- deprecate
- diff
- dist-tag
- docs
- doctor
- edit
- exec
- explain
- explore
- find-dupes
- fund
- get
- help
- hook
- init
- install
- install-ci-test
- install-test
- link
- ll
- login
- logout
- ls
- org
- outdated
- owner
- pack
- ping
- pkg
- prefix
- profile
- prune
- publish
- query
- rebuild
- repo
- restart
- root
- run-script
- search
- set
- shrinkwrap
- star
- stars
- start
- stop
- team
- test
- token
- uninstall
- unpublish
- unstar
- update
- version
- view
- whoami

## Diretórios de instalação 

Em particular, o npm tem dois modos de operação:

- modo local: 

O npm instala pacotes no diretório do projeto atual, cujo padrão é o 
diretório de trabalho atual. Os pacotes são instalados em ./node_modules e 
os compartimentos em ./node_modules/.bin.

- modo global: 

npm instala pacotes no prefixo de instalação em $npm_config_prefix/lib/node_modules e 
bins em $npm_config_prefix/bin.

*O modo local é o padrão. Use -gou --globalem qualquer comando para executar no modo global*.

## O package.json

Este documento é tudo o que você precisa saber sobre o que é necessário em seu arquivo package.json. 
Deve ser JSON real, não apenas um literal de objeto JavaScript.

Muito do comportamento descrito neste documento é afetado pelas definições de 
configuração descritas em config.
