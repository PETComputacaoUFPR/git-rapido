# Vamos as apresentações: Controle de versão, Leitor; Leitor, Controle de versão

Feitas as apresentações você deve estar se perguntando: quem é você, Controle de versão?

De maneira simples, o controle de versão é uma ferramenta que registra as alterações feitas em um documento, arquivo ou conjunto de arquivos ao longo do tempo para que você possa recuperar versões específicas.

Você pode versionar tudo. Tudo mesmo. Desde o seu [sistema de controle de versão](https://github.com/git/git), as suas [resoluções do ano](https://github.com/una/personal-goals), os [problemas da sua casa](https://github.com/hostyle/house-problems/issues?q=is%3Aissue) e outras coisas como o código fonte do seu projeto, o [design da sua empresa](https://github.com/google/material-design-lite) e até mesmo [essa apostila](https://github.com/PETComputacaoUFPR/git-rapido).

Existem diferentes formas de controle de versão e veremos agora um pouco sobre elas.

## Controle de versão: modo calouro
O método mais comum para fazer esse controle é criar um diretório de backup. Se você for esperto, até utiliza data e hora.

O problema ao fazer isto é ter o *overhead* das cópias dos arquivos (ou do projeto todo) ocupando espaço e qualquer descuido pode causar erros. Quando é uma boa hora de se fazer uma cópia do arquivo? Depois de várias alterações ou depois de algumas poucas?

Para lidar com isso algumas pessoas desenvolveram sistemas locais de versionamento, como o rcs. Sistemas como esse salvavam os patches entre cada mudança e possibilitavam que qualquer arquivo pudesse ser recriado a partir de qualquer ponto na linha do tempo.

