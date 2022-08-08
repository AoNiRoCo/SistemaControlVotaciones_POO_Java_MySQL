## Espacio para la documentación referente a a la base dedatos

Lenguaje MySQL
Aplicado en la herramienta MariaDB

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
•	El sistema debe permitir al operador de cómputo la consulta de boletas por folio.
•	El sistema debe permitir al operador de cómputo consultar el conteo de votos por casilla, por candidato, candidatura y por fecha.
•	El sistema debe permitir al operador de cómputo consultar el conteo de votos por candidato, fecha y candidatura.
Especificación modular 
Diseño lógico del almacenamiento
Entidades

![Matriz relaciones](BaseDeDatos/MatrizDeRelaciones.png)
![Captura Entidadees](https://github.com/AoNiRoCo/SistemaControlVotaciones_POO_Java_MySQL/blob/master/BaseDeDatos/Entidades.png?raw=true)

Descripción de las relaciones

Cada CREDENCIAL puede ser identificación de uno o más FOTOPERSONA.
Cada CREDENCIAL debe ser identificador de un y sólo un CANDIDATO.	
Cada CREDENCIAL debe ser identificador de un y sólo un FUNCIONARIO.
Cada CREDENCIAL puede ser concentrada en una y sólo una CASILLA.
Cada PARTIDOPOLITICO debe ser representado por uno o más CANDIDATO.
Cada FOTOPERSONA debe ser identificación de un y sólo un CREDENCIAL.
Cada CANDIDATO debe ser poseedor de un y sólo un CREDENCIAL.
Cada CANDIDATO puede ser representante de uno o más PARTIDOPOLITICO.
Cada CANDIDATO puede ser representado en uno o más BOLETA.
Cada BOLETA puede ser manifiesto de uno o más CANDIDATO.
Cada BOLETA debe ser consignada a uno o más CASILLA.
Cada FUNCIONARIO debe ser identificado por un y sólo un CREDENCIAL.
Cada FUNCIONARIO puede ser operador de una y sólo una CASILLA.
Cada CASILLA puede ser acopio de uno o más BOLETA.
Cada CASILLA puede ser concentrado de uno o más CREDENCIAL.
Cada CASILLA puede ser operado por un uno o más FUNCIONARIO.
Diagrama de Entidad-Relación

![Diagrama E-R](https://github.com/AoNiRoCo/SistemaControlVotaciones_POO_Java_MySQL/blob/master/BaseDeDatos/DiagramaEntidadRelacion.png?raw=true)


