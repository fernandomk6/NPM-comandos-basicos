# npm start

```
npm start [-- <args>]
```

## Descrição

Isso executa um comando predefinido especificado na "start" propriedade do objeto de um pacote "scripts".

Se o "scripts" objeto não definir uma "start" propriedade, o npm será executado node server.js.

Observe que isso é diferente do comportamento do node padrão de executar o arquivo especificado no "main" 
atributo de um pacote ao evocar com node.

A partir de npm@2.0.0, você pode usar argumentos personalizados ao executar scripts. 
Consulte npm run-script para mais detalhes.

## Exemplo

```
{
  "scripts": {
    "start": "node foo.js"
  }
}

---

npm start

> npm@x.x.x start
> node foo.js

(foo.js output would be here)
```