# 						Estudo Git e Github

### Entendendo o que é Git e a sua Importância

* Foi criado em 2005
* É um sistema de versionamento de código distribuído, no qual foi criado por **Linus Torvalas **

#### Benefícios

* Controle de versão
* Armazenamento em nuvem
* Trabalho e, equipe
* Melhorar o código
* Reconhecimento

## Chave SSH e Token

​		_SSH_ : forma de estabelecer uma chave segura e encriptada entre duas máquinas, vai sempre ter uma chave pública e uma chave privada.

#### Criando uma SSH dentro do Git Bash

	1. ssh-keygen -t ed2559 -C <e-mail utilizado no cadastro do Github>
	1. cd /c/Users/User/.ssh/  <código para achar as chaves criadas>
	1. cat id_ed25519.pub <código para visualizar o código>

Após criado a chave e copiado o código da chave pub, devemos colocá-la no terminal do GitHub, segundo os seguintes passos:

1. Perfil
2. Settings
3. SSH and GPG Keys
4. New SSH Key

Para que essa chave funcione, precisamos inicializá-lo dentro do Git Bash

1. eval $(ssh -agent -s) <gerar o número de processo>
2. ssh -add id_ed25519 <código para adicionar a chave>
3. git clone <link ssh do githhub>