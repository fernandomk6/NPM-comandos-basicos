# npm update

```
npm update [<pkg>...]

aliases: up, upgrade, udpate
```

## Descrição 

Este comando atualizará todos os pacotes listados para a versão mais recente 
(especificada pelo tag config ), respeitando as restrições sem ver tanto do seu 
pacote quanto de suas dependências (se também exigirem o mesmo pacote).

Ele também instalará pacotes ausentes.

Se o -g sinalizador for especificado, este comando atualizará os pacotes 
instalados globalmente.

Se nenhum nome de pacote for especificado, todos os pacotes no local especificado 
(global ou local) serão atualizados.
