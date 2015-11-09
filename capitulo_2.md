# Vamos as apresentações: Controle de versão, Leitor; Leitor, Controle de versão

Feitas as apresentações você deve estar se perguntando: quem é você, Sistema de Controle de Versão (ou *Version Control System* ou VCS)?

De maneira simples, o controle de versão é uma ferramenta que registra as alterações feitas em um documento, arquivo ou conjunto de arquivos ao longo do tempo para que você possa recuperar versões específicas.

Você pode versionar tudo. Tudo mesmo. Desde o seu próprio [sistema de controle de versão](https://github.com/git/git), as suas [resoluções do ano](https://github.com/una/personal-goals), os [problemas da sua casa](https://github.com/hostyle/house-problems/issues?q=is%3Aissue) e outras coisas como o código fonte do seu projeto, o [design da sua empresa](https://github.com/google/material-design-lite) e até mesmo [essa apostila](https://github.com/PETComputacaoUFPR/git-rapido).

Ao longo da apostila, iremos falar bastante sobre software e código fonte sob VCS****, mas tenha em mente que você pode utilzar para várias outras coisas.

Existem diferentes formas de controle de versão e veremos agora um pouco sobre elas.

## Controle de versão: modo calouro
O método mais comum para fazer esse controle é criar um diretório de backup. Se você for esperto, utiliza data e hora.

O problema ao fazer isto é ter o *overhead* das cópias dos arquivos (ou do projeto todo) ocupando espaço e qualquer descuido pode causar erros. Quando é uma boa hora de se fazer uma cópia do arquivo? Depois de várias alterações ou depois de algumas poucas?

![Controle de Versão Local](https://git-scm.com/figures/18333fig0101-tn.png)
###### Fonte: Git-scm

Para lidar com isso algumas pessoas desenvolveram sistemas locais de versionamento, como o [rcs](https://www.gnu.org/software/rcs/). Sistemas como esse salvavam os patches entre cada mudança e possibilitavam que qualquer arquivo pudesse ser recriado a partir de qualquer ponto na linha do tempo.

## Você não trabalha sozinho
O grande problema com sistemas locais é: o que fazer quando tenho que trabalhar em conjunto com alguém? Claro que você pode ficar trocando patches com seus colegas como quem troca figurinhas do álbum da copa, mas pode ficar cansativo aplicar as modificações e resolver quaisquer diferenças entre o seu código e o dos outros. Aliás, este método não garante que o seu código seja **exatamente** igual ao dos outros.

Bem, para trabalhar em equipe, você vai precisar de uma referência para o seu projeto. Essa referência é o servidor central de um Sistema de Controle de Versão Centralizado (ou *Centralized Version Control System*, CVCS). CVCS tem um único servidor central com todos os arquivos versionados que podem ser resgatados (através de um *checkout*) pelos clientes. O Subversion e o CVS são um exemplo disso.

![Controle de Versão Centralizado](https://git-scm.com/figures/18333fig0102-tn.png)
###### Fonte: Git-scm

Você pode ver que é muito mais fácil gerenciar as coisas assim, através de um repositório central, do que gerenciar diversos repositórios locais.

### Glossário: Reposi... quê?
|Repositório: |
|---|
| Chamamos de repositórios o local de armazenamento de um projeto sob um sistema de controle de versão. |

Você pode ver que os CVCS tem uma grande falha: o servidor central. Qualquer erro ou mal funcionamento afeta o desenvolvimento do projeto. Se não existir um backup, qualquer problema com o disco do servidor pode danificar o repositório. Tudo, menos as cópias locais dos desenvolvedores é perdido.

## As maravilhas do mundo distribuído
É aí que surgem os Sistemas de Controle de Versão Distribuídos (*Distributed Version Control System* ou DVCS). Em um DVCS, os clientes não só copiam as últimas versões do arquivo como copiam todo o histórico daquele arquivo, ou seja, os clientes são repositórios completos.

![Controle de Versão Distribuído](https://git-scm.com/figures/18333fig0103-tn.png)
###### Fonte: Git-scm

Esses sistemas (como o Git e Mercurial) lidam muito bem com esse fato, permitindo que você colabore com diversas pessoas e equipes no desnvolvimento de de um projeto.