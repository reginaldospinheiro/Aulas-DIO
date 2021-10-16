# **_Comandos Básicos para Git/GitHub_**

## _Comandos de Configurações Globais_
<br/>

##### **git config --global --list** -> Informa as configurações Globais de usuario e email
<br/>

##### **git config --global unsetser.email "seu email"** -> Para setar as configurações do seu e-mail. Usar o mesmo do github.
##### **git config --global user.name** -> Para setar as configurações do seu nome usuário. Usar o mesmo do github.
<br/>

##### **git config removel --global unset.email "seu email"** -> Para remover o email do usuário.
##### **git config --global unset.name** -> Para remover o nome de usuário.
<br/>

## _Comandos de Navegação_
<br/>

##### **dir** -> Listar pastas.
##### **cd** -> Abrir pastas.
##### **cd ..** -> Voltar Pasta
##### **cd /** -> para entrar em pasta especifica. _EX: cd /windows_.
##### **cls** -> Para Limpar o prompt.
##### **Tecla TAB** -> Auto Completar.
##### **ls** -> Para Listar arquivos.
##### **ls -a** -> Para Listar arquivos ocultos.
##### **pdw** -> Para Mostrar o caminho da pasta onde você está.
<br/>

## _Comandos para pastas/Docs_
<br/>

##### **mkdir** -> criar pastas.
##### **echo** > **arquivo.extensão**. -> Para criar arquivos.
##### **rmdir nome do diretorio /S /Q** -> remove a pasta e arquivos dentro.
##### **del nome do diretorio** -> Apaga arquivos dentro de uma pasta.
##### ****
<br/>

## _Criar chave SSH e Token no GIT_
<br/>

#### _A chave é útil para que não seja feita a solicitação de permissões ao enviar arquivos do git para o github_
<br/>

##### **ssh-keygen -t rd25519 -C seu_email_** -> Para Gerar a Chave. _OBS: O e-mail tem que ser o mesmo do github. Será solicitado uma senha._
##### **cat id_ed25519.pub** -> Para ver a chave publica e colocar no github
##### **eval $(ssh-agent -S)** -> Para Startar um projeto.
##### **ssh-add id_ed25519** -> Para entregar a chave para o agente. _OBS: Ele vai solicitar a chave que foi usada na criação da chave_.
<br/>

## _Para movimentar os diretorios Online e Local_
<br/>

#### _pastas privadas sempre vão solicitar senhas._
#### _Para locais de trabalho com chave SSH configurados, utilizar no clone a opção SSH._
<br/>

##### **git clone** -> para clonar um diretorio do github.
<br/>

#### _Para iniciar um projeto local. Entrar com o comando **"git init"** para gerar a pasta git dentro da pasta para que o git comece a versionar o código._
_Alguns comando somente funcionam após a criação desta pasta._
<br/>

##### **git init** -> Para que o git comece a versionar e gerenciar a pasta. Ela é oculta.
##### **git add .** -> Para adicionar os arquivos para a fila de commit.
##### **git commit -m "descrição breve do commit"** -> Para commit de projeto.
##### **git remote -v** -> Confira se o endereço do repositório do GitHub está correto no projeto local.
##### **git remote add origin e a url da repositorio do github que você deseja apontar** -> Comando para que o git local possa apontar para uma pasta remota do github.
##### **git push -u origin master** -> Para enviar os projetos do repositório local para o repositório online do github. _"OBS: Caso esteja trabalhando em outro branch, substitua o nome master pelo nome do branch"_
##### **git pull** -> para baixar as atualizações do repositório github para o git local.

<br/>

