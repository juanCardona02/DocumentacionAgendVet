# Diagrama de Compomentes

Permite identificar las dependencias lógicas y los artefactos que se van a usar para la implementación del agendamiento de citas para la veterinaria.

Este diagrama indica que el lenguaje de desarrollo será Java, con el uso del framework Spring.

En dicho diagrama, existen seis componentes lógicos, de cuales:

	-El adaptador depende del servicio y de los Objeto de transferencia de datos.
	-El servicio depende del dominio, de la infraestructura y de la entidad.
	-La infraestructura depende del servicio.

Todas las solicitudes generadas a la aplicación entrarán por el adaptador, el cual se encarga de informarle al servicio la solcitud y esta va a infraestructura para darle respuesta.

**Diagrama de Compomentes**

<br>
<img src="/Images/Diagrama-Componentes/DiagramaComponentes.png" alt="Diagrama de Compomentes" width="500">
