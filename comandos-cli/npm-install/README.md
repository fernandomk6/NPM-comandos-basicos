# npm install

```
npm install [<package-spec> ...]

aliases: add, i, in, ins, inst, insta, instal, isnt, isnta, isntal, isntall
```

## Descrição

Este comando instala um pacote e todos os pacotes dos quais ele depende. 
Se o pacote tiver um package-lock, ou um arquivo npm shrinkwrap, ou um 
arquivo yarn lock, a instalação das dependências será conduzida por ele, 
respeitando a seguinte ordem de precedência:

Um pacote é:

- a) uma pasta contendo um programa descrito por um package.json arquivo
- b) um tarball gzipado contendo (a)
- c) uma url que resolva para (b)
- d) a `<name>@<version>` que é publicado no registro (ver registry) com (c)
- e) a `<name>@<tag>` (ver npm dist-tag) que aponta para (d)
- f) a `<name>` que tem uma tag "mais recente" que satisfaz (e)
- g) a `<git remote url>` que resolve para (a)

## Production e devDependencies

Com o --production sinalizador (ou quando a NODE_ENV variável de ambiente 
estiver definida como production), o npm não instalará os módulos listados em devDependencies. 
Para instalar todos os módulos listados em ambos dependencies e devDependencies quando 
NODE_ENV a variável de ambiente estiver definida como production, você pode 
usar --production=false.
