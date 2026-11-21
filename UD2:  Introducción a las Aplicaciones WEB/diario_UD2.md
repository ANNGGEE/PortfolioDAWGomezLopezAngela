# Diario de clase - UD2: Introducción a las Aplicaciones Web
## 1. ¿Qué he aprendido?

En esta unidad he aprendido diferentes conceptos relacionados con las aplicaciones web, su funcionamiento y los elementos necesarios para desplegarlas. He conocido mejor el protocolo HTTP (HyperText Transfer Protocol), utilizado para la comunicación entre clientes y servidores web, que normalmente funciona a través del puerto 80. También he aprendido la diferencia entre HTTP y HTTPS, siendo este último más seguro porque cifra la información que se transmite.

Otro de los contenidos que he aprendido ha sido el funcionamiento de los servidores web, especialmente Apache, y su función dentro de una arquitectura web. También he conocido cómo instalarlo y comprobar su funcionamiento tanto en Windows, mediante herramientas como XAMPP, como en Ubuntu, utilizando comandos desde la terminal.

Además, he aprendido qué es una arquitectura cliente-servidor, cómo se comunican ambas partes y las diferencias entre las arquitecturas de dos y tres capas. También he conocido los principales componentes de una arquitectura web moderna, como el frontend, el backend, las API, las bases de datos y los servidores web.

Por otro lado, he aprendido qué es el protocolo FTP, utilizado para transferir archivos entre un cliente y un servidor, y la diferencia entre FTP y SFTP, que ofrece una mayor seguridad al cifrar las comunicaciones mediante SSH. También hemos estudiado los diferentes tipos de alojamiento web, como el compartido, los VPS y los servidores dedicados, conociendo sus principales diferencias en cuanto a recursos, rendimiento y control.

Además de la teoría, hemos realizado varias prácticas relacionadas con el despliegue de aplicaciones web. Una de ellas ha sido la virtualización, en la que hemos instalado Ubuntu 24.04 LTS en VirtualBox. Durante esta práctica he aprendido a crear y configurar una máquina virtual y a instalar las Guest Additions, que mejoran la integración entre Ubuntu y VirtualBox, permitiendo, entre otras cosas, adaptar automáticamente la resolución de pantalla.

Otra actividad ha sido la instalación de Docker en Ubuntu. He aprendido qué son los contenedores, en qué se diferencian de las máquinas virtuales y cuáles son sus principales ventajas, como la portabilidad, el aislamiento y la rapidez de despliegue. También hemos instalado Docker Engine y Docker Desktop y comprobado su funcionamiento mediante la ejecución del contenedor hello-world.

Por último, hemos trabajado con la instalación de contenedores de servidores web y de aplicaciones utilizando Nginx y Apache Tomcat. Hemos creado dos contenedores independientes mediante comandos de Docker, asignando los puertos 8080 para Nginx y 8081 para Tomcat. También hemos aprendido a comprobar su estado, consultar sus registros y acceder a su contenido mediante diferentes comandos. Durante esta práctica surgieron algunos problemas, especialmente con Tomcat, pero finalmente conseguimos solucionarlos desplegando una aplicación web de ejemplo en formato WAR.

Gracias a todas estas actividades he podido comprender mejor cómo se prepara un entorno para desplegar aplicaciones web, desde la instalación de un sistema operativo hasta la configuración y puesta en funcionamiento de diferentes servidores. Considero que ha sido una unidad en la que hemos combinado teoría y práctica, lo que me ha ayudado a entender mejor los contenidos trabajados en clase.

![Aplicaciones Web](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ6hmMW5tKMcX6LqGju56eVKIt71wJIjch5eAnB1C2kIw&s=10)

## 2. ¿Qué no entiendo?

Todavía me cuesta comprender cómo funcionan conjuntamente los diferentes componentes de las arquitecturas web modernas. Aunque conozco qué son el frontend, el backend, las API, las bases de datos y los servidores, me gustaría entender mejor cómo se comunican entre sí y cómo trabajan conjuntamente dentro de una aplicación web real. También me gustaría conocer el recorrido que sigue una petición desde que el usuario accede a una página hasta que recibe la información solicitada.

Tengo algunas dudas sobre las diferencias entre un servidor web y un servidor de aplicaciones. Aunque en la práctica hemos utilizado Nginx como servidor web y Tomcat como servidor de aplicaciones, todavía me cuesta comprender del todo cuándo es necesario utilizar ambos, cómo se relacionan y qué ventajas ofrece utilizar un servidor web como proxy inverso para comunicarse con el servidor de aplicaciones. Me gustaría entender mejor cómo se configura esta comunicación en un entorno real.

Otra de las partes que me ha resultado algo complicada ha sido trabajar con Docker, especialmente cuando han surgido problemas durante la creación y configuración de los contenedores. Aunque he aprendido a utilizar comandos como docker run, docker start, docker ps, docker logs y docker exec, en ocasiones me ha costado identificar qué estaba fallando y saber qué comando debía utilizar para solucionarlo. Por ejemplo, durante la práctica de Tomcat, al principio no conseguía visualizar correctamente su contenido desde el navegador. Finalmente descubrimos que era necesario desplegar una aplicación web para poder acceder a ella, pero durante el proceso tuve algunas dificultades para entender dónde se almacenaban las aplicaciones y cómo funcionaba su despliegue dentro del contenedor.

Aunque finalmente he conseguido solucionar los problemas que fueron apareciendo durante la práctica, he decidido incluirlos en este apartado porque han sido algunas de las partes que más me han costado y en las que he tenido que invertir más tiempo para conseguir que todo funcionara correctamente.

Por último, también me gustaría comprender mejor las diferencias entre los distintos tipos de alojamiento web, especialmente entre un VPS y un servidor dedicado. Aunque entiendo sus características principales y las diferencias en cuanto a recursos y control, todavía tengo dudas sobre qué opción sería más adecuada en función del tipo de aplicación que se quiera desplegar, el número de usuarios que vaya a tener y los recursos que necesite.

![Nginx](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT7MhtMUiEAYbHpQpesHu0wjzh7HqLWEPa2Xp9mu6EOvQ&s=10)

## 3. ¿Qué es lo que más me ha gustado? ¿Y es lo que menos?

Lo que más me ha gustado de esta unidad ha sido la parte práctica relacionada con la virtualización y Docker, especialmente poder instalar Ubuntu en VirtualBox y trabajar posteriormente con contenedores. Me ha parecido interesante aprender cómo se puede disponer de un sistema operativo completo dentro de una máquina virtual y utilizarlo para realizar instalaciones y configuraciones sin tener que modificar directamente el sistema operativo principal del ordenador.

También me ha gustado bastante trabajar con Docker, me ha parecido muy útil descubrir cómo permite ejecutar diferentes servicios mediante contenedores independientes. Me ha resultado especialmente interesante poder instalar Nginx y Tomcat y comprobar desde el navegador que ambos servidores estaban funcionando correctamente. Me parece que es una forma bastante práctica de aprender cómo se despliegan aplicaciones web y cómo se pueden utilizar diferentes servicios dentro de un mismo sistema.

Además, me ha gustado que durante estas actividades no todo consistiera en seguir una serie de pasos y ejecutar comandos, sino que también tuviéramos que buscar soluciones cuando algo no funcionaba como esperábamos. Por ejemplo, durante la configuración de Tomcat tuvimos que consultar los registros del contenedor, revisar los directorios donde se almacenaban las aplicaciones y realizar diferentes comprobaciones hasta conseguir que apareciera correctamente el contenido en el navegador. Aunque he tenido que dedicar más tiempo del esperado a solucionar estos problemas, también me ha servido para aprender de ellos y entender mejor cómo funcionan las herramientas que hemos utilizado.

Por otro lado, lo que menos me ha gustado ha sido la parte en la que han surgido problemas durante las instalaciones y configuraciones, especialmente con Docker y Tomcat. En algunos momentos no tenía demasiado claro cuál era el origen del problema ni qué pasos debía seguir para solucionarlo, por lo que he tenido que probar diferentes comandos y realizar varias comprobaciones hasta conseguir que funcionara. También me ha resultado algo complicado diferenciar algunas de las funciones de los servidores web y los servidores de aplicaciones, ya que sus responsabilidades pueden estar relacionadas y no siempre me ha quedado completamente claro dónde termina el trabajo de uno y empieza el del otro.

![Tomcat](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR9Ohr1qT744L-ducZkKD0ukyKB4yLYYgnfS6hpWc0Gcw&s=10)

## 4. ¿Qué más me gustaría saber relacionado con la unidad?

Me gustaría profundizar más en el despliegue de aplicaciones web y conocer cómo se realiza este proceso en entornos reales, especialmente cómo se publica una aplicación para que otras personas puedan acceder a ella a través de Internet. También me gustaría aprender a configurar servidores como Apache o Nginx, utilizar dominios y certificados de seguridad HTTPS y comprender mejor cómo se conectan los diferentes servicios de una aplicación.

Por otro lado, me gustaría conocer más sobre la virtualización, ya que me ha parecido un tema interesante después de instalar Ubuntu en VirtualBox. Me gustaría aprender cómo funcionan los hipervisores, qué tipos de virtualización existen y qué otras posibilidades ofrecen las máquinas virtuales, tanto para trabajar con diferentes sistemas operativos como para crear entornos de pruebas y servidores. También me gustaría conocer mejor sus diferencias con los contenedores de Docker y cuándo resulta más conveniente utilizar cada uno.

Además, me gustaría profundizar en Docker, aprendiendo a crear mis propias imágenes y utilizar herramientas como Docker Compose para gestionar varios contenedores conjuntamente. También me interesa aprender más sobre la administración de servidores remotos mediante SSH y conocer cómo se configura un VPS para alojar una aplicación web.

En definitiva, me gustaría seguir aprendiendo sobre virtualización y despliegue de aplicaciones web para comprender mejor cómo se utilizan estas tecnologías en proyectos reales y conocer todas las posibilidades que ofrecen.

![Virtualización](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSVVHsM6fQryrk-FSD0Qe8OHq1w3cBP-9QKH08Wk69nZg&s=10)

