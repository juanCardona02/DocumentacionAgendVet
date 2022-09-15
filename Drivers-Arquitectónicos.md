# DRIVERS ARQUITECTÓNICOS

[Atributos de Calidad](https://docs.google.com/spreadsheets/d/1S_FjFUqPp5lyossS7RIULytX8pctjinT/edit?usp=sharing&ouid=100818533910801106935&rtpof=true&sd=true)

<p><b>Atributos de calidad</b></p>
  - Priorización de atributos
		<br>
        Gráfico Radar
        <br>
		<img src="Images/Mapa-Empatia/PriorizaciónAtributos.png" alt="Gráfico Radar" width="500">
  
  - Características y escenarios de calidad
	- Confiabilidad
			<br>
			1.Características
			<br>
			![esc](Images/Atributos-Calidad/Confiabilidad/CaracterisiticasConfiabilidad.png)<br>
			2.Escenarios<br>
				2.1. Escenario de Calidad 1
				![esc](Images/Atributos-Calidad/Confiabilidad/EsBaConfiabilidad1.png)
				2.2. Escenario de calidad 2
				![esc](Images/Atributos-Calidad/Confiabilidad/EsBaConfiabilidad2.png)
				2.3. Escenario de Calidad 3
				![esc](Images/Atributos-Calidad/Confiabilidad/EsBaConfiabilidad3.png)
				2.4. Escenario de calidad 4
				![esc](Images/Atributos-Calidad/Confiabilidad/EsBaConfiabilidad4.png)
				2.5. Escenario de Calidad 5
				![esc](Images/Atributos-Calidad/Confiabilidad/EsBaConfiabilidad5.png)
	- Disponibilidad
			<br>
			1.Características
			<br>
			![esc](Images/Atributos-Calidad/Disponibilidad/CaracterisiticasDisponibilidad.png)<br>
			2.Escenarios<br>
				2.1. Escenario de Calidad 1
					![esc](Images/Atributos-Calidad/Disponibilidad/EsBaDisponibilidad1.png)
				2.2. Escenario de calidad 2
					![esc](Images/Atributos-Calidad/Disponibilidad/EsBaDisponibilidad2.png)
				2.3. Escenario de Calidad 3
					![esc](Images/Atributos-Calidad/Disponibilidad/EsBaDisponibilidad3.png)
				2.4. Escenario de calidad 4
					![esc](Images/Atributos-Calidad/Disponibilidad/EsBaDisponibilidad4.png)
	- Rendimiento
			<br>
			1.Características
			<br>
			![esc](Images/Atributos-Calidad/Rendimiento/CaractersiticasRendimiento.png)<br>
			2.Escenarios<br>
				2.1. Escenario de Calidad 1
					![esc](Images/Atributos-Calidad/Rendimiento/EsBaRendimiento1.png)
				2.2. Escenario de calidad 2
					![esc](Images/Atributos-Calidad/Rendimiento/EsBaRendimiento2.png)
				2.3. Escenario de Calidad 3
					![esc](Images/Atributos-Calidad/Rendimiento/EsBaRendimiento3.png)
				2.4. Escenario de calidad 4
					![esc](Images/Atributos-Calidad/Rendimiento/EsBaRendimiento4.png)
	- Experiencia de Usuario
			<br>
			1.Características
			<br>
			![esc](Images/Atributos-Calidad/Ux/CaracterisitcasUx.png)
			<br>
			2.Escenarios<br>
				2.1. Escenario de Calidad 1
					![esc](Images/Atributos-Calidad/Ux/EsBaUx1.png)
				2.2. Escenario de calidad 2
					![esc](Images/Atributos-Calidad/Ux/EsBaUx2.png)
				2.3. Escenario de Calidad 3
					![esc](Images/Atributos-Calidad/Ux/EsBaUx3.png)
				2.4. Escenario de calidad 4
					![esc](Images/Atributos-Calidad/Ux/EsBaUx4.png)		
	- Seguridad
			<br>
			1.Características
			<br>
			![esc](Images/Atributos-Calidad/Seguridad/CaracterisitcasSeguridad.png)
			<br>
			2.Escenarios<br>
				2.1. Escenario de Calidad 1
					![esc](Images/Atributos-Calidad/Seguridad/EsBaSeguridad1.png)
				2.2. Escenario de calidad 2
					![esc](Images/Atributos-Calidad/Seguridad/EsBaSeguridad2.png)
				2.3. Escenario de Calidad 3
					![esc](Images/Atributos-Calidad/Seguridad/EsBaSeguridad3.png)
				2.4. Escenario de calidad 4
					![esc](Images/Atributos-Calidad/Seguridad/EsBaSeguridad4.png)	
				2.5. Escenario de calidad 5
					![esc](Images/Atributos-Calidad/Seguridad/EsBaSeguridad5.png)		
				2.6. Escenario de calidad 6
					![esc](Images/Atributos-Calidad/Seguridad/EsBaSeguridad6.png)

**Funcionalidades Críticas** 
  - **AGENDAMIENTO**:La funcionalidad de agendamiento es crítica en el sentido que es parte esencial del core del negocio de la veterinaria.  Su indisponibilidad o lentitud al momento de solicitar una cita puede repercutir en los ingresos de la empresa.  Es por ello, desde una óptica de negocio consideramos ponerle foco técnico con el fin de brindar una mejor experiencia al usuario y que ello se vea reflejado en el crecimiento mismo de la veterinaria.
  - **ENVÍO NOTIFICACIONES**:Representa una funcionalidad crítica, porque hace parte fundamental en sentido de confiabilidad, tanto un cliente como un veterinario deben estar al tanto de los estados de las citas, en casos de cancelación / reagendamiento ambos actores deben ser notificados, de lo contrario se genera insatisfacción en torno al producto, lo que impacta diréctamente degeneración en la imágen de la empresa.

**Restricciones Técnicas**
  - Funcionales:
  
	Funciones como administrar sedes y/o veterinarios sólo estarán disponibles para el rol de administrador
	Sólo el rol de administrador puede bloquear / eliminar otros usuarios.
		
	- El administrador puede:

		- Registrar veterinarias
		- Registrar sedes
		- Registrar / modificar / eliminar / consultar tipos de sedes
		- Registrar / modificar / eliminar / consultar consultorios
		- Bloquear / eliminar usuarios en el sistema
		- Registrar / modificar / eliminar / consultar equipamiento por sede
		
	- Un veterinario puede:
	
		- Registrar, modificar o eliminar medicamentos
		- Consultar medicamentos	
		- Consultar dueños	
		- Recetar fórmulas
		- Crear / seleccionar agendas
		- Actualizar datos de sí mismo (veterinario)
		- Modificar / eliminar citas
		- Consultar / modificar / eliminar razas
		- Eliminar veterinario (sí mismo)
		
	- Un dueño puede:
	
		- Registrar / modificar / eliminar una cuenta de usuario
		- Consultar agendas
		- Registrar / modificar / eliminar citas
		- Consultar citas
		- Consultar historias clínicas
		- Consultar fórmulas	
		- Registrar / modificar / eliminar / consultar mascotas
		- Registrar / consultar razas


**Restricciones de Negocio**

- El detalle de historia clínica y toda la información que contiene(fórmula, paciente, veterinario que atendió...) se cierra solo cuando se da como finalizada la cita.
- Una vez cerrada una cita no se puede modificar información de la historia clínica referente a dicha cita.
- Una cita debe agendarse en un espacio disponible con antelación de al menos tres  horas.
- Los horarios disponibles deben ser previa y claramente definidos por la veterinaria / sede.
- Los tipos de mascotas al ser atendidos deben ser previamente definidos.
- Un veterinario puede cancelar únicamente una cita agendada a sí mismo.
- No pueden existir citas simultáneas para el mismo usuario.
- Un veterinario no puede tener citas agendadas para diferentes usuarios / sedes en simultáneo.
- Un consultorio no puede tener más de una cita en simultáneo.
