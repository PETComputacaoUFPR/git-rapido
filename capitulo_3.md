# Qual escolher?
###### Obviamente pelo título da apostila, nós vamos usar Git.


Se você ainda tem dúvidas de se você deve usar CVS, segue aqui uma breve lista de motivos:

* Use no desenvolvimento de código
* Use na manutenção de configurações
* Qualquer coisa que precise ter suas alterações salvas e controle sobre as modificações
* Atividades que exigem colaboração entre pessoas
* Armazenamento adequado das alterações
* Restaurar versões anteriores
* Compreender e visualizar o que aconteceu entre diferentes versões de algo
* Backup

## Por que o Git?

**Resposta curta**: é rápido e distribuído.

**Resposta longa**:

Era uma vez uma equipe de pessoas que trabalhava no kernel Linux. Essas pessoas transmitiam as alterações feitas no código em patches e arquivos compactados, mas isso era muito chato. Em 2002, a equipe decidiu utilizar o BitKeeper como DVCS, entretanto ele é proprietário. Você talvez se pergunte: "qual o problema disso?". Bem, veja só, o kernel Linux é *open-source* distribuído sob a GPL. O BitKeeper não cobrava pagamento do projeto até 2005, quando a empresa se desfez.

Com a dissuloção do BitKeeper, a comunidade de desenvolvedores (em particular o Linus Torvalds) desejou desenvolver a sua própria ferramenta baseada no que eles aprenderam com o BitKeeper. Os objetivos desse novo sistema eram:

* Velocidade
* Design simples
* Suporte robusto e desenvolvimento não linear (milhares de branches paralelos)
* Totalmente distribuído
* Capaz de lidar eficientemente com grandes projetos como o kernel do Linux (velocidade e volume de dados)

Foram com esses objetivos em mente que se fez o Git.

### Glossário: Branches?
Falaremos sobre branches num capítulo específico.