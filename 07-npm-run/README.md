# npm run

`npm run nome_do_script`

## aliases: 

run, rum, urn`

## Descrição

Isso executa um comando existente no objeto script dentro do package.json.
Se nenhum "command" for fornecido, ele listará os scripts disponíveis.

## Exemplo

Supomos que em seu package.son exista o seguinte objeto:

```json
"scripts": {
  "http-server": "http-server"
}
```

Para executar esse script pasta digitar `npm run http-server`.
