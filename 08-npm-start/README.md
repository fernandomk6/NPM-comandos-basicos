# npm start

`npm start`

## Descrição

Executará o script `start` especificado no objeto scripts dentro do package.json.

Se o "scripts" objeto não definir uma "start" propriedade, o npm será executado node server.js.

## Exemplo

```json
{
  "scripts": {
    "start": "node foo.js"
  }
}
```

Esse script pode ser executado usando o `npm start`.