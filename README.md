# ArteLine
### Software Engineering subject project

#### Introducción

El avance de la tecnología en los últimos años ha dado lugar al surgimiento de la experiencia de mercado con mejores aportes de valor para el cliente y mejores plazas para los propietarios. Esta nueva modalidad de hacer negocios ha causado gran controversia con el método tradicional; la compra y venta de servicios y productos realizadas de manera presencialfrente al comercio electrónico basado en las ventas online.
Debido alafuerte demanda de usuarios que prefieren esta experiencia, la empresa ArtLine ha decidido optimizar sus procesos de venta haciendo uso del comercio electrónico con el fin de mejor la experiencia de sus clientes al realizar compras de cualquier tipo de obra de arte, además de generar una mejora en el proceso de administración de las mismas obras de arte.
Gracias a la Ingeniería de software que de acuerdo a Pressman, es el estudio de los principios y metodologías para el desarrollo y mantenimiento de sistemas de software, es posible crear un sistema de manera óptima con base a las necesidades y requerimientos que los clientes desean.
Con ayuda del sistema la empresa se verá beneficiada en distintos aspectos ya que podrán reducir costos al invertir menos en publicidad y ampliar sus mercados, de igual manera sus productos estarán disponibles los 7 días de la semana y 24 horas del día, lo cual mejora la comodidad del cliente al no verse limitado por un horario en específico.




#### Objetivo general

Construiruna aplicación web para la empresa ArteLine, para mejorar el control del almacenamiento de las obras de arte y poder optimizar el proceso de venta.
Problemática

Actualmente la empresa ArteLine se dedica a la venta y exposición de obras de arte visuales, realizando de manera manual todos los procesos, provocando saturación de información, haciendo más difícil el trabajo y procesamiento de la misma, generando errores por parte de los empleados. Además, únicamente se realizan ventas de manera física y al no contar con un registro de las obras vendidas ni las existentes en su almacén, los clientes adquieren obras que no están disponibles, provocando a la empresa una pérdida económica y poca satisfacción con los clientes y obligándolos de una manera a adquirir obras en otras empresas.
Justificación del proyecto

En la empresa ArteLine, cuya problemática se basa en la necesidad de implementar un software que les ayude a procesar su información de forma correcta, es pertinente implementar una solución donde se cambien estas metodologías convencionales de registros de datos por métodos digitales y ágiles, obteniendo un beneficio total para la empresa,ya que el empleado será capaz de agilizar sus procesos de ventas de artículos y disminuirá la posibilidad de escribir datos erróneos ya que en el software se establecerán formatos fijos para el registro de datos, lo cual permitirá que el empleado solo haga uso de información básica de la obras de arte; mientras que el dueño, con laimplementación de este software, se centra en la obtención de reportesacertados, un mejor control y organización de la información, tanto del catálogo como de las ventas de cada producto de la tienda, esto le permite la toma de decisiones futuras; por su parte el cliente podrá ver información real de las obras disponibles, facilitando la adquisición de las obras, en caso de que se necesite una devolución o requiera presentar una queja, podrá realizarlo de manera digital, sin la necesidad de acudir a la tienda.
Descripción de procesos principales

Registro del personal: Registrar a cada uno de los empleados que laboran en la tienda ArteLine
Reglas de negocio:
-	Cada empleado contara con una clave única para acreditar su pertenencia a la tienda.
-	Los empleados deberán proporcionar información personal, como nombre completo, edad, sexo, dirección y número telefónico para poder ser registrados.
-	Se deberán indicar el departamento al que pertenecen.
-	Solo los administradores podrán registrar a nuevos empleados o en su defecto darlos de baja.

Registro y almacenamiento de obras de arte: Registrar en un formulario las obras con los que se cuenta en el almacén de la tienda.
Reglas de negocio:
-	Todas las obras de arte deberán contar con un código único para su identificación.
-	Cada registro irá acompañado de la información de la obra, como tipo, autor, época y si es local o extranjera y precio.
-	Se establecerá el lugar de almacenamiento.
-	Registrar los nuevos productos que llegan al almacén.
-	Notificar cuando un producto haya sido vendido, para que no aparezca más en exhibición.

Clasificación de obras de arte: Las obras podrán ser clasificadas mediante sus atributos, este proceso no tiene interfaz gráfica.
	Reglas de negocio:
-	Se permitirá categorizar las obras mediante los siguientes índices: tipo de obra, autor, remates, líneas de tiempo, época y si es local o extranjera.
-	No se permitirá agregar más categorías.
-	La clasificación solo será visible al momento de consultar el inventario y generar reportes.
-	Mostrará el estatus de las obras de arte, si están disponibles o no.


Generación de venta: Este proceso cuenta con un formulario en donde se registrarán las ventas individuales de las obras.
Reglas de negocio:
-	Se requerirán los siguientes datos: Código de la obra, fecha y hora de la venta, nombre, e-mail y teléfono del comprador.
-	Se creará un registro de venta por cada obra, es decir, si el cliente compra más de una obra, se harán los respectivos registros de cada una.
-	Se creará una factura virtual, la cual será enviada al correo.
-	Una vez confirmada la venta, ésta no será modificable

Modificación de obras: Formulario de actualización de información sobre las obras disponibles.
Reglas de negocio:
-	No se podrá modificar el código de identificación de la obra.
-	No se podrán eliminar las obras, solo se podrán marcar como inhabilitadas.

Generación de reportes: Formulario donde se podrán crear los reportes de ventas.
Reglas de negocio:
-	Cada reporte deberá incluir las obras vendidas, para ello se hará uso del código de identificación.
-	Los reportes se generarán mediante un rango de fechas.
-	Los reportes se podrán generar de acuerdo a las categorías previamente mencionadas.
-	Los reportes podrán ser guardados como PDF o enviados por correo.
-	Se podrán crear reportes programados automáticos cada rango de tiempo.

Estimación de esfuerzo-COCOMO

-	Calculo de Kilo líneas de códigos:
Se trabajará con C#, por lo cual las líneas de código por cada PF son igual a 74, entonces:
` KLDC= (261,36 * Líneas de código por cada PF) /1000 = (261,36*74) /1000= 19.34064 KDLC `

-	Calculo de variable FAE:

Conductores de costo | Muy bajo|	Bajo | Nominal | Alto | Muy alto | Extra alto
-------------------- | --------|----- | ------- | ---- | -------- |-----------
Fiabilidad requerida del software | 0.75 | 0.88 | 1.00 | 1.15 |	1.40 |	--
Tamaño de la base de datos |	--	|0.94	|1.00|	1.08|	1.16|	--
Complejidad del producto|	0.70|	0.85|	1.00|	1.15|	1.30	|1.65
Restricciones del tiempo de ejecución |	--	|--|	1.00|	1.11	|1.30|	1.66
Restricciones del almacenamiento principal	|--|	--|	1.00|	1.06	|1.21|	1.56
Volatilidad de la máquina virtual	|--	|0.87|	1.00|	1.15|	1.30|	--
Tiempo de respuesta del ordenador	|--	|0.87|	1.00|	1.07|	1.15	|--
Capacidad del analista|	1.46	|1.19	|1.00|	0.86	|0.71	|--
Experiencia en la aplicación	|1.29	|1.13|	1.00|	0.91|	0.82|	--
Capacidad de los programadores	|1.42|	1.17|	1.00|	0.86|	0.70|	--
Experiencia en S.O. utilizado	|1.21|	1.10	|1.00|	0.90|	-- 	|--
Experiencia en el lenguaje de programación	|1.14|	1.07|	1.00|	0.95|	--|	--
Prácticas de programación modernas	|1.24|	1.10|	1.00|	0.91|	0.82|	--
Utilización de herramientas software	|1.24|	1.10|	1.00|	0.91|	0.83	|--
Limitaciones de planificación del proyecto|	1.23	|1.08|	1.00|	1.04|	1.10|--
#### Tabla 1. Conductores de costo
##### Fuente Propia


El valor de la variable FEA se obtiene al multiplicar los valores fijados en la tabla de conductores de costo:

`FEA= (1.15*1.00*0.85*1.11*1.00*1.00*1.07*0.86*0.91*0.70*1.00*0.95*1.00*0.91*1.08)=0.593`


Justificación de los Valores:

-	Atributos de Software:
-	Fiabilidad requerida del software:
Si se generan errores en la compra-venta de una obra perdidas económicas para la empresa (valoración alta 1.15).  
-	Tamaño de la base de datos:
Se utilizará una base de datos de tamaño  estándar para controlar el almacenamiento de la información y llevar acabo los diferentes procesos (valoración nominal 1.00).
-	Complejidad del producto:
No se harán cálculos complejos, solo es almacenamiento, compra y venta (valoración baja 0.85).
-	Atributos de Hardware:
-	Restricciones del tiempo de ejecución:
El sistema requiere que  las respuestas se den en tiempo real para evitar errores con los clientes (valoración alta 1.11).
-	Restricciones del almacenamiento principal:
Existen pocas limitaciones en el almacenamiento a utilizar (valoración nominal 1.00).
-	Volatilidad de la máquina virtual:
Se usará el entorno de desarrollo Windows (valoración nominal 1.00).
-	Tiempo de respuesta del ordenador:
Se requiere de una rápida respuesta para no perjudicar las operaciones realizadas por los usuarios (valoración alta 1.07).

-	Atributos del personal:
-	Capacidad del analista:
Capacidad de comprensión para poder detectar problemas y posibles soluciones, basado en su experiencia con proyectos similares (valoración alta 0.86).
-	Experiencia en la aplicación:
Habilidades y técnicas basadas en proyectos anteriores para poder brindar soluciones (valoración alta 0.91).
-	Capacidad de los programadores:
Los programadores deben tener los conocimientos y habilidades en el lenguaje de programación que se empleara para el proyecto (valoración  muy alta 0.70).
-	Experiencia en los S.O utilizados:
Conocimiento básico el uso de  Windows 10 Professional (valoración nominal 1.00).
-	Experiencia en lenguaje de programación
Se requiere  de una amplia experiencia en el lenguaje a utilizar, debido a que en la programación se codificará el funcionamiento del sistema (valoración muy alta 0.95).

-	Atributos del proyecto
-	Practica de programación moderna:
Se aplicaran los conocimientos  de programación convencional (valoración nominal 1.00).
-	Utilización de herramientas de software:
Se debe de contar con cierta experiencia en el uso de herramientas estándar (valoración alta 0.91).
-	Limitación de planificación de proyecto:
No se presentan limitaciones (valoración baja 1.08).


-	Calculo del esfuerzo del desarrollo:
```E=Esfuerzo=aKLCDe*FAE (personas*mes)
KLDC=19.340
FAE=0.771
E=3.2 (19.340)1.05*(0.593)=42.658
```
-	Calculo de tiempo de desarrollo:
```
T=Tiempo Duración Desarrollo=cEsuerzod(mes)
2.5(42.658)0.38=10.405
```

-	Calculo de productividad:
```
PR=Productividad=LCD/Esfuezo
19340/42.658=453.373
```
-	Calculo de personal promedio:
```
P=Personal=Esfuerzo/Tiempo(personas)
P=42.658/11.48=3.7
```
Por lo tanto, el equipo se conformará por 4 personas, que trabajaran en un lapso de 10 meses, sin embargo el proyecto debe terminarse en 4 meses, por lo que será necesario adquirir más personal, generando un total de 7 personas laborando en 4 meses.
El equipo deberá conformarse por: 1 líder de proyecto, 2 analistas ,2 diseñadores de base de datos, 2 programadores y 1 tester.






#### Conclusiones

Según el análisis realizado al sistema que está empleado en ArteLine, todos sus problemas se enfocan en la necesidad de implementación de un sistema de información, en donde, según la descripción de procesos principales, resulta ser un software técnicamente factible, es decir, no requiere un sitio de alojamiento de base de datos y aplicación Web especial y su implementación está dentro de las herramientas Web disponibles; por lo tanto el sistema de información podrá ser implementado sin ningún tipo de complicación o requerimiento especial.
