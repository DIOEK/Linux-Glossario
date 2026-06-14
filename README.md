# Linux-Glossario
Glossário de termos e comandos linux

venv - Virtual enviroment. Virtual Python environment that uses it's own Python interpreter, installed packages and pip configuration. Used when you need different versions of different software, for example you nesse flask x.x for a project and flask y.x for another, you should create a different venv for each.
bin - tradicional directory in linux used to storage executable programs and scripts
activate - shell script that is created with a venv and is used to activate it
source - Shell built-in command. When we execute a script, a new subprocess is created for it. Any enviroment changes dissapear when the script ends. But activating a virtual envinment needs to keep this change, such as changes in PATH, setting VIRTUAL_ENV etc... So source runs the script inside the current shell session only, so it does not intervene with other sessions. Other way to write source is ". venv/bin/activate" where . is shorthand for source.
asyncua - Pyhton Library used for dealing with OPC UA and it's associated systems. Allows fo control of these systems such as read/write. Has python interface and also CLI controlls.
uaread(asyncua) - reads a value of a node in a ocp server
uawrite(asyncua) - writes a value to a node in ocp server
uals(asyncua) - lists ocp ua address space like ls
uacall
node(opc) - Bsic OPC elemente, can be data, object, function accessible via NodeId.
OCP UP - Open source protocol used for working with industrial systems SCADA/ICS/IoT to expose sensors. 
Javascript - Linguagem interpretada,. muito utilizada para frontend e desenvolvimento Web. Geralmente roda no navegador.
Node(Javascript) - Ambiente de execução que permite desenvolvimento Backend fora do navegador. I/O assíncrono e arquitetura orientada a eventos. Não é um servidor completo mas pode entregar requests HTTP, por simular o servidor. Contudo não suporta roteamento dentre outro recursos que um webserver dedicado como apache nginx fornece.
React(Javascript) - Biblioteca para frontened utilizada no js, muito utilizada para componentes gráficos.
I/O assíncrono - Significa que a aplicação continua a executar sua função enquanto o ocorro o imput e o outpu(requisição de recursos, por exemplo).
CVE-2025-55182 - React2Shell(Vulnerabilidade) Vulnerabilidade que atinge a maneira que o React faz o parsing
ldap - Protocolo que ajuda a acessar e manter data. ldap pode ser utilizado para acessar data sobre usuários como usernames. Trabalha com vários tipos de Diretórios como um DC normal de Windows.
ldapsearch - tool for windows that you can use to query using the ldap protocol. Common flags: -x (simple authentication instead of sasl), -H (indicates Host), -D (bind Domain Name, can be empty ''), -w (indicates password for the bind DN, can be empty ''), -b (base DN)
SMB - Server Message Block - protocolo de comunicação utilizado para compartilhar arquivos, printes, portas seriais e outros recursos. Basea-se na relação cliente-servidor. Suporta user authenticação,
smbpass - aplicação que gerencia logins no protocolo smb, pode ser utilizada para mudar senhas e etc
evilwin-rm
reg(windows) - command line tool for interacting with windows registry
save(windows) - saves a registry hive to a file
hive(windows) - database file of windows registry
mcp - Windows Registry - database hieraquica que guarda informação sobre usuá
Mcp - Model context protocol - Allows ai to connecto to local data sources like files, code 
opt(linux) - optional third party software packages
ss (linux)- socket statistics lista sockets de rede e verifica quais processos estão a executar em quais portas. Pode aceitar flags para mostrar portas TCP (-t), UDP(-u), no modo listening (-l),  processo associado ao port (-p), endereços ip e numero de porta (-n).
ps (linux) - Process Status - Comando que lista processos rodando e informações sobre eles
Jupyter - Aplicação web de código aberto que permite criar e executar documentos interativos contendo código, texto, fórmulas matemáticas, visualizações e resultados num único ficheiro.
cron - serviço (daemon) que executa scritps ou processos rotineiramente de tempo em tempo. systemctl status cron ou crond. Sempre está rodando em segundo plano.
cronjob - file que que o cron executa geralemnte vai vir acompanhada de weekly ou algo assim. Ficam guardadas em /etc/cronjobs
incron - como um cron mas a condiocional que da trigger no gatilho é quando algo ocorre em algum file por exemplo um file ser criado por exemplo. podemos achar eles na pasta /etc/incron.d 
touch - touch grass
touch(linux) - cria uma file vazia ou então da "update nas timestamps de acesso e modificação da file" 
stat - mostra metadata da file como tamanho, timestamps de modificação e mudança acesso etc
spool - local onde algo espera para ser processado por outra coisa
log - Um log é um registo cronológico de eventos produzidos por um sistema, aplicação ou serviço. Um log é o "diário" de um programa.
.war(java) - Web Application Archive - formato de pacote utilizado para distribuir e implementar aplicações web Java em servidores de aplicações como Apache Tomcat  Wildfly, Jetty ou GlassFish
proxy(reverse proxy web) - serviço que recebe os requests e encaminha eles ao server http, atua como sujeito intermédio na conversa entre server e client EZ: Apache Nginx
xml - eXtensible Markup Language - usada para guardar, estruturar e transportar data em um formato que seja legível para humanos e máquinas. Extensible(usuário pode crar suas próprias marcas Estruturada(funciona de maneira hierarquica, utilizável em diferentes plataformas e auto descritível a tag mostra a data que contém.
markup language - linguagens com fim de estruturação, não lógica. Seu trabalho é estruturar, aprensentar e formatar. Ex: HTML XML MD

