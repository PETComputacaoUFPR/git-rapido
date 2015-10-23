# Workflows

Se você nunca usou o Git ou vem de outro controle de versão, pode ser difícil saber por onde começar. Este capítulo tem como objetivo explicitar alguns *workflows* possíveis com o Git.

Lembre-se que estes *workflows* são guias e não regras. Você pode alterá-los ao seu bel-prazer para melhor adequá-lo ao seu modo de trabalho.

## Centralizado

Você não precisa mudar seu modo de trabalho para começar a usar o Git. Se você usava Subversion (SVN) pode continuar trabalhando igual.

Usar o Git em vez do SVN tem suas vantagens. Primeiro, cada desenvolvedor tem sua própria cópia local do projeto inteiro. Isso permite trabalhar de forma independente e isolada no repositório, sem medo de alterar o código dos colegas ou em produção: é possível adicionar commits e esquecer do que está acontecendo no repositório central até que seja conveniente.

Isso também permite utilizar o sistema de *branching* e *merging* do Git, que, ao contrário do SVN, foram pensados para serem uma forma segura de adicionar e compartilhar código entre repositórios.