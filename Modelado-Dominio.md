# MODELADO DE DOMINIO

-**País**
<br>
Entidad que representa a cada uno de los países, donde están ubicados los departamentos que contienen las ciudades en donde están cada una de las veterinarias.
<br>
-**Departamento**
<br>
Entidad que pertenece a un país determinado, y que representa a cada uno de los departamentos donde están ubicadas las ciudades que tienen sedes pertenecientes a cada una de las veterinarias.
<br>
-**Ciudad**
<br>
Entidad que pertenece a un departamento determinado, donde están ubicadas cada uno de las veterinarias.
<br>
-**Veterinaria**
<br>
Entidad que brinda apoyo en los diferentes campos de la salud para el bienestar de una mascota.(La información más específica la tiene la sede)
<br>
-**Sede**
<br>
Entidad que representa una sucursal,la cual pertenece a una veterinaria.
<br>
-**Tipo sede**
<br>
Entidad que representa una sede,la cual pertenece a la sede de una veterinaria.
<br>
-**Consultorio**
<br>
Entidad,generalmente de carácter privado, donde un veterinario atiende a los pacientes que asisten a él para realizar una consulta.
<br>
-**Tipo Identificación**
<br>
Entidad que representa el tipo de documento que identifica a la persona.
<br>
-**Dueño**
<br>
Entidad que representa al dueño de la mascota.
<br>
-**Veterinario**
<br>
Entidad que representa al veterinario que atiende a un paciente en una determinada veterinaria.
<br>
-**Animal**
<br>
Entidad que representa a cada uno de los animales que hacen parte de una raza determinada.
<br>
-**Raza**
<br>
Entidad que pertenece a un animal y que representa cada una de las razas que tiene una mascota.
<br>
-**Mascota**
<br>
Entidad que representa el paciente que asiste a la cita,la cual pertenece a una raza.
<br>
-**Agenda**
<br>
Entidad que contiene los horarios y fechas de disponibilidad para todos los veterinarios.
<br>
-**Agenda por Veterinario**
<br>
Entidad que relaciona cada agenda con cada veterinario.
<br>
-**Estado de Agendamiento**
<br>
Entidad que indica los estados que puede tener una cita, es decir, si la cita está programada, se canceló, etc.
<br>
-**Cita**
<br>
Entidad que representa una cita dentro de la veterinaria
<br>
-**Detalle Historia Clínica**
<br>
Entidad que representa la información general de diagnóstico y mediciones.
<br>
-**Historia Clínica**
<br>
Entidad que representa la información de la mascota y última revisión, y es el cúmulo de todos los detalles.
<br>
-**Fórmula**
<br>
Entidad que representa la información más general de una fórmula médica.
<br>
-**Detalle Fórmula**
<br>
Entidad que representa los medicamentos, cantidad e indicaciones de la fórmula.
<br>
-**Notificación**
<br>
Entidad que representa una novedad de la cita.
<br>
-**Tipo Notificación**
<br>
Entidad que representa una notificación,la cual pertenece a la notificación de una cita.


[Modelos](https://app.diagrams.net/#G1biPMACpC6PVnlxnaMcAy8FE57Oh2dilD)

**Modelo de dominio** 
	<br>
	<img src="Images\Modelo-Dominio/ModeloDominio.png" alt="Modelo Dominio" width="500">

**Modelo de dominio enriquecido** 	
	<br>
	<img src="Images\Modelo-Dominio/ModeloDominioEnriquecido.png" alt="Modelo Dominio Enriquecido" width="500">
