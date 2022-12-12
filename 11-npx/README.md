# npx

- `npx node_do_pacote` ou
- `npx nome_do_script`

Execute um comando de um pacote local ou remoto.

## Descrição 

npx é o executor de pacotes do node. Pode ser usado para executar qualquer pacote do npm,
sem instala-lo. Ao invés de instalar, você usa o pacote quando necessário. Quando precisar
usar, use o npx. npx é quando você deseja apenas usar o pacote, o npm é quando você deseja
instalar/gerenciar esse pacote e não apenas executar uma tarefa uma vez.

Quando você executa um pacote usando NPX, ele procura o pacote no registro local e 
global e, em seguida, executa o pacote.

Se o pacote ainda não estiver instalado, o NPX baixa os arquivos do pacote e instala 
o pacote, mas apenas armazenará os arquivos em cache em vez de salvá-los, ou seja, 
contradizendo o que foi dito na outra resposta:

>ja o npx ele irá usar o pacote sem precisar baixar em sua máquina,

Este comando permite que você execute um comando arbitrário de um pacote 
npm (um instalado localmente ou obtido **remotamente**), em um contexto semelhante ao 
executá-lo via **npm run**.

Esse comando permite você executar um pacote ou script que não esteja instalado
em suas dependencias. Você executa o comando apenas uma vez quando achar necessário,
sem tornar esse comando ou pacote, uma dependencia de seu projeto.

É semelhante a um `npm run alguma_coisa`, porem esse `alguma_coisa` não precisa está
instalada em sua maquina, basta está disponivel no registro do npm, e ela sera
executada como se estivesse instalada em sua máquina. Mas não será uma dependencia
de seu projeto. É uma forma de executar qualquer coisa do npm a qualquer momento
sem precisar instalar uma dependencia. Execute=o sob demanda.


