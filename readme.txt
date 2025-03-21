Instrucciones para un Código Claro y Documentado en XML
1. Encabezado de Documentación
Cada archivo XML debe comenzar con un encabezado de documentación utilizando comentarios:

Ejemplo de encabezado en XML:
<!--
Nombre: [Nombre del Alumno]
Curso: [Nombre del Curso]
Fecha: [DD/MM/AAAA]
Ejercicio: [Título del Ejercicio]
-->

2. Uso de Comentarios en XML
Los comentarios deben explicar la estructura y propósito de cada parte del código XML.

Ejemplo:
<!-- Definición de una persona -->
<persona>
    <nombre>Juan Pérez</nombre>
    <edad>30</edad>
    <ciudad>Madrid</ciudad>
</persona>

3. Control de Modificaciones y Fechas
Si se hacen cambios en el código XML, se deben registrar con comentarios indicando la fecha y la descripción del cambio.

Ejemplo:
<!--
Fecha: 12/02/2025
Cambio: Se agregó el campo correo-electronico
-->
<persona>
    <nombre>Juan Pérez</nombre>
    <edad>30</edad>
    <ciudad>Madrid</ciudad>
    <correo-electronico>juan@example.com</correo-electronico>
</persona>
