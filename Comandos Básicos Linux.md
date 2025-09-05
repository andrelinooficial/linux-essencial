## Comandos principais Bash 

### Abaixo os principais comandos usados no Bash:



<code> man</code><br>
Apresenta um manual ensinando os parâmetros de uso de comandos, exemplo: <code>man ls</code>

<br>

<code> cd /home </code><br>
Navega para o diretório /home

<br>

<code> pwd</code><br>
Mostra o diretório atual (Onde você está no momento)

<br>

<code> sudo apt update </code><br>
Busca atualizações para o sistema

<br>

<code> sudo apt upgrade </code><br>
Instala atualizações

<br>

<code> ls </code><br>
Lista diretórios (Você pode usar ls -lha para lista com mais detalhes)

<br>

<code> rm </code><br>
Remove um arquivo, para remover uma pasta com seus conteúdos use: <code>sudo rm -R diretorio</code>

<br>

<code> df -h</code><br>
Apresenta um resumo sobre o espaço que está sendo usado de armazenamentro

<br>

<code>sudo usermod -aG sudo nomeDoUsuario </code><br>
Adiciona um usuário como administrador adicionando ao grupo sudo !

<br>

<code>mkdir nomeDoDiretorio </code><br>
Cria um novo diretório (Caso queira criar diretórios com subdiretórios use: mkdir -p novoDiretoro)

<br>

<code>cat nomeDoArquivo.yaml </code><br>
Visualiza um arquivo

<br>

<code>nano nomeDoArquivo</code><br>
Abre um arquivo com o editor de texto nano... Ex: nano /etc/ssh/sshd_config -> Abre o arquivo sshd_config possibilitando edição do arquivo

<br>

<code>wget https://enderecodainternetparabaixaralgumacoisa.xyz</code><br>
Abre um arquivo com o editor de texto nano... Ex: nano /etc/ssh/sshd_config -> Abre o arquivo sshd_config possibilitando edição do arquivo


## Comandos para Administração de usuários:


<br>

<code>sudo useradd nomeDoUsuario </code><br>
Cria um novo usuário

<br>

<code>sudo passwd nomeDoUsuario </code><br>
Trocar a senha do usuário

<br>

<code>sudo usermod -L nomeDoUsuario </code><br>
Bloqueia um usuário


<br>

<code>sudo usermod -U nomeDoUsuario </code><br>
Desbloqueia um usuário

<br>

<code>sudo groupadd nomeDoGrupo </code><br>
Cria um novo grupo no sistema


<br>

<code>sudo usermod -aG sudo nomeDoUsuario </code><br>
Adiciona um usuário ao grupo sudo garantindo privilégios administrador (Você pode trocar sudo pelo nome do grupo que você deseja atrelar o usuário)

<br>


## Copiando, movendo e removendo :


<br>

<code>cp nomeDoArquivo /home</code><br>
Copia um arquivo do diretório atual para o diretório /home - (Caso queira fazer uma cópia no mesmo local use: <code>cp nomeDoArquivo nomeDoArquivo2</code>)<br>
OBS: Caso queira copiar uma pasta que contém arquivos utilize o parâmetro -R ex: <code>cp -R nomeDaPasta /home</code>


<code>mv nomeDoArquivo /home</code><br>
Move um arquivo do diretório atual para o diretório /home



<code>rm nomeDoArquivo</code><br>
remove um arquivo - (Caso queira remover um diretório use: <code>rm -r nomeDoDiretório</code>, se quiser forçar use -f, ex: <code>rm -rf nomeDoDiretorio</code>)


## Localização de arquivos:

Existe um programa chamado locate que não faz parte do repositório padrão de instalação do Debian, mais pode ser instalado usando o comando: <code>sudo apt install locate</code><br>
Este programa possibilita a localização de arquivos no sistema ! é importante sempre executar o comando <code>sudo updatedb</code> para garantir que ele reconheça toda a raiz do sistema para fazer buscas! 
<br>

<code>cp nomeDoArquivo /home</code><br>
Copia um arquivo do diretório atual para o diretório /home - (Caso queira fazer uma cópia no mesmo local use: <code>cp nomeDoArquivo nomeDoArquivo2</code>)<br>
OBS: Caso queira copiar uma pasta que contém arquivos utilize o parâmetro -R ex: <code>cp -R nomeDaPasta /home</code>
