# Você precisa de controle (de versão)

Em um belo dia, você acessa seu computador, navega até a pasta do seu atual projeto e se depara com a cena de um crime: um dos arquivos está diferente do que você se lembra! Depois de um árduo trabalho para fazer a *função perfeita*, você não encontra nenhuma das suas alterações no seu arquivo. O que pode ter acontecido?

É então que você nota os seguintes arquivos:
* `projetoPerfeito-conflict-copy-joão.c`
* `projetoPerfeito-conflict-copy-caio.c`

Mas é claro! Alguém alterou o arquivo junto com você e gerou uma cópia de conflito. Agora basta fazer um diff dos arquivos, ver o que foi alterado e aplicar as alterações no arquivo correto. Mas antes vocÊ verifica o seu e-mail para ver se ninguém mais da equipe mandou alterações do código ou já resoveu o problema que você vai trabalhar.

E logo você se vê preso num ciclo vicioso com um CVH: Controlador de Versão Humano. Você se pega avisando sua equipe antes de alterar um arquivo e quando vai salvá-lo para evitar esses conflitos e criando pastas `V1`, `V2`, `V1-Corrigida`, `V2-Backup` para se organizar.

De repente, você e sua equipe estão trabalhando na V1-Corrigida (a versão correta do projeto) e acham um terrível e odiável bug. Ninguém sabe como ele surgiu. Depois de algum tempo perdido de debug, a origem dele é traçada até o coração da sua *funçãoPerfeita*. Mas você tem certeza que quando escreveu a função ela funcionava perfeitamente! Alguém deve ter modificado e inserido algum erro. Mas quem teria feito isso e, mais importante, quando isso teria ocorrido?

Ah, se ouvesse uma maneira fácil de fazer esse controle. Uma forma de salvar as versões do seu código a cada modificação, quem alterou, que parte alterou. Se fosse possível ainda manter várias versões do mesmo arquivo vivendo de forma harmoniosa. Ah, se algo tão maravilhoso assim existisse.