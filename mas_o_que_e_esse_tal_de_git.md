# Mas o que é esse tal de Git?
Vamos agora falar um pouco sobre como o Git funciona. Se você já usou um VCS antes, tente não pensar nos conceitos dele.

A maioria dos VCS armazena uma lista de mudanças por arquivo. Esses sistemas mantém um conjunto de arquivo e as mudanças feitas a cada arquivo ao longo do tempo.

O Git salva um conjunto de snapshots (captura de algo em um determinado instante, como uma foto) de um mini sistema de arquivos. Toda vez que você salva (faz um *commit*) é como se o Git tirasse uma foto dos seus arquivos naquele momento. Para ser mais eficiente, arquivos não alterados não são salvos, apenas um link para o arquivo anterior é armazenado.

Outro diferencial do Git é que a maioria das operações precisam apenas dos arquivos e dos recursos locais. Como ele é distribuído, todo o histórico do seu projeto está no seu disco já. Você pode navegar até a versão de um mês atrás de um arquivo e fazer comparações e modificações sem tem que requisitar a algum servidor por isso. Por isso, há poucas coisas que você pode fazer que realmente necessitam de acesso a internet.

A maioria das ações no Git apenas acrescenta dados à base. Assim, quase tudo é reversível no Git. Como em qualquer sistema, você pode perder arquivos e informações de coisas que não salvou (*commitou*), mas depois de salvo é muito difícil que informação seja perdida.

### Integridade
Tudo o que o Git armazena é identificado por um checksum. Esse checksum é calculado antes que seja armazenado e existem um para cada arquivo e *commit*. Com isso é impossível mudar o conteúdo de algum arquivo sem que o Git saiba.

O checksum utilizado é uma hash SHA-1, uma string de 40 caracteres composta de caracteres hexadecimais calculado a partir do conteúdo de um arquivo ou diretório.

### Três estados