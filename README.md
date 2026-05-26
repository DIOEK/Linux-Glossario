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
