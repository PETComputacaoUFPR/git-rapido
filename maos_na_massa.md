# Mãos na massa!

### Instalando e configurando
Descubra como  instalar o  Git para a sua plataforma através do site: https://git-scm.com/downloads

Depois de instalar o git na sua máquina, abra o terminal e configure suas informações:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

Se você use o Github ou o Gitlab, coloque as suas informações de usuário.

```bash
# Configure seu editor
git config --global core.editor vim
# Configure sua ferramenta de diff
git config --global merge.tool vimdiff
```

Para ver suas configurações utilize o comando `git config --list`.

#### O Comando `git config`
O comando `git config` lida com as suas configuraçãos do git em nível de repositório, global e de sistema.

Se você utilizar o comando sem nenhuma flag, estas configurações serão salvas apenas para o repositório. Com a flag `--global`, as configurações são salvas para todo o usuário (no arquivo .gitconfig, na sua pasta home). A flag `--system` salva as configurações para todos os usuários da máquina.

### Obtendo ajuda
```bash
git help <comando>
git <comando> --help
man git-<comando>
```

