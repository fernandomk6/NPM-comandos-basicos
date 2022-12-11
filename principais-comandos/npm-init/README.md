# npm init

```
npm init <package-spec> (same as `npx <package-spec>)
npm init <@scope> (same as `npx <@scope>/create`)

aliases: create, innit
```

npm init `<initializer>` pode ser usado para configurar um pacote npm novo ou existente.

initializer neste caso, é um pacote npm chamado `create-<initializer>`, que será instalado por npm-exec, 
e então terá seu bin principal executado - presumivelmente criando ou atualizando package.json e 
executando quaisquer outras operações relacionadas à inicialização.

O comando init é transformado em uma npm exec operação correspondente da seguinte forma:

```
npm init foo -> npm exec create-foo
npm init @usr/foo -> npm exec @usr/create-foo
npm init @usr -> npm exec @usr/create
npm init @usr@2.0.0 -> npm exec @usr/create@2.0.0
npm init @usr/foo@2.0.0 -> npm exec @usr/create-foo@2.0.0
```

Se o inicializador for omitido (apenas chamando npm init), o init retornará ao comportamento 
legado do init. Ele fará várias perguntas e, em seguida, escreverá um package.json para você. 
Ele tentará fazer suposições razoáveis ​​com base nos campos existentes, dependências e opções selecionadas. 
É estritamente aditivo, portanto manterá todos os campos e valores que já foram definidos. 
Você também pode usar -y/ --yes para pular o questionário completamente. 
Se você passar --scope, ele criará um pacote com escopo.

## Exemplos

Crie um novo projeto baseado em React usando create-react-app:

```
$ npm init react-app ./my-react-app
```

Crie um novo esmpacote -compatível usando create-esm:
 
```
$ mkdir minha-esm-lib && cd minha-esm-lib 
$ npm init esm --sim
```

Gere um package.json simples e antigo usando init herdado:

```
$ mkdir meu-npm-pkg && cd meu-npm-pkg 
$ git calor
$ npm init
```

Gere-o sem que ele faça perguntas:

```
$ npm init -y
```
