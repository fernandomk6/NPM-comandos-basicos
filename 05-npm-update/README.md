# npm update

`npm update nome_do_pacote`

## aliases: 

up, upgrade, udpate

## Descrição 

Esse comando irá atualizar o pacote especificado ou todos os pacotes.
Se o argument `-g` for especificado, todos os pacotes gloais serão atualizados.

A atualização é feita com base nas versões que estão especificadas no package.json.

```json
"dependencies": {
  "nodemon": "^1.15.1",
  "react": "18.2.0"
}
```

A dependencia nodemon poderá ser atualizada para qualquer versão compativel com a 1.15.1.
Já a dependencia react não poderá ser atualizada, pois o json especifica que a versão deve ser 
exatamente a 18.2.0.

## Tabela de condições de dependencias

- `version`: Exatamente a versão especificada
- `>version`: Qualquer versão maior que `version`
- `>=version`: Qualquer versão maior ou igual a `version`
- `<version`: Qualquer versão menor que `version`
- `<=version`: Qualquer versão menor ou igual a `version`
- `~version`: Aproximadamente `version`
- `^version`: Compativel com a versão `version`
- `1.2.x`: Qualquer vesão entre `1.2.0` e `1.2.999...` mas não `1.2.3`
- `*`: Qualquer versão

## Selecionando versão a ser atualizada

Ao executar o comando `npm outdated` será retornado uma lista das dependencias locais desatualizadas.
A versão terá 3 campos.

1. Current: versão atualmente instalada
2. Wanted: versão máxima que satisfaz a condição no package.json propriedade dependences
3. Latest: versão mais recente disponível no registro npm para o pacote.

O comando `npm update` irá atualizar todas as dependencias para a versão mais alta suportada,
pela condição do package.json (wanted).

Caso a versão wanted não seja a latest, e você deseja atualizar para a versão mais recente você
tem duas opções:

1. Alterar a condição da versão da dependecia no package.json manualmente para que a wanted seja
igual a latest. Por exemplo: `"dependencies": { "react": ">18.1.1" }`. Dessa forma a versão
wanted será a versão maior disponivel depois da 18.1.1.

2. Instalar novamente o pacote, usando `@latest`. Exemplo: `npm install react@latest`
