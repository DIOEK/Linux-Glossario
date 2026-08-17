# Glossario
Linux terms and commands glossary

venv - Virtual Environment. Python virtual environment that uses its own Python interpreter, installed packages, and pip configuration. Used to isolate dependencies between projects. For example, one project may use Flask 2.x while another uses Flask 3.x without conflicts. Source: https://docs.python.org/3/library/venv.html

bin (linux) - Traditional Linux directory used to store executable programs and scripts.

activate (venv) - Script created inside a Python virtual environment used to activate it and configure environment variables such as PATH and VIRTUAL_ENV.

source - Shell built-in command used to execute a script inside the current shell session. When a script is executed normally, a subprocess is created and any environment changes disappear when it exits. The source command prevents this behavior, allowing changes such as those made by activate to remain in the current session. Equivalent to ". venv/bin/activate". Source: https://www.gnu.org/software/bash/manual/bash.html

asyncua - Python library for communicating with OPC UA systems. Allows reading, writing, browsing the address space, and invoking methods on OPC UA servers. Source: https://opcua-asyncio.readthedocs.io

uaread (asyncua) - CLI tool from the AsyncUA package used to read the value of an OPC UA node.

uawrite (asyncua) - CLI tool from the AsyncUA package used to write a value to an OPC UA node.

uals (asyncua) - CLI tool from the AsyncUA package used to list the OPC UA address space, similar to the ls command.

uacall (asyncua) - CLI tool used to invoke methods exposed by an OPC UA server.

node (opc ua) - Basic OPC UA element. A node can represent an object, variable, method, type, or reference and is identified by a NodeId.

OPC UA - Open Platform Communications Unified Architecture. Industrial communication protocol widely used in SCADA, ICS, and IoT environments to exchange data between devices, sensors, controllers, and applications. Source: https://opcfoundation.org/about/opc-technologies/opc-ua/

Javascript - Interpreted programming language widely used for frontend and backend web development. Source: https://developer.mozilla.org/en-US/docs/Web/JavaScript

Node.js (Javascript) - JavaScript runtime environment built on Google's V8 engine. Allows JavaScript applications to run outside the browser using an event-driven architecture and asynchronous I/O. While it can serve HTTP requests, it does not fully replace dedicated web servers such as Apache or Nginx. Source: https://nodejs.org

React (Javascript) - JavaScript library used to build user interfaces through reusable components. Source: https://react.dev

Asynchronous I/O - Execution model where an application can continue performing other tasks while waiting for input/output operations such as file access, network communication, or database queries.

CVE-2025-55182 - No widely recognized public documentation was found for this CVE associated with the name React2Shell. The reference should be verified before being included in the glossary.

ldap - Lightweight Directory Access Protocol. Protocol used to access and manage directory services such as Active Directory. Source: https://datatracker.ietf.org/doc/html/rfc4511

ldapsearch - Command-line tool used to query LDAP directories. Common flags: -x (simple authentication), -H (LDAP server URI), -D (Bind DN), -w (Bind DN password), -b (Base DN). Source: https://www.openldap.org/software/man.cgi?query=ldapsearch

SMB - Server Message Block. Network protocol used to share files, printers, and other resources. Based on a client-server architecture and supports user authentication. Source: https://learn.microsoft.com/en-us/windows-server/storage/file-server/file-server-smb-overview

smbpasswd - Samba utility used to manage SMB user passwords. Source: https://www.samba.org/samba/docs/current/man-html/smbpasswd.8.html

evil-winrm - Remote administration tool for Windows systems using the WinRM protocol. Source: https://github.com/Hackplayers/evil-winrm

reg (windows) - Command-line utility used to query and modify the Windows Registry. Source: https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/reg

save (windows) - reg subcommand used to export a registry hive to a file.

hive (windows) - Logical structure or file containing a section of the Windows Registry database.

MCP (Model Context Protocol) - Open protocol that enables AI models to communicate with external data sources, tools, and services. Source: https://modelcontextprotocol.io

opt (linux) - Directory typically used to install optional or third-party software packages.

ss (linux) - Socket Statistics. Utility used to display network sockets and associated processes. Common flags include TCP sockets (-t), UDP sockets (-u), listening sockets (-l), associated processes (-p), and numeric addresses/ports (-n). Source: https://man7.org/linux/man-pages/man8/ss.8.html

ps (linux) - Process Status. Command used to display information about running processes. Source: https://man7.org/linux/man-pages/man1/ps.1.html

Jupyter - Open-source web application used to create and execute interactive documents containing code, text, mathematical formulas, visualizations, and output in a single file. Source: https://jupyter.org

cron - Daemon responsible for executing scheduled tasks periodically. Typically runs continuously in the background. Source: https://man7.org/linux/man-pages/man8/cron.8.html

cronjob - Scheduled task executed by the cron service. Definitions are usually stored in crontab files or directories such as /etc/cron.d.

incron - Utility similar to cron but triggered by filesystem events using inotify. It can execute actions when files or directories are created, modified, or deleted. Source: https://inotify.aiken.cz/incron.html

touch - touch grass

touch (linux) - Command used to create empty files or update file access and modification timestamps. Source: https://man7.org/linux/man-pages/man1/touch.1.html

stat - Command used to display file metadata such as size, permissions, ownership, and timestamps. Source: https://man7.org/linux/man-pages/man1/stat.1.html

spool - Temporary storage location where data waits to be processed by another service. Common examples include print queues, email queues, and scheduled task queues.

log - Chronological record of events generated by a system, service, or application. Acts as the "journal" of a program.

.war (java) - Web Application Archive. Package format used to distribute Java web applications for deployment on application servers such as Apache Tomcat, WildFly, Jetty, or GlassFish. Source: https://docs.oracle.com/javaee/7/tutorial/packaging003.htm

proxy (reverse proxy web) - Intermediate service that receives client requests and forwards them to backend servers. Common examples include Apache HTTP Server, Nginx, and HAProxy. Source: https://docs.nginx.com/nginx/admin-guide/web-server/reverse-proxy/

xml - eXtensible Markup Language. Markup language used to store, structure, and transport data in a format readable by both humans and machines. Characteristics include extensibility, hierarchical structure, portability, and self-describing tags. Source: https://www.w3.org/XML/

FTP - File Transfer Protocol. Tool provided by TCP/IP protocol. It allows remote transfer of files and folders between computers, where one acts as a server and the other acts as a client. Default port is 21 and commands are very, very similar to bash commads. It can be accessed bia curl and other tools of http protocols. https://www.geeksforgeeks.org/computer-science-fundamentals/file-transfer-protocol-ftp/ https://linuxize.com/cheatsheet/ftp/

Path Traversal - Also known as Directory Traversal or "dot-dot-slash" attack. A vulnerability that allows an attacker to access files or directories outside the application's intended directory by manipulating file paths. It commonly uses sequences such as "../" (Linux) or "..\" (Windows) to navigate up the filesystem hierarchy and access sensitive files. The attack is not limited to the web root directory and may allow access to any file that the application's permissions permit. Source: https://owasp.org/www-community/attacks/Path_Traversal

Domain - A logical grouping of computers, users, and other network resources that are centrally managed under a common administration and security policy. In Microsoft environments, domains are typically managed through Active Directory and allow centralized authentication, authorization, and resource sharing across the network. Source: https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview

DC - Domain Controller. A server that maintains directory service information for a domain, including users, authentication credentials, groups, computers, and enterprise security policies. Domain Controllers host Active Directory Domain Services (AD DS) and authenticate users and computers within the domain. Source: https://www.techtarget.com/searchwindowsserver/definition/domain-controller

AD - Active Directory. Microsoft's directory service for Windows domains. It stores and manages information about network resources such as users, computers, groups, printers, and security policies, and provides authentication and authorization services across the network. Source: https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview

Immutability - The property of an object or dataset that prevents it from being modified or deleted after creation. In backup systems, immutability ensures that backups cannot be altered, overwritten, or removed during a defined retention period, protecting them from accidental deletion, malicious activity, and ransomware attacks. Source: https://www.ibm.com/think/topics/immutable-backups

Veeam - Data protection, backup, disaster recovery, and ransomware recovery software company. Its products are used to create, manage, replicate, and restore backups for physical, virtual, cloud, and hybrid environments. Source: https://www.veeam.com

Backup - A copy of data, system state, configuration, or application data stored separately from the original source to enable recovery in the event of data loss, corruption, hardware failure, accidental deletion, or cyberattacks. Source: https://www.ibm.com/topics/backup

Hydra - Commonly known as THC Hydra. Open-source password auditing and credential brute-forcing tool capable of testing username and password combinations against numerous network services and protocols, including SSH, FTP, SMB, RDP, HTTP authentication, LDAP, and others. Frequently used during penetration testing and security assessments to identify weak credentials. Source: https://github.com/vanhauser-thc/thc-hydra

NFS - Network File System - Protocol used so a user can access files and directories store locally at another computer, they must be inside the same network even if not locally. Follows a client-server architecture. The NFS server, exports(shares) one or more directories. The client requests acess to an exported directory. The server verifies whether the client is authorized to mount the share. Applications can then read, write and modify files on the remote server as if stored locally. https://cmdref.net/os/linux/disk/nfs.html

Mounting - The act of making a filesystem or storage device accessible through a directory in an operating system. can be done via GUI or even command line. Works differently for each protocol, like SMB(Windows) NFS.

showmount - command used for querying NFS servers for shared(exported) directories.

Runtime error - A runtime error is an error that happens when a program is already running, after it has been compiled. Basically a "bug". The trick is if a program is working fine, but it requires input of some sort and you don't provide it, or provide the wrong sort of input, then this type of error may appear. https://www.geeksforgeeks.org/dsa/runtime-errors/

SSRF (Server Side Request Forgery) - Technique where the attacker might cause the server to connect to inside only services. Basically having unauthorized access to server side services. https://portswigger.net/web-security/ssrf

API (Aplication Programming Interface) - Basically the thing that allows for software to communicate with server and other software, via REST or whatever. Always usefull to check for /api directories e subdirectories sucha as /api/version /api/v1(2,3, etc) 

SID (Security Identifier) - 

