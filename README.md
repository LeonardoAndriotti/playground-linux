# Playground Linux

[Comandos gerais](#playground-linux)

[Permissões de arquivos](#permissões-de-arquivos)

[Links validos](#Links)

| Comandos        | Descrição  | Exemplo  |
| ------------- |:-------------:| -----:|
| pwd    | imprime o nome do diretório atual | pwd |
| ls      | listar o conteúdo do diretório      |  ls -l (ordenado p/coluna) / ls -f (executáveis)  / ls -la lista arquivos oculto|
| mkdir | Criar pastas     |    mkdir "nome da pasta"|
| touch | Criar arquivos     |    touch "nome do arquivo"."extensão"|
| cp | Copiar arquivos     |    cp "nome do arquivo" "nome da copia" |
| rm | Remover     |    rm -rf (remover dir, arquivos, etc) / rm -rfv (mostra o que foi removido) |
| mv | Mover arquivos     |    mv "nome do arquivo" "destino"|
| grep | procura por padrão em cada arquivo     |   grep "palavra" -n "nome do arquivo".txt |
| tail -f | gera a última parte dos arquivos     |    tail -f "nome do arquivo"|
| man | acesso ao manual    |    mkdir "nome da pasta"|
| tar -cvf  | compactar arquivos     |    tar -cvf “nome.tar” + arquivos|
| tar -xvf | descompactar arquivos    |    tar -xvf “nome do arquivo”|
| tar -tvf  | listar arquivos compactados     |    tar -tvf nome do arquivo|
| df | relatar uso de espaço em disco do sistema de arquivos     |    df -T / df -a / df  |
| free  | Exibe a quantidade de memória livre e usada no sistema   |    free |
| tree | lista o conteúdo dos diretórios em um formato de árvore.   |    tree |
| find  | procure arquivos em uma hierarquia de diretórios    |    find  "diretório" -name "nome do arquivo".txt |
| reboot | reinicia o sistema   |    reboot |
| shutdown | Ligar ou desligar  |   shutdown -h +19:00 ou  shutdown -h +8|
| useradd  | crie um novo usuário ou atualize as informações padrão do novo usuário   |    useradd "nome do user" |
| adduser | adiciona um utilizador ou grupo ao sistema   |    adduser |
| passwd  | altera senha do usuário  |    passwd "nome do usuário |
| usermod  | altera usuário    |    usermod  |
| groupadd | cria um grupo    |    groupadd |
| gpasswd  | Define senha para o grupo   |    gpasswd |
| groumod | Altera o grupo    |    groumod |
| groupdel | remove um grupo    |    groupdel |
| top  | exibir processos Linux   |    top |
| htop  | visualizador de processo interativo    |    htop |
| ps  | relatar um instantâneo dos processos atuais    |   ps / ps -ef |
| kill  | finaliza processos   |    kill / kill -9 |

## Permissões de arquivos 

*R* : Leitura /  *W* : Escrita / *X* : Executar

*U* : Usuário /  *G* : Grupo / *O* : Outros

| Permissão        | Número  | 
| ------------- |:-------------:|
| r | 1     |  
| w | 2     |  
| wx | 3     |  
| x | 4     |  
| rx | 5     |  
| rw | 6    |  
| rwx | 7   |  

1. Grupo -> root
1. Grupo -> grupo pertence o arquivo
1. Grupo -> outros



| Comandos        | Descrição  | Exemplo  |
| ------------- |:-------------:| -----:|
| chmod | dar permissão    |    chmod 777 "arquivo ou dir" -R|
| chmod | dar permissão    |    chmod g + xux|
| chmod | dar permissão     |    chmod root:root "nome do arquivo"|

Para alterar o proprietário de um arquivo ou pasta qualquer, utilizamos o comando “chown” (change owner). Este comando tem a seguinte sintaxe:

chown [novo proprietário] [caminho/da/pasta/arquivo] [-R]

Para [novo proprietário] utilizamos o nome de usuário do novo proprietário.

Para [caminho/da/pasta/arquivo] indicamos o caminho da pasta ou do arquivo que queremos alterar.

O [-R] serve para pastas e indica “modo recursivo”, ou seja, altere a pasta e todos os arquivos dentro dela. Ele é opcional.

## Links

[baeldung - JAVA_HOME](https://www.baeldung.com/java-home-on-windows-7-8-10-mac-os-x-linux#linux)

[baeldung - PATH](https://www.baeldung.com/linux/path-variable)

