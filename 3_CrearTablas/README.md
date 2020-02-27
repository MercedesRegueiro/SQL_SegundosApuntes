<h1>Creacion de Tablas</h1>
1º Entramos en la instancia creada.<br/>
<img src="../imagenes/tablas1.PNG"/>
2º Vamos a la pestaña de <i>BROWSER</i> y ahí es donde creamos la tabla.<br/>
<img src="../imagenes/tablas2.PNG"/>
<h2>Sintaxis para crear tabla</h2>
CREATE TABLE "nombre_tabla"(<br/>
"columna 1" "tipo_de_datos_para_columna_1",<br/>
"columna 2" "tipo_de_datos_para_columna_2",<br/>
... <br/>
);<br/>
<h3><b>EJEMPLOS</b></h3>
<img src="../imagenes/tablas3.PNG"/>
<img src="../imagenes/tablas4.PNG"/>
<img src="../imagenes/tablas5.PNG"/>

<h2>Claves Primarias</h2>
Hay dos formas de hacerlo, hacerlo despues de crear las tablas o mientras la creas (Yo prefiero de esta segunda forma).<br/>
<h4><b>Primera forma</b></h4>
Debemos escribir lo siguiente:<br/>
ALTER TABLE "nombre_tabla" ADD PRIMARY KEY ("columna");
<img src="../imagenes/ClavePrimaria1.PNG"/>
<h4><b>Segunda forma</b></h4>
Cuando estamos creando la tabla es cuando se pone la clave primaria.<br/>
Para ello hay que escribir al lado del tipo de dato <i>PRIMARY KEY</i><br/>
<img src="../imagenes/ClavePrimaria.PNG"/>

<h2>Claves Ajenas</h2>
Hay dos formas de hacerlo, hacerlo mientras creas la tabla o despues de crearlas (Yo prefiero de esta segunda forma).<br/>
<h4><b>Primera forma</b></h4>
Mientras creamos la tabla debemos poner:<br/>
REFERENCES "nombre_tabla" ("columna")<br/>
<img src="../imagenes/ClaveAjena1.PNG"/>
<b>IMPORTANTE: Debemos crear las tablas de forma ordenada para que funcione.</b>
<h4><b>Segunda forma</b></h4>
Despues de crear todas las tablas debemos escribir lo siguiente:
ALTER TABLE "nombre_tabla"<br/>
ADD FOREIGN KEY ("columna") REFERENCES "nombre_tabla" ("columna");<br/>
<img src="../imagenes/ClaveAjena2.PNG"/>
<img src="../imagenes/ClaveAjena3.PNG"/>
<img src="../imagenes/ClaveAjena4.PNG"/>
<img src="../imagenes/ClaveAjena5.PNG"/>


