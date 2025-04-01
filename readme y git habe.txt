LENGUAJES DE MARCAS - XML
05.02. Validación XML - DTD II
Ejercicio 1. Factura electrónica.
Diseña un documento XML que represente una factura electrónica para una transacción
comercial entre una librería y una biblioteca.
La factura debe contener la información del número y fecha de emisión, así como los
datos del emisor y el cliente. Además, debe incluir un detalle de los productos vendidos,
especificando el código del artículo, su tipo, descripción, cantidad y precio de venta por
unidad. Algunos productos pueden tener una oferta aplicada.
El documento debe estar validado mediante una DTD, el detalle es el siguiente:
• Elemento factura:
• Debe contener los elementos datos-emisor, datos-cliente y detalle-
factura.
• Tiene dos atributos obligatorios: numero y fecha.
• Elementos datos-emisor y datos-cliente:
• Ambos elementos deben contener los elementos nombre, cif y telefono.
• Elementos nombre, cif y telefono:
• Son elementos de texto simple (#PCDATA), es decir, solo pueden
contener caracteres de texto.
• Elemento detalle-factura:
• Debe contener uno o más elementos linea.
• Tiene un atributo obligatorio llamado importe.
• Elemento linea:
• Debe contener los elementos descripcion, cantidad y pvp.
• Tiene dos atributos obligatorios: codigo-articulo y tipo.
• codigo-articulo debe ser un identificador único (ID).
• tipo puede tomar los valores "Libro", "DVD" o "Varios".
• Elemento descripcion, cantidad y pvp:
• Son elementos de texto simple (#PCDATA).
• Elemento oferta:
• Es un elemento vacío que puede aparecer opcionalmente dentro del
elemento linea.
Ejercicio 2. Equipos NBA.
Diseña un documento XML que contenga información sobre equipos de la NBA,
incluyendo sus títulos, posición y quinteto titular.
Cada equipo debe ser identificado por su nombre y debe especificarse su conferencia
(división en la que está inscrito un equipo dentro de la NBA. La NBA está dividida en dos
conferencias principales: la Conferencia Este y la Conferencia Oeste). Además, se debe
detallar el número de títulos ganados por el equipo, su posición en la clasificación y el
quinteto titular.
LENGUAJES DE MARCAS - XML
La DTD debe establecer las siguientes restricciones para la estructura y contenido del
documento XML:
• El elemento raíz debe ser EquiposNBA, que contiene uno o más elementos
equipo o nombre.
• El elemento nombre contiene el nombre de un equipo.
• El elemento equipo contiene la información detallada de un equipo, incluyendo
sus títulos, posición y quinteto titular.
• El elemento equipo tiene un atributo obligatorio llamado conferencia, que
especifica la conferencia a la que pertenece el equipo.
• Los elementos titulos, posicion y quinteto contienen información sobre los títulos
ganados, posición en la clasificación y quinteto titular de un equipo,
respectivamente.
• Elemento EquiposNBA:
• Este es el elemento raíz que contiene la información sobre los equipos
de la NBA.
• Puede contener una secuencia de elementos equipo o nombre.
• Elemento nombre:
• Contiene el nombre de un equipo de la NBA.
• Es un elemento de texto simple (#PCDATA).
• Elemento equipo:
• Contiene información detallada sobre un equipo, incluyendo sus títulos,
posición y quinteto titular.
• Tiene un atributo obligatorio llamado conferencia, que especifica la
conferencia a la que pertenece el equipo.
• Atributo equipo conferencia:
• Este atributo especifica la conferencia a la que pertenece el equipo (por
ejemplo, "este" u "oeste").
• Es un atributo de tipo CDATA (datos de caracteres).
• Elemento titulos:
• Contiene el número de títulos ganados por el equipo.
• Es un elemento de texto simple (#PCDATA).
• Elemento posicion:
• Contiene la posición del equipo en la clasificación.
• Es un elemento de texto simple (#PCDATA).
• Elemento quinteto:
• Contiene el quinteto titular del equipo.
• Es un elemento de texto simple (#PCDATA).
Ejercicio 3. Aeropuerto.
Escribir un documento XML con una DTD externa que represente la siguiente
información:
LENGUAJES DE MARCAS - XML
Especificaciones de la DTD:
Hay que guardar el nombre del aeropuerto, los datos de cada vuelo agrupados y la fecha
del panel, en ese orden.
Sólo el código de un vuelo y su estado deben representarse mediante atributos. El código
ha de ser único y obligatorio para cada vuelo.
Para cada vuelo se tiene que guardar la información en el mismo orden en el que aparece
en el panel.
En la DTD debe indicarse que al menos tiene que aparecer un vuelo.
Los posibles estados de un vuelo son C (Cancelado), E (En hora), R (Retrasado). El valor
por defecto debe ser E.
Para indicar si un vuelo es diario, se debe utilizar un elemento vacío que, respecto a cada
vuelo, podrá aparecer (en el caso de sí ser diario) o no aparecer (en el caso contrario)

https://github.com/nrcb28/reimagined-palm-tree.git
