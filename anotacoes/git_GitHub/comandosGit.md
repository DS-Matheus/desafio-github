## Comandos básicos do Git Bash

### Primeiros passos

* **ssh-keygen:** usado para gerar uma chave de identificação SSH.
  ssh-keygen -t ed25519 -C email
* **cat:** concatena e/ou faz a leitura de arquivos.
  cat id_ed25519.pub
* **eval $(ssh-agent -s):** inicia o processo do agente de chaves SSH, usado para gerencia-las de forma automática.
* **ssh-add:** adiciona uma chave SSH ao agente, deve-se utilizar a chave privada nesse processo.
  ssh-add id_ed25519
* **git config:** gerencia as configurações do git, como nome de usuário e email, que podem ser definidas para todos os repositórios ou para um em especifico.
  git config --global user.email email
  git config --global user.name nome
* **git remote add:** cria um ponteiro do repositório local para o da nuvem, permitindo que o primeiro possa "empurrado" enviado para o segundo, em nuvem.
  git remote add origin endereçoRepositorioGitHub
  (origin é apenas um apelido)
* **git remote -v:** exibe os ponteiros do repositório atual.

### Navegação e manipulação de arquivos

* **cd:** altera o diretório atual para o especificado.
  cd /c/workspace/
* **"cd ..":**	volta o diretório em 1 nível.

* **cat:** concatena e/ou faz a leitura de arquivos.
  cat exemplo.txt exemplo2.txt
* **pwd:** exibe o caminho do diretório atual.
* **ls:** exibe todos os arquivos e pastas do diretório atual.
* **"ls -a":** mesma função que o ls com a adição de exibir também os arquivos e pastas ocultas.
* **mkdir:** cria um novo diretório na localização atual
* **mv:** move um arquivo ou diretório para outra localização.
  mv arquivo1.txt ./c/workspace/arquivos/
* **echo:** exibe no terminal a mensagem digitada a seguir, pode ser utilizado em conjunto com ">" para salvar essa mensagem em um arquivo.txt.
  echo hello world > hello.txt