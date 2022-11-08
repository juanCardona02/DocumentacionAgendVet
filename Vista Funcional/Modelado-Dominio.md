# MODELADO DE DOMINIO

**País**

Entidad que representa a cada uno de los países, donde están ubicados los departamentos que contienen las ciudades en donde están cada una de las sedes veterinarias.

**Departamento**

Entidad que pertenece a un país determinado, y que representa a cada uno de los departamentos donde están ubicadas las ciudades que tienen sedes pertenecientes a cada una de las sedes veterinarias.

**Ciudad**

Entidad que pertenece a un departamento determinado, donde están ubicadas cada uno de las sedes veterinarias.

**Veterinaria**

Entidad que brinda apoyo en los diferentes campos de la salud para el bienestar de una mascota.

**Sede**

Entidad que representa una sede perteneciente a una veterinaria.

**Tipo sede**

Entidad que representa el tipo una sede,la cual pertenece a la sede de una veterinaria, por ejemplo, sede principal o sede secundaria.

**Consultorio**

Entidad generalmente de carácter privado, donde un veterinario atiende a los pacientes que asisten a una consulta.

**Tipo Identificación**

Entidad que representa el tipo de documento que identifica a la persona, por ejemplo, cédula de ciudadanía.

**Dueño**

Entidad que representa al dueño de una mascota.

**Veterinario**

Entidad que representa al veterinario que atiende a un paciente en una determinada veterinaria.

**Animal**

Entidad que representa a los animales que son mascota.

**Raza**

Entidad que pertenece a un animal y que representa cada una de las razas que tiene una mascota.

**Mascota**

Entidad que representa el paciente que asiste a la cita,la cual pertenece a un dueño.

**Agenda**

Entidad que contiene los horarios y fechas de disponibilidad para todos los veterinarios.

**Novedad Agenda**

Entidad que reprsenta una novedad en los horarios y fechas de disponibilidad de la agenda que tiene un veterinario.

**Agenda por Veterinario**

Entidad que relaciona cada agenda con cada veterinario.

**Cita**

Entidad que representa una cita dentro de la veterinaria

**EStado Cita**

Entidad que representa los estados que puede tener una cita, es decir la cita está programada, se canceló o finalizó.

**Detalle Historia Clínica**

Entidad que representa la información general de la cita como diagnóstico y mediciones.

**Historia Clínica**

Entidad que alberga la información de la mascota, última revisión y el cúmulo de todos los detalles de historia clínica.

**Fórmula**

Entidad que representa la información más general de una fórmula veterinaria.

**Detalle Fórmula**

Entidad que relaciona los medicamentos, cantidad e indicaciones de la fórmula.

**Notificación**

Entidad que representa una notificación que se envía cada que hay una novedad con el estado de la cita.

**Tipo Notificación**

Entidad que representa un tipo de notificación, el cual varía según el estado de la cita.

[Modelos](https://app.diagrams.net/#G1biPMACpC6PVnlxnaMcAy8FE57Oh2dilD)
<br>
<br>
[Simulación de datos](https://docs.google.com/spreadsheets/d/1voCIOK7ZRH8KMb8mZcd0OrBhj2e0mXab/edit?usp=sharing&ouid=100818533910801106935&rtpof=true&sd=true)
<br>
<br>

**Modelo de dominio**
<br>
<img src="../Images\Modelo-Dominio/ModeloDominio.png" alt="Modelo Dominio" width="500">

**Modelo de dominio enriquecido**
<br>
<img src="../Images\Modelo-Dominio/ModeloDominioEnriquecido.png" alt="Modelo Dominio Enriquecido" width="500">
