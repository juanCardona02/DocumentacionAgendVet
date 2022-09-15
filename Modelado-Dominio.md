# MODELADO DE DOMINIO

-<b>País</b>: Entidad que representa a cada uno de los países, donde están ubicados los departamentos que contienen las ciudades en donde están cada una de las veterinarias.
<br>
- <b>Departamento <b>:Entidad que pertenece a un país determinado, y que representa a cada uno de los departamentos donde están ubicadas las ciudades que tienen sedes pertenecientes a cada una de las veterinarias.
<br>
-*Ciudad*:Entidad que pertenece a un departamento determinado, donde están ubicadas cada uno de las veterinarias.
<br>
-<b>*Veterinaria*</b>: Entidad que brinda apoyo en los diferentes campos de la salud para el bienestar de una mascota.(La información más específica la tiene la sede)
<br>
-*Sede*: Entidad que representa una sucursal,la cual pertenece a una veterinaria.
<br>
-*Tipo sede*:Entidad que representa una sede,la cual pertenece a la sede de una institución.
<br>
-*Consultorio*:Entidad,generalmente de carácter privado, donde un veterinario atiende a los pacientes que asisten a él para realizar una consulta.
<br>
-*Tipo Identificación*:Entidad que representa el tipo de documento que identifica a la persona.
<br>
-*Dueño*:Entidad que representa al dueño de la mascota.
<br>
-*Veterinario*:Entidad que representa al veterinario que atiende a un paciente en una determinada veterinaria.
<br>
-*Animal*: Entidad que representa a cada uno de los animales que hacen parte de una raza determinada.
<br>
-*Raza*: Entidad que pertenece a un animal y que representa cada una de las razas que tiene una mascota.
<br>
-*Mascota*:Entidad que representa el paciente que asiste a la cita, el cual pertenece a una raza.
<br>
-*Agenda*: Entidad que contiene los horarios y fechas de disponibilidad para todos los veterinarios.
<br>
-*Agenda por veterinario*:Entidad que relaciona cada agenda con cada veterinario.
<br>
-*Estado de agendamiento*: Entidad que indica los estados que puede tener una cita, es decir, si la cita está programada, se canceló, etc.
<br>
-*Cita*:Entidad que representa una cita dentro de la veterinaria
<br>
-*Detalle de historia*:Entidad que representa la información general de diagnóstico y mediciones.
<br>
-*Historia clínica*:Entidad que representa la información de la mascota y última revisión, y es el cúmulo de todos los detalles.
<br>
-*Fórmula*:Entidad que representa la información más general de una fórmula médica.
<br>
-*Detalle fórmula*: Entidad que representa los medicamentos, cantidad e indicaciones de la fórmula.
<br>
-*Notificación:* Entidad que representa una novedad de la cita.
<br>
-*Tipo Notificación*: Entidad que representa una notificación,la cual pertenece a la notificación de una cita.


[Modelos](https://app.diagrams.net/#G1biPMACpC6PVnlxnaMcAy8FE57Oh2dilD)

**Modelo de dominio** 
	<br>
	<img src="Images\Modelo-Dominio/ModeloDominio.png" alt="Modelo Dominio" width="500">

**Modelo de dominio enriquecido** 	
	<br>
	<img src="Images\Modelo-Dominio/ModeloDominioEnriquecido.png" alt="Modelo Dominio Enriquecido" width="500">
