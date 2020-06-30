# Informe

### Tutorial de Generación de Máquinas virtuales en Microsoft Azure
**1.PLANTEAMIENTO DEL PROBLEMA**

Para pequeños desarrolladores o científicos, probar aplicaciones u otros programas en otros sistemas operativos requiere un elevado uso de recursos para los ensayos. Esto requiere la adquisición de infraestructura llegando a ser costosa para ocuparlo en un periodo corto de tiempo. ¿Cómo ejecuto un sistema operativo externo que permita la aplicación de programas a bajo costo y con poso consumo de recursos? Para ello, es necesario un proveedor de servicios en la nube.
Microsoft Azure es uno de los proveedores de servicios en la nube más usados en la actualidad. Se creo en la necesidad de un soporte técnico, fuera de una empresa, para satisfacer a una o varias empresas. Su tipo de nube es pública, es decir, que cualquiera con conexión a internet puede hacer uso de este servicio. Entre los servicios más destacados que ofrece es la generación de máquinas virtuales, con el objetivo de que sean empleados como servidores.  Estas máquinas permiten ejecutar sistemas operativos dentro de otro, sin influir en el de la base.

**2. OBJETIVOS**

2.1 Objetivo general

Desarrollar un tutorial basado en el funcionamiento del servicio de computación en la nube, Microsoft Azure, como un generador de máquinas virtuales para los estudiantes de Tercer nivel de la carrera de Ingeniería en Telecomunicaciones, de la Universidad de las Fuerzas Armadas ESPE, en la sede Sangolquí, en el periodo mayo – septiembre de 2020.

2.2 Objetivos Específicos

Crear una cuenta de usuario en Microsoft Azure

Enmarcar las características que poseen las máquinas virtuales y los pasos para su instanciamiento.

Grabar un videotutorial mostrando el funcionamiento dentro de la pantalla virtual

**3. ESTADO DEL ARTE**

*Control Automático de Memoria de Múltiples Máquinas Virtuales en un Servidor Consolidado*

En la publicación realizada por Wei-Zhe-Zhang, Hu-Cheng Xie y Ching-Hsien Hsu, profesores del Departament of Computer Science and Information Enginnering, Chung Hua University, Hsinchu, Taiwan; explican el diseño de un ballon driver, en la cual permitió controlar el consumo de memoria de dos o más máquinas virtuales operativas en una máquina física. Con ello evitaron que las aplicaciones ejecutadas sufran deterioraciones provocada por una lucha en el consumo de memoria. Este driver se ajusta automáticamente y fue evaluada en 10 máquinas virtuales, mostrando efectividad de 500% en su disco duro y un 300% en su Memoria RAM. (Zhang , Xie, & Hsu, 2015).

*La nube o sin la nube: La Pregunta para un Centro de Datos Científicos*

Marcelo Cinque, Doménico Cotroneo, Flavio Frattini y Stefano Russo, investigadores del Dipartimento di Ingengneria Elettrica e delle Tecnologie dell’Infozaion, Universiá di Napoli Federico, Italia; mencionan las ventajas y desventajas de los sistemas de cómputo en la nube para un desarrollo de datos. Ellos manifiestan principalmente que los servicios en la nube son efectivos para guardar información, siempre y cuando estos no sean vulnerables a fallas eléctricas o informáticas. La investigación concluyó que el rendimiento de los servicios de la nube, como es el caso de las máquinas virtuales, está ligada al consumo adecuado de los recursos para un mejor rendimiento. Ellos recomiendan definir bien su propósito de trabajo en ellas evitando así a una susceptibilidad de fallas. (Cinque, Cotroneo, Frattini, & Russo, 2015).

*Programación de máquinas virtuales en la nube: modelado de la instanciación de máquinas virtuales en la nube*

Stelios Sotiriadis, Nik Bessis, Nick Antonopoulos, programadores de Comput & Math., University of Derby, UK; y Fatos Xhafa, programador de Departamento de Llenguatges y Sistemas de la Universidad Politécnica de Catalunya, Barcelona, España; enfocaron en el desarrollo de un protocolo para la creación de máquinas virtuales, en función de las exigencias de trabajo. El análisis realizado se basó en la estructura de las capas de las máquinas, y los enfoques estáticos y dinámicos. Este modelo resalta una correcta instanciación de las máquinas virtuales, permitiendo una optimización del tiempo de latencia. Este trabajo no solo se enfoca en nubes locales, también busca un óptimo uso en nubes colaborativas. (Sotiriadis, Bessis, Xhafa, & Antonopoulos, 2012).

**4. MARCO TEÓRICO**

*4.1 ¿Qué es Microsoft Azure?*

Es uno de los tres proveedores de servicios de la nube más utilizados en el mundo. Cuando se menciona la nube se refiere a los servicios de hardware y software que se ofrece por medio de internet en la cual interactúan usuarios y un centro de datos.  Los usuarios pueden abarcar tanto a personas en particular como compañías en general.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2011.27.38.jpeg)

**Fig 1.** Esquema general de los servicios que ofrece Microsoft Azure

Fuente: https://blog.educacionit.com/2020/01/23/por-que-aprender-a-administrar-maquinas-virtuales-en-microsoft-azure/

El manejo y almacenamiento de la información puede que sea intangible, pero detrás de ello, se encuentra almacenada en grandes centros de datos distribuidos en todo el mundo, y su acceso está disponible en cualquier lugar y en cualquier momento. Esto se debe a que los centros de datos están dotados de una enorme infraestructura, organizados en habitaciones, con la capacidad de envío y recepción de un gran flujo de datos. Actualmente, la compañía dispone de más de 50 centros de datos en todo el mundo.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2011.27.48.jpeg)

**Fig 2.** Esquema general de los servicios que ofrece Microsoft Azure

Fuente: https://news.microsoft.com/en-gb/2019/04/09/microsoft-has-doubled-size-of-uk-azure-regions-increasing-compute-capacity-by-more-than-1500-as-country-embraces-digital-transformation/

El acceso se encuentra disponible para cualquier usuario a cualquier hora del día. Sin embargo, su uso está especificado tanto como un gestor de datos tanto a escala personal como a escala corporativa. Para una cálida bienvenida, Microsoft Azure ofrece una suscripción gratuita con un monto inicial de $200 dólares, en la cual no tiene que pagar. El cliente posee esta cuota con un plazo de un año a partir de la creación de la cuenta. Pasado el año, el cliente, si lo desea, puede renovar la cuota con un pago se acuerdo al uso de los servicios que ofrece Microsoft Azure.

![](https://kb.cloud.im/hc/article_attachments/360045148153/mceclip0.png)

**Fig 3.** Página principal de Microsoft Azure

Fuente: https://kb.cloud.im/hc/article_attachments/360045148153/mceclip0.png

*4.2 Tipos de nube*

Microsoft Azure ofrece los siguientes tipos de nube:

- Nube pública
Las propiedades del Hardware y el Software son administradas por el proveedor de servicios en la nube. Si bien, la gestión de archivos lo realiza el usuario, el proveedor de la nube lo realiza en mayor parte. Una de las ventajas de esta nube son los costos accesibles por el uso de los servicios.
- Nube privada
Los recursos informáticos son de usos exclusivo de la empresa. La ventaja es la personalización de los servicios, permitiendo que las empresas tengan una mejor gestión de recursos con los niveles de seguridad adecuados y reduciendo el tiempo de latencia.
- Nube híbrida
Constituye las nubes públicas y privadas enlazadas entre sí. En una parte de ella se maneja la información general y otra información de tipo confidencial. Las ventajas que se pueden describir en el uso de estos servicios es la libre combinación de servicios públicos y el respaldo de una infraestructura privada.

*4.3 Servicios en la nube*

Microsoft comercializa los siguientes servicios en la nube:
- Software as a Service (SaaS)
La persona accede a los datos almacenados a través de internet. El mantenimiento es manejado por el proveedor. Constituye la parte externa de todos ellos
- Platform as a Service (PaaS)
Ofrece un entorno característico para el desarrollo de aplicaciones.
- Infrastructure as a Service (IaaS)
El proveedor proporciona el software y las aplicaciones. Generalmente, se enfoca al Hardware virtualizado, constituido por un conjunto de redes y servidores.

*4.4 Funcionalidades principales*

Microsoft Azure se ha destacado principalmente como:

4.4.1 Almacenamiento
- BackUp
Es uno de los servicios más demandados. Este garantiza una solución a una copia de seguridad, simplifica la recuperación de datos y es más fácil de habilitar que otros servicios en la nube entre las máquinas virtuales de Azure y los servidores locales.
- Línea Storage
Se encarga de la administración y almacenamiento de recursos. Esta destinado para disco, archivo, blob, HPC cache, entre otros.

4.4.2. Virtualización

La virtualización crea un entorno informático simulado, o virtual, en lugar de un entorno físico. A menudo, incluye versiones de hardware, sistemas operativos, dispositivos de almacenamiento, etc., generadas por un equipo. Esto permite a las organizaciones particionar un equipo o servidor físico en varias máquinas virtuales. (General, s.f.) Es el funcionamiento de un sistema operativo dentro de otro, sin que las operaciones realizadas en uno cambien al sistema de soporte. La creación es característica de cada usuario, donde puede configurar cualquier sistema operativo y el tamaño de sus componentes como disco duro, memoria RAM, tarjetas de red, entre otros. 

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2011.28.03.jpeg)

**Fig 4.** Vista previa de cuatro virtualizaciones en una pantalla

Fuente: https://askleo.com/can-my-isp-see-what-im-doing-if-i-use-a-virtual-machine-vm/

La ventaja de ejecutar un sistema operativo en la nube es que no requiere consumo adicional de memoria RAM (aparte de lo que consume el navegador) ya el proceso se lo ejecuta en un centro de datos. El propósito de la virtualización que ofrece este servicio en la nube es para establecer servidores. No importa el sistema operativo que posea, ni la versión del sistema que usa, ya que el único requisito para la creación de máquinas virtuales es poseer una cuenta de usuario del proveedor de la nube y conexión a internet. Este servicio parte de SaaS.

Funcionamiento de virtualización de servidores
1. Adquisición del servidor
2. Implementación del servidor virtual
3. Creación de los sistemas virtuales
4. Instalación de los sistemas y conexión con SAN

Otras ventajas de las máquinas virtuales
- Interfaz y administración sencillas: el uso y puesta a punto de las máquinas virtuales de Azure están diseñados para todo tipo de usuarios.
- Aislamiento de fallos: un fallo general de la aplicación en una máquina virtual no afecta a los demás sistemas, evitando fallos críticos para la empresa.
- Mayor protección de los datos: acceder a un sistema virtualizado proporciona una capa más de seguridad para sus datos.
- Acceso remoto: la disponibilidad de la información contenida en las máquinas virtuales desde cualquier lugar gracias a la nube.
- Administración de sistemas centralizada: facilidad para la gestión mediante la interfaz de administración de máquinas virtuales de Azure.
- Aplicaciones de Microsoft integradas con más facilidad: los programas de Microsoft (Office 365, Exchange, SharePoint, Dynamics, etc.) están soportados de forma nativa, lo que proporciona un sistema estable para la virtualización de estas aplicaciones

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2011.28.14.jpeg)

**Fig 5.** Ejecución de una máquina virtual dentro de otra máuina virtual

Fuente: https://www.xataka.com/especiales/maquinas-virtuales-que-son-como-funcionan-y-como-utilizarlas

*4.4.3 Otros servicios*
- Análisis: verificación de datos en tiempo real
- Bases de datos: parte de un IaaS
- Contenedores: desarrollo de aplicaciones dentro de un contenedor
- DevOps: integración entre desarrolladores
- IA y Machine Learning
- Identidad: gestiona el directorio activo en nube sincronizando con el resto de los servicios.
- Redes: virtualiza conexiones de red y direcciones TCP/IP.
- Seguridad: cuida la infraestructura de algún ataque.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2011.34.11.jpeg)

**Fig 6.** Portal de Microsoft Azure

Fuente: https://azurecomcdn.azureedge.net/cvt-2ce59fd809b99599ffdde580d1ff242f2386263d3d8436821e75ad942b78dfb2/images/page/free/portal-home-alt

**5. EXPLICACIÓN DEL FUNCIONAMIENTO**

5.1	Creación de la cuenta en Microsoft Azure

5.1.1 Ingrese a la página principal de Microsoft Azure. https://azure.microsoft.com/es-es/, y seleccione cuenta gratuita.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.18.41.jpeg)

8.1.2 Para cuenta normal, ingresamos el correo electrónico de Microsoft y la contraseña.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.18.46.jpeg)
![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.18.53.jpeg)

8.1.3	Proceda a detallar sus datos personales

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.19.04.jpeg)

8.1.4	Introduzca su número de teléfono para verificar la correspondencia de la cuenta

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.19.10.jpeg)

8.1.5 Introduzca los datos de la tarjeta de crédito. Hay que mencionar que esta petición es como garantía de uso de los servicios de Microsoft Azure, sin embargo, no se descontará de su cuenta al menos que solicite cuenta premium.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.19.16.jpeg)

8.1.6. Si está de acuerdo, acepte los términos y condiciones

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.19.24.jpeg)

8.1.7. El sistema confirma su creación. Así que seleccione IR al portal

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.19.32.jpeg)

8.1.8. Una vez en el portal, seleccione Máquinas Virtuales

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.20.25.jpeg)

8.1.9.Seleccione Agregar

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.20.33.jpeg)

8.1.10. Proceda a llenar los siguientes datos. Para ello, piense y escriba un nombre para su máquina virtual.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.20.39.jpeg)

8.1.11. Seleccione el lugar de origen de la máquina. Lo más recomendable es escoger el centro de datos más cercano a la localidad.

8.1.12.	Cree una cuenta de usuario para el ingreso de la máquina virtual. Para ello, piense en un nombre característico y una contraseña. Esto permitirá el acceso remoto desde el computador de origen a la máquina instanciada.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.20.44.jpeg)

8.1.13. Seleccione el puerto de entrada para la conexión. Lo más recomendable es conectar a un puerto RSP ya que es el método más generalizado para todas las computadoras. Cuando termine, presione Siguiente

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.20.50.jpeg)

8.1.14. En esta pantalla, por defecto crea un grupo de gestor de disco duro. Si dispone de un grupo de recursos, puede insertarlo. Es recomendable mantener la selección del disco 

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.20.55.jpeg)

8.1.15. Si desea aumentar la capacidad del disco, seleccione modificar tamaño y escoja el requerido. Caso contrario, manténgalo por defecto.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.21.00.jpeg)

8.1.16.	Verificamos las redes y los protocolos que nos permitirá conectar con nuestra máquina Virtual.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.21.06.jpeg)

8.1.17.	Verifique la administración del equipo cuando se arranque.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.21.11.jpeg)

8.1.18.	Este paso es opcional para personalizar a la máquina virtual.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.21.17.jpeg)

8.1.19.	Esta pantalla muestra uestra la facturación de uso de lam máquina con el crédito establecido.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.21.22.jpeg)

8.1.20.	Espere la implementación de la máquina

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.21.27.jpeg)

8.1.21.	La máquina virtual está lista, por lo que debe presionar ir al recurso en la barra de notificaciones.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.21.32.jpeg)

8.1.22.	Proceda a realizar la conexión entre su máquina y su computador, Para ello, seleccione conectar y luego elija el protocolo correspondiente.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.21.36.jpeg)
![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.21.42.jpeg)

8.1.23.	Proceda a descargar el archivo del escritorio remoto. Puede guardarlo en cualquier lugar.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.21.46.jpeg)
![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.21.52.jpeg)

8.1.24.	Proceda a ejecutar el archivo. Luego presione aceptar para confirmar la conexión.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.21.57.jpeg)

8.1.25.	Escriba el usuario y la contraseña.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.22.04.jpeg)

8.1.26.	Seleccione si para permitir establecer la conexión.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.22.10.jpeg)

8.1.27.	Una vez aceptada todas las condiciones, se activa el instanciamiento.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.22.15.jpeg)

8.1.28.	Y listo, su máquina está lista para ejecutar. El menú siguiente abre una introducción al manejo del equipo. También puede navegar por internet.

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.22.19.jpeg)
![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.22.26.jpeg)

8.1.29.	8.1.27.	Y, por otro lado, el escritorio de la computadora no ha cambiado en nada

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2010.22.31.jpeg)

**9. DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN**

Como el proceso se da en un navegador web, se debe tomar en cuenta estos mínimos requisitos
- Sistema operativo Windows 10, 8 o 7. 
- 1-2 GB de RAM - 16 y 20 GB de almacenamiento en disco

**10.	CONCLUSIONES*
- Se concluye que se realizó el desarrollo del tutorial de manera exitosa debido a que el sistema de cómputo de la nube de Microsoft Azure brinda una guía rápida para la instanciación de máquinas virtuales, logrando desarrollar un videotutorial de aproximadamente 12 minutos. 
- Crear una cuenta en Microsoft Azure es muy sencillo, solo que debe garantizar una forma de pago a futuro, analizando los precios y el tiempo de ejecución del proyecto. si se desea obtener servicios a largo plazo.
- La instanciación de la máquina virtual fue muy concreta ya que especificaba los tamaños de los discos, las entradas de datos y otras especificaciones. Su implementación duró aproximadamente entre 2 a 5 minutos.

**11.	RECOMENDACIONES**
- Es importante verificar las conexiones remotas disponibles tanto en nuestro computador como en la máquina virtual. Si las conexiones son incompatibles, es preferible modificarlas antes de su creación ya que puede ser más difícil cambiar por las reglas de conexión establecidas.
- Es recomendable consultar conceptos desconocidos acerca de la estructura de computadoras. Tales conceptos como protocolos, reglas de seguridad, tipos de discos, deben ser analizados con detalle para un óptimo uso en nuestro sistema.

**12.	CRONOGRAMA**

Vista de calendario de actividades organizadas en los Meses de Mayo y junio

![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2011.06.19.jpeg)
![](https://github.com/deyder73/Tutorial-M-qina-Virtual/blob/master/img/WhatsApp%20Image%202020-06-30%20at%2011.06.26.jpeg)

**13.	BIBLIOGRAFÍA**

Cinque, M., Cotroneo, D., Frattini, F., & Russo, S. (2015). To Cloudify or Not Cloudify: The Question for Scientific data Center. IEEE, 1-14.
Editorial, E. (20 de 05 de 2019). REPORTEDIGITAL. Obtenido de https://reportedigital.com/negocios/tecnologia/que-es-nube-informatica/

General, I. (s.f.). Microsoft Azure. Obtenido de https://azure.microsoft.com/es-es/overview/what-is-virtualization/

González Fuentes, J. A. (2008). ojosdepapel.com. Obtenido de http://www.ojosdepapel.com/Index.aspx?
blog=918#:~:text=Internet%20se%20inici%C3%B3%20en%20torno%20al%20a%C3%B1o%201969%2C%20cuando%20el,vulnerables%20las%20comunicaciones%20militares%20norteamericanas.

Microsoft Services. (s.f.). Microsoft Azure. Obtenido de https://azure.microsoft.com/es-es/overview/what-are-private-public-hybrid-clouds/

Polanco, C. (s.f.). SOFECOM. Obtenido de https://sofecom.com/que-es-la-nube-informatica/

Sotiriadis, S., Bessis, N., Xhafa, F., & Antonopoulos, N. (2012). Cloud Virtual Machine Schduling: Modeling the Cloud Virtual Machine Instantiation. IEEE, 1-8.

The Mini Drive. (09 de 05 de 16). Obtenido de https://www.theminidrive.com/blogs/theminiblog-1/117191109-emuladores-y-maquinas-virtuales

Zhang , W. Z., Xie, H. C., & Hsu, C. H. (2015). Automatic Memory Control of Multiple Virtual Machines on a Consolidated Served. IEEE, 2-4.
