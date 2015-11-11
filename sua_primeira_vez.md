# Sua primeira vez

Você agora tem o Git configurado na sua máquina, customizado e adaptado as suas necessidades e padrões. Você está pronto para usá-lo.

Agora só falta uma coisa: um repositório.

Um repositório Git é um conjunto de arquivos e pastas monitorados pelo VCS. Você pode obter um repositório de duas maneiras: iniciando o Git em uma pasta ou clonando um repositório de algum lugar.


### Criando seu repositório
Criar um repositório é um ato especial que ocorre quando uma pessoa e um projeto tem um afeto muito profundo um pelo outro. Quando eles desejam consumir sua relação por toda a eternidade, eles iniciam o Git.

`git init`

Este lindo comando inicia o controle de versão **dentro** do repositório em que ele é invocado.

`git init projeto`

Este comando, muito similar, cria uma pasta chamada *projeto* e inicia o controle de versão.

### Clonando o seu repositório
Clonar é um recurso muito útil utilizado por todos os cientistas malucos (e sãos também). Clonar um repositório é o ato de copiar *byte a byte* o repositório de outra pessoa ou outro local.

Você pode fazer isso assim:

`git clone [forma]`

Você pode clonar através de diferente protocolos:

* Local: `git clone ~/velho ~/novo`
  * Clona o repositório `velho` como `novo`
* ssh: `git clone ssh://url.da.maquin/repositorio` OU `git clone usuario@maquina:/repositorio`
* http(s): `git clone http(s)://url.com/repositorio`

**Exemplo Prático!**

Você pode clonar esta apostila com os seguintes comandos:

* `git clone https://github.com/PETComputacaoUFPR/git-rapido.git`
* `git clone git@github.com:PETComputacaoUFPR/git-rapido.git`