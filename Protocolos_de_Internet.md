# Principales protocolos de internet
 

### TCP/IP
 ---
Es el acrónimo que se utiliza comúnmente para el conjunto de protocolos de red que componen el conjunto de protocolos de Internet.

- **Tansmision Control Protocol**

Permite a las aplicaciones comunicarse entre sí como si estuvieran conectadas físicamente. TCP envía los datos en un formato que se transmite carácter por carácter, en lugar de transmitirse por paquetes discretos. Esta transmisión consiste en lo siguiente:
- Punto de partida, que abre la conexión.
- Transmisión completa en orden de bytes.
- Punto de fin, que cierra la conexión.

      Puertos
      Rango 1 al 1023:
        1 – 255 puertos publicos
        256 – 1023 puertos asignados a empresas
      Rango 1024 al 49151 – asignados por IANA a especificas aplicaciones
      Rango 49152 al 65535 – puertos dinámicos y privados


- **Internet Protocol**

El IP (Protocolo de Internet) es el protocolo más básico de Internet, y provee todos los servicios necesarios para el transporte de datos. 
El protocolo IP se encarga de:
- Direcciones IP: Las convenciones de direcciones IP forman parte del protocolo IP. 
- Comunicaciones de host a host: El protocolo IP determina la ruta que debe utilizar un paquete, basándose en la dirección IP del sistema receptor.
 - Formato de paquetes: el protocolo IP agrupa paquetes en unidades conocidas como datagramas.
- Fragmentación: Si un paquete es demasiado grande para su transmisión a través del medio de red, el protocolo IP del sistema de envío divide el paquete en fragmentos de menor tamaño. A continuación, el protocolo IP del sistema receptor reconstruye los fragmentos y crea el paquete original.

### SCTP
 ---
Esta orientado a la conexión que ofrece los mismos servicios a las aplicaciones que TCP. Además, SCTP admite conexiones entre sistema que tienen más de una dirección, o de host múltiple. La conexión SCTP entre el sistema transmisor y receptor se denomina asociación. Los datos de la asociación se organizan en bloques. Dado que el protocolo SCTP admite varios hosts, determinadas aplicaciones, en especial las que se utilizan en el sector de las telecomunicaciones, necesitan ejecutar SCTP en lugar de TCP.

      Puertos
      Rango 1 al 1023:
        1 – 255 puertos publicos
        256 – 1023 puertos asignados a empresas
      Rango 1024 al 49151 – asignados por IANA a especificas aplicaciones
      Rango 49152 al 65535 – puertos dinámicos y privados

### UDP
 ---
Proporciona un servicio de entrega de datagramas. UDP no verifica las conexiones entre los hosts transmisores y receptores. Dado que el protocolo UDP elimina los procesos de establecimiento y verificación de las conexiones, resulta ideal para las aplicaciones que envían pequeñas cantidades de datos.

      Puertos
      Rango 1 al 1023:
        1 – 255 puertos publicos
        256 – 1023 puertos asignados a empresas
      Rango 1024 al 49151 – asignados por IANA a especificas aplicaciones
      Rango 49152 al 65535 – puertos dinámicos y privados

### FTP
 ---
**File Transfer Protocol** o Protocolo de transferencia de archivos.
Es un protocolo que define cómo transferir archivos de un ordenador a otro, de un servidor remoto a un servidor local o viceversa. Se precisa un servidor de FTP y un cliente de FTP. Los servidores pueden ser de libre acceso con un login o FTP anónimo. 
    
    Puertos:
    20/TCP DATA Port
    21/TCP Control Port

### HTTP
 ---
**HyperText Transfer Protocol** o Protocolo de Transferencia de Hipertexto. 
El protocolo HTTP es el que permite el intercambio de información hipertextual (enlaces) de las páginas web. Se trata de un protocolo genérico orientado a objetos, que puede usarse para muchas tareas como servidor de nombres y sistemas distribuidos orientados a objetos, por extensión de los comandos o los métodos usados. Una de sus características principales es la independencia en la visualización y presentación de los datos, lo que permite que los sistemas sean construidos independientemente del desarrollo de nuevos avances en la representación de los datos. 

En este protocolo existen una serie de conceptos tales como:
* Conexión: es el circuito virtual establecido entre 2 programas en una red de comunicación
* Mensaje: es la unidad básica de un protocolo HTTP y consiste en una secuencia estructurada que se tramite entre los programas
* Cliente: es el programa que hace la llamada al servidor y es el que atiende en la transmisión la trama de los mensajes
* Servidor: es el programa que presta el servicio en la red
* Proxy: se trata de un programa intermedio que actúa sobre el servidor y el cliente

      Puertos:
      443/TCP
    
### SMTP
---
**Simple Mail Transfer Procol** o Protocolo de Transmisión de Correo Simple es el protocolo que nos permite recibir correos electrónicos y, junto con el protocolo POP (Post Office Protocol) o Protocolo de Oficina de Correos, usado por los ordenadores personales para administrar el correo electrónico. 

    Puertos
    25/TCP
    587/TCP (alternativo para clientes de correo)
    465/TCP (SMTPS)

### IMAP
 ---
**Internet Message Access Protocol** (Protocolo de acceso a mensajes de internet), es un protocolo de aplicación que permite el acceso a mensajes almacenados en un servidor de Internet. Mediante IMAP se puede tener acceso al correo electrónico desde cualquier equipo que tenga una conexión a Internet.

    Puertos:
    143/TCP
    220/TCP (IMAP3)
    993/TCP (IMAPS)

### NNTP 
 ---
**Network News Tranfer Protocol** (Protocolo de Transferencia de Sistemas de Redes de Noticias). Se trata de un foro de discusión por temas en forma de tablón de anuncios que cuenta con sus propios servidores y sus propios programas. Generalmente, el mismo programa que gestiona correos electrónicos, sirve para gestionar las news o noticias.

    Puertos:
    119/TCP

### IRC
 ---
 **Internet Relay Chat** es un protocolo de comunicación que permite conversaciones (chats) y debates en grupo o en privado, en tiempo real siguiendo la arquitectura del modelo cliente-servidor, pero formándose redes entre los servidores para acoger a más usuarios. Las conversaciones se desarrollan en los denominados canales de chat. Se entra en ellos adoptando un nickname o apodo y existen personas encargadas de crear y mantener los canales (los llamados CS o Chan Service), personas encargadas de mantener la red (IRCop), usuarios con privilegios de administrador del canal (Op) e incluso robots (Bot) que automatizan los servicios del canal. 
 
    Puertos:
    194/TCP
 
### TELNET
 ---
Protocolo que permite la conexión remota a otro ordenador y que permite manejarlo como si se estuviese físicamente ante él. Así, es posible arreglar fallos a distancia o consultar datos en la otra máquina.

    Puertos:
    23/TCP

### ARP
 ---
**Address Resolution Protocol** (protocolo de resolución de direcciones) ayuda al protocolo IP a dirigir los datagramas al sistema receptor adecuado asignando direcciones Ethernet a direcciones IP conocidas.

### ICMP
 ---
**Internet Control Messages Protocol** (protocolo de mensajes de control de Internet) detecta y registra las condiciones de error de la red.
ICMP registra:
- Paquetes soltados: Paquetes que llegan demasiado rápido para poder procesarse.
- Fallo de conectividad: No se puede alcanzar un sistema de destino.
- Redirección: Redirige un sistema de envío para utilizar otro enrutador.