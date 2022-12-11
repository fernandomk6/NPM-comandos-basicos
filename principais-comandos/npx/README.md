# O NPX

Execute um comando de um pacote local ou remoto.

## Descrição 

Este comando permite que você execute um comando arbitrário de um pacote 
npm (um instalado localmente ou obtido **remotamente**), em um contexto semelhante ao 
executá-lo via **npm run**.

Se algum pacote solicitado não estiver presente nas dependências locais do projeto, 
ele será instalado em uma pasta no cache npm, que é adicionado à PATHvariável de 
ambiente no processo executado.

