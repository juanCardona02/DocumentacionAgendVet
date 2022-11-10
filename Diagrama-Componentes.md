# Diagrama de Compomentes

Permite identificar las dependecias lógicas y los artefactos que se van a usar para la implemetanción del agendamiento de citas para la veteriniaria.

Este diagrama indica que el lenguaje de desarrollo será Java, con la utilización del framework Spring.

En dicho diagrama, existen seis compomentes lógicos, de cuales:
 - El adaptador depende del servicio y de los Objeto de transferencia de datos.
 - El servicio depende del dominio, de la infraestructura y de la entidad.
 - La infraestructura depende del servicio.

**Diagrama de Compomentes**
<br>
<img src="/Images/Diagrama-Componentes/DiagramaComponentes.png" alt="Diagrama de Compomentes" width="500">
