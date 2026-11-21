# Diario de clase - UD2: Introducción a las Aplicaciones Web
## 1. ¿Qué he aprendido?

En esta unidad he aprendido diferentes conceptos relacionados con las aplicaciones web, su funcionamiento y los elementos necesarios para desplegarlas. He conocido mejor el protocolo HTTP (HyperText Transfer Protocol), que se utiliza para la comunicación entre clientes y servidores web, y su diferencia con HTTPS, que ofrece una mayor seguridad al cifrar la información que se transmite. También he aprendido cuál es la función de los servidores web, especialmente Apache, y cómo instalarlo y comprobar su funcionamiento en Ubuntu, utilizando comandos desde la terminal.

Además, he aprendido qué es una arquitectura cliente-servidor, cómo se comunican ambas partes y las diferencias entre las arquitecturas de dos y tres capas. También hemos visto los principales componentes de una arquitectura web moderna, como el frontend, el backend, las API, las bases de datos y los servidores web. Por otro lado, he aprendido qué es el protocolo FTP, para qué se utiliza y en qué se diferencia de SFTP, que ofrece una mayor seguridad mediante el cifrado de las comunicaciones con SSH. También hemos estudiado los diferentes tipos de alojamiento web, como el compartido, los VPS y los servidores dedicados.

He aprendido más sobre los diferentes modelos de arquitectura web y cómo se organizan sus componentes, así como los distintos tipos de alojamiento web, como el compartido, los VPS y los servidores dedicados, conociendo sus diferencias y características principales. También he trabajado con los servidores y clientes FTP, aprendiendo para qué sirven y cómo permiten transferir archivos entre equipos. Por último, he conocido la diferencia entre FTP y SFTP, siendo este último más seguro porque cifra las comunicaciones mediante SSH.

En cuanto a la parte práctica, hemos empezado trabajando con la virtualización, instalando Ubuntu 24.04 LTS en VirtualBox. He aprendido a crear y configurar una máquina virtual y a instalar las Guest Additions, que permiten mejorar la integración entre Ubuntu y VirtualBox, por ejemplo, adaptando automáticamente la resolución de pantalla.

Otra de las actividades ha sido la instalación de Docker en Ubuntu. He aprendido qué son los contenedores, cuáles son sus ventajas y en qué se diferencian de las máquinas virtuales. También hemos instalado Docker Desktop y comprobado que funciona correctamente mediante la ejecución del contenedor hello-world.

Por último, hemos trabajado con la instalación de servidores web y de aplicaciones utilizando Nginx y Apache Tomcat. Para ello, hemos creado dos contenedores independientes con Docker, utilizando los puertos 8080 para Nginx y 8081 para Tomcat. También hemos aprendido a comprobar su funcionamiento, consultar sus registros y utilizar diferentes comandos para gestionar los contenedores. Durante esta práctica surgieron algunos problemas, especialmente con Tomcat, pero finalmente conseguimos solucionarlos desplegando una aplicación web de ejemplo.

Gracias a estas actividades he podido conocer mejor cómo funcionan las herramientas que se utilizan para desplegar aplicaciones web y poner en práctica algunos de los conceptos que hemos estudiado en clase.

![Aplicaciones Web](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ6hmMW5tKMcX6LqGju56eVKIt71wJIjch5eAnB1C2kIw&s=10)

## 2. ¿Qué no entiendo?

Todavía me cuesta comprender cómo funcionan conjuntamente los diferentes componentes de las arquitecturas web modernas. Aunque conozco qué son el frontend, el backend, las API, las bases de datos y los servidores, me gustaría entender mejor cómo se comunican entre sí y cómo trabajan conjuntamente dentro de una aplicación web real. También me gustaría conocer el recorrido que sigue una petición desde que el usuario accede a una página hasta que recibe la información solicitada.

Tengo algunas dudas sobre las diferencias entre un servidor web y un servidor de aplicaciones. Aunque en la práctica hemos utilizado Nginx como servidor web y Tomcat como servidor de aplicaciones, todavía me cuesta comprender del todo cuándo es necesario utilizar ambos, cómo se relacionan y qué ventajas ofrece utilizar un servidor web como proxy inverso para comunicarse con el servidor de aplicaciones. Me gustaría entender mejor cómo se configura esta comunicación en un entorno real.

Otra de las partes que me ha resultado algo complicada ha sido trabajar con Docker, especialmente cuando han surgido problemas durante la creación y configuración de los contenedores. Aunque he aprendido a utilizar comandos como docker run, docker start, docker ps, docker logs y docker exec, en ocasiones me ha costado identificar qué estaba fallando y saber qué comando debía utilizar para solucionarlo. Por ejemplo, durante la práctica de Tomcat, al principio no conseguía visualizar correctamente su contenido desde el navegador. Finalmente descubrí que era necesario desplegar una aplicación web para poder acceder a ella, pero durante el proceso tuve algunas dificultades para entender dónde se almacenaban las aplicaciones y cómo funcionaba su despliegue dentro del contenedor.

Aunque finalmente he conseguido solucionar los problemas que fueron apareciendo durante la práctica, he decidido incluirlos en este apartado porque han sido algunas de las partes que más me han costado y en las que he tenido que invertir más tiempo para conseguir que todo funcionara correctamente.

Por último, también me gustaría comprender mejor las diferencias entre los distintos tipos de alojamiento web, especialmente entre un VPS y un servidor dedicado. Aunque entiendo sus características principales y las diferencias en cuanto a recursos y control, todavía tengo dudas sobre qué opción sería más adecuada en función del tipo de aplicación que se quiera desplegar, el número de usuarios que vaya a tener y los recursos que necesite.

![Nginx](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT7MhtMUiEAYbHpQpesHu0wjzh7HqLWEPa2Xp9mu6EOvQ&s=10)

## 3. ¿Qué es lo que más me ha gustado? ¿Y es lo que menos?

Lo que más me ha gustado de esta unidad ha sido la parte práctica relacionada con la virtualización y Docker. Me ha parecido interesante aprender a instalar Ubuntu en VirtualBox y poder trabajar con otro sistema operativo sin tener que instalarlo directamente en el ordenador. También me ha gustado descubrir cómo funciona Docker y cómo permite ejecutar diferentes servicios mediante contenedores independientes.

Me ha resultado especialmente interesante la práctica de Nginx y Tomcat, ya que hemos podido instalar ambos servidores y comprobar desde el navegador que funcionaban correctamente. Me parece una forma bastante práctica de entender cómo se despliegan aplicaciones web y cómo se utilizan diferentes herramientas para conseguirlo.

También me ha gustado que durante las prácticas tuviéramos que buscar soluciones cuando algo no funcionaba como esperábamos. Por ejemplo, durante la configuración de Tomcat tuvimos que revisar los registros y comprobar dónde se almacenaban las aplicaciones hasta conseguir que apareciera el contenido en el navegador. Aunque he tenido que dedicar más tiempo del esperado a solucionar estos problemas, también me ha servido para aprender de ellos y entender mejor cómo funcionan las herramientas que hemos utilizado.

Por otro lado, lo que menos me ha gustado ha sido encontrarme con tantos problemas durante algunas instalaciones y configuraciones, especialmente con Docker y Tomcat. En ocasiones no tenía claro cuál era el origen del error y tenía que probar diferentes comandos hasta conseguir solucionarlo. También me ha resultado algo complicado diferenciar las funciones de los servidores web y los servidores de aplicaciones, ya que al principio me costaba entender qué hacía cada uno.

![Tomcat](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR9Ohr1qT744L-ducZkKD0ukyKB4yLYYgnfS6hpWc0Gcw&s=10)

## 4. ¿Qué más me gustaría saber relacionado con la unidad?

Me gustaría profundizar más en el despliegue de aplicaciones web y conocer cómo se publican en servidores reales para que otras personas puedan acceder a ellas a través de Internet. También me gustaría aprender a configurar servidores como Apache o Nginx, utilizar dominios y certificados HTTPS y comprender mejor cómo se conectan los diferentes servicios de una aplicación.

Por otro lado, me gustaría conocer más sobre la virtualización, ya que me ha parecido un tema interesante después de instalar Ubuntu en VirtualBox. Me gustaría aprender cómo funcionan los hipervisores, qué otros tipos de virtualización existen y qué ventajas ofrecen las máquinas virtuales. También me gustaría comprender mejor sus diferencias con los contenedores de Docker y cuándo conviene utilizar cada uno.

Además, me interesa aprender a utilizar Docker de forma más avanzada, crear mis propias imágenes y utilizar herramientas como Docker Compose para gestionar varios contenedores conjuntamente. También me gustaría conocer mejor cómo se administran servidores remotos mediante SSH y cómo se configura un VPS para alojar aplicaciones web.

En definitiva, me gustaría seguir aprendiendo sobre virtualización y despliegue de aplicaciones web para conocer mejor cómo se utilizan estas herramientas en proyectos reales y descubrir todas sus posibilidades.

![Virtualización](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSVVHsM6fQryrk-FSD0Qe8OHq1w3cBP-9QKH08Wk69nZg&s=10)

