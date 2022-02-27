# JPA
Java Persistence API

¿Qué es JPA?
<ol>
<li>Es una API (Application Programming Interface) desarrollada principalmente para la plataforma Java EE.</li>
<li>Es la propuesta estándar que ofrece Java para implementar un Framework Object Relational Mapping (ORM), 
  que permite interactuar con la base de datos por medio de objetos.</li>
<li>JPA es el encargado de convertir los objetos Java en instrucciones para el Manejador de Base de Datos (MDB).</li>
</ol>

PROVEEDORES: Oracle, Redhat, Eclipse, etc que proporcionan nuevos productos mediante la adición de la persistencia.
Algunos de estos productos incluyen: Hibernate, Eclipselink, Toplink, ObjectDB, Open JPA, entre otros.
Se usará <b>eclipselink en su versión 2.1</b>

<h2>phpMyAdmin</h2>
Crear una base de datos--> Nombre: escuela (cotejamiento) --> CREAR.<br>
Sin crear ninguna tabla, nos vamos a la sección de Privilegios.<br>
<b>Agregamos cuenta de usuario:</b>
<ul>
  <li>Nombre de usuario: esc </li>
  <li>Nombre de host (cualquier servidor) : % (el signo porcentaje da todos los permisos) </li>
  <li>Contraseña : 12345 </li>
  <li>Autenticación de MySQL nativo </li>
  <li>Dar todos los permisos de Datos, Estructura, Administración. </li>
  <li>CONTINUAR</li>
</ul>

<h2>Netbeans</h2>
<ul>
  <li>New proyect -> Java -> Java Application --> Nombre: testJPA</li>
  <li>A la izquierda tenés: Proyects / Files / Services </li>
  <li>Para crear conexión de Base de Datos. Entras a Services. </li>
    <ol>
      <li>Databases --> Click Derecho --> New Connection.</li>
      <li>Elegimos el Driver: MySQL (Connector/J driver) --> Sino está agreagarlo.</li>
      <li>Host: localHost --> Port: 3306 </li>
      <li>Database: escuela </li>
      <li>User Name: esc </li>
      <li>Password: 12345 </li>
      <li>JDBC: jsbc:mysql.../escuela?serverTimezone=UTC</li>
      <li>Finish</li>
    </ol>
  <li>Volvemos a Proyects y: En librerias --> Click derecho -->Add JAR/Folder</li>
  <li>Agrego archivo: mysql-connection-java-5.1.23-bin</li>
</ul>
<li>En testJPA --> New -->Persistence Unit</li>
<li>Paso1:En caso de no aparecer ir a OTHER --> Carpeta Persistence Unit -> Persistence Unit --> Next</li>
<li>Paso2:Nombre: testJPAPU (Persistence Unit)</li>
<li>Persitence Librery: EclipseLink(JPA 2.1)</li>
<li>DataBase Connection: jdbc:mysql://...escuela?serverTimezone=UTC --> Finish</li>


  




