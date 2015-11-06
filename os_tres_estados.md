# Os Três Estados
Essa é uma das partes fundamentais para entender o Git.

O Git possui três estados para um arquivo:
1. Consolidado (*committed*)
2. Modificado (*modified*)
3. Preparado (*staged*)


### Estado Consolidado

As informações estão consolidadas quando estão salvas no seu repositório, quando elas foram *commitadas*. Um *commit* é justamente um *snapshot* que discutimos anteriormente.

Para salvar os arquivos você pode usar o comando: `git commit`. Este comando vai abrir o editor padrão (geralmente o Nano) e pede que você dê um nome para esse *commit*.

|**Importante**|
|--------------|
|Não se preocupe com comandos agora. Veremos eles com mais detalhes no futuro.|

### Estado Modificado
Este estado trata de um arquivo que foi alterado, mas não foi consolidado ainda.

### Estado Preparado
Um arquivo é tido como preparado quando você marca um arquivo modificado (ou um novo arquivo) em sua versão corrente para que ele faça parte do próximo *commit*.

Você pode fazer isso através do comando `git add [arquivo1] [arquivo2] [...] [arquivoN]`

## Três Estados: Três Áreas
Por isso, todo projeto do Git tem três áreas principais:
* O repositório Git
* O diretório de trabalho
* A área de preparação

O repositório é onde o Git armazena os metadados e o banco de objetos do seu projeto. Essa é a parte mais importante do Git e é a parte copiada quando você clona um repositório de outro computador.

O diretório de trabalho é um único *checkout* de uma versão do projeto. Estes arquivos são obtidos a partir da base de dados comprimida no diretório do Git e colocados em disco para que você possa utilizar ou modificar.

A área de preparação é um simples arquivo, geralmente contido no seu diretório Git, que armazena informações sobre o que irá em seu próximo commit. É bastante conhecido como índice (index), mas está se tornando padrão chamá-lo de área de preparação.

![Três estados do Git](https://git-scm.com/figures/18333fig0106-tn.png)