#Sistema Control Votaciones

Paradigma: hìbrido, OO, Estructurado.
Lenguajes: Java, MySQL.

#Descripción breve
Desarrollo de un sistema de información computacional para la automatización de procesos en actividades de un escenario de votaciones en sistemas de red de tipo cliente-servidor 

#Descripción detallada

El desarrollo de este software se encuentra basado en la metodología orientada a objetos propuesta en Alfredo Weitzenfeld en su libro “Ingeniería de Software Orientada a Objetos con UML, Java e Internet”, por lo que se ha desarrollado en el lenguaje de programación java.

Para la base de datos, se ha hecho uso del lennguaje MySQL en apoyo del gestor MariaDB, como requisito funcional explícito.

El sistema esta desarrollado en base a un enfoque de microservicios, por lo que puede ser utilizado de forma modular tanto a nivel cliente como a nivel servidor permitiendo la escalabilidad e independencia de su funcionamiento.

 Lista de requisitos funcionales (creación, inserción y/o carga, consultas).
1.	Lista de requisitos de almacenamiento.
•	El sistema debe permitir a un votante la capacidad de consultar a sus candidatos correspondientes a su sección por medio del ingreso de su clave electoral y/o credenciales de acceso.
•	El sistema debe permitir a un votante seleccionar a los candidatos correspondientes a cada candidatura de la sección del votante.
•	El sistema debe permitir al votante corroborar su voto visualizando la boleta, antes de ser realizada la confirmación.
•	El sistema debe permitir al operador de cómputo la captura del registro de los candidatos.
•	El sistema debe permitir al operador de cómputo la captura del registro de los votantes.
•	El sistema debe permitir al operador de cómputo la captura del registro de los partidos políticos.
•	El sistema debe permitir al operador de cómputo la captura del registro de las casillas.
•	El sistema debe permitir al operador de cómputo la asignación de los funcionarios de casilla.
•	El sistema debe permitir al operador de cómputo elegir la anulación de una boleta o de una casilla junto a sus respectivas boletas.
•	El sistema debe permitir al operador de computo la consulta de boletas por folio.
•	El sistema debe permitir al operador de cómputo consultar el conteo de votos por casilla, por candidato, candidatura y por fecha.
•	El sistema debe permitir al operador de cómputo consultar el conteo de votos por candidato, fecha y candidatura.
•	
2.	Lista de requisitos de procesamiento (procesos aplicados a los datos para obtener información).
•	El sistema debe ser capaz de realizar la validación de las credenciales de acceso y dirigir al usuario operador o funcionario a su caso de uso correspondiente.
•	El sistema debe ser capaz de realizar la consulta de electores por medio de la clave electoral y/o credenciales de acceso.
•	El sistema debe ser capaz de ordenar los datos del registro de los votantes, ordenarlos y enviarlos al servidor para dejar el registro en espera, posteriormente retornar la boleta con los registros que serán realizados para después de recibir la confirmación por parte del usuario, retornar la señal de confirmación hacia el servidor y hacia el sistema de almacenamiento.
•	El sistema debe ser capaz de discriminar, reestructurar y trasladar, en cuanto a lo necesario, el registro de nuevos electores hacia el sistema de almacenamiento.
•	El sistema debe ser capaz de discriminar, reestructurar y trasladar, en cuanto a lo necesario, el registro de nuevos candidatos hacia el sistema de almacenamiento.
•	El sistema debe ser capaz de discriminar, reestructurar y trasladar, en cuanto a lo necesario, el registro de nuevos funcionarios hacia el sistema de almacenamiento.
•	El sistema debe ser capaz de discriminar, reestructurar y trasladar, en cuanto a lo necesario, el registro de nuevos Operadores de cómputo hacia el sistema de almacenamiento.

•	El sistema debe ser capaz de extraer la información de cada boleta del sistema de almacenamiento para trasladarlos a la interfaz de usuario.
•	El sistema debe ser capaz de extraer la información de cada candidato del sistema de almacenamiento para trasladarlos a la interfaz de usuario.
•	El sistema debe ser capaz de corroborar la información de un votante, de un funcionario de casilla o de un operador de cómputo consultándola en el sistema de almacenamiento para trasladarlos a la interfaz de usuario.
•	El sistema debe ser capaz de corroborar la información de una casilla con sus respectivos funcionarios y, en caso de requerirse, electores, consultándola en el sistema de almacenamiento para trasladarlos a la interfaz de usuario.
•	El sistema debe ser capaz de consultar un conteo de votos por candidato, un conteo de votos por casilla, un conteo de votos por partido, un conteo de votos por estado y partido, un conteo de votos totales, un conteo de votos nulos y un conteo de casillas anuladas.

Lista de requisitos no funcionales
1.	explícitos (solicitados expresamente por el cliente).
•	El sistema no debe permitir vínculos directos de qué votante votó por cuál candidato.
2.	implícitos (Relacionados con estándares del grupo de desarrollo).
•	El sistema debe ser capaz de administrar la base de datos con actualizaciones, modificaciones, respaldo.
•	Se debe contar con una bitácora de instrucciones insertadas en el sistema.
•	El sistema debe ser modulado, de tal manera que pueda ser soportada sin conexión constante al sistema completo o al servidor central.

https://github.com/AoNiRoCo/SistemaControlVotaciones_POO_Java_MySQL/blob/7db1690f1672be9f6627514b5825c59da83f9b3e/Delimitaci%C3%B3nYArquitecturaDelSistema.png
