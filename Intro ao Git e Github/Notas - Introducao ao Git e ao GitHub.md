6 de fev. de 2022

# Comandos básicos para navegação no terminal

- Windows:
	- cd: Muda de pasta
	- dir: Lista conteúdo da pasta
	- mkdir: Cria pasta
	- del: Deleta arquivos contidos na pasta
	- rmdir: Deleta a pasta e seu conteúdo (pode usar flags /S /Q)

- Unix 
	- ls: Equivale ao dir
	- rm e rf: Equivalem ao del e rmdir
	- pwd: Mostra o caminho completo (caso esteja no GitBash)

# Chave SSH e Token

- No GitBash, digite:

`$ ssh-keygen -t ed25519 -C seuemail@mail.com`

- Prompt exibe:

    `Generating public/private ed25519 key pair.   Enter file in which to save the key (/c/Users/usuario/.ssh/id_ed25519):
    passphrase (empty for no passphrase):
    Enter same passphrase again:`

- Geradas as chaves (privada e pública), navego até a pasta

    `$ cd /c/Users/usuario/.ssh`

- Listo o conteúdo da pasta com ls ou dir

- Uso o comando cat para exibir conteúdo da chave pública

    `cat id_ed25519.pub`

- Copio a chave exibida pelo terminal

- Colo na conta do GitHub > Settings > SSH and GPG Keys

- No terminal, digito o comando abaixo para inicializar o agente SSH

    `$ eval  $(ssh-agent -s)`

- Depois de inializado, passo a chave privada para o agente (como já estou na pasta informo apenas o nome e não o caminho inteiro):

`$ ssh-add id_ed25519`

- Uso a senha criada na geração das chaves (início do passo a passo).
- Para clonar um repositório, sendo que configuramos SSH, temos que pegar não a url do mas sim clicar em <> Code e copiar o SSH.

A outra forma seria clonar normal usando o endereço https, que vai pedir senha e é menos seguro.

# Token de Acesso Pessoal

Outra forma de acesso.

É uma string bem grande. Deve ser salvo num arquivo.

GitHub > Settings > Developer Settings > Personal access tokens > Generate new token

Clono assim, normal:

`git clone urldorepo`

Em seguida, entro com o token de acesso no modal que surge.

