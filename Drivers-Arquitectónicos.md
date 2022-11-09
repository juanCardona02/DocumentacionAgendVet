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
  - **AGENDAMIENTO**: La funcionalidad de agendamiento es crítica en el sentido que es parte esencial del core del negocio de la veterinaria.  Su indisponibilidad o lentitud al momento de solicitar una cita puede repercutir en los ingresos de la empresa.  Es por ello, desde una óptica de negocio consideramos ponerle foco técnico con el fin de brindar una mejor experiencia al usuario y que ello se vea reflejado en el crecimiento mismo de la veterinaria.

  - **ENVÍO NOTIFICACIONES**: Representa una funcionalidad crítica, porque hace parte fundamental en sentido de confiabilidad, tanto un cliente como un veterinario deben estar al tanto de los estados de las citas, en casos de cancelación / reagendamiento ambos actores deben ser notificados, de lo contrario se genera insatisfacción en torno al producto, lo que impacta diréctamente degeneración en la imágen de la empresa.

**Restricciones Técnicas**
  - Ciertas funciones están disponibles sólo para usuarios registrados.
  - Ciertas funciones están disponibles sólo para el administrador.
  - Dado el enfoque de la aplicación no se requiere de ninguna tecnología impuesta bajo ninguna clase de norma, sin embargo se usarán tecnologías según lo que consideramos más factible basados en la arquitectura que elegimos.
  
**Restricciones de Negocio**
  - *ALCANCE*: Se espera contar con una funcionalidad completa end to end, que materializa toda la arquitectura y diseño detallado.
  - *TIEMPO*: Se necesita entregar una funcionalidad al finalizar el semestre académico, equivalente a 16 semanas.
  - *COSTO*: Los recursos son subsidiados por la universidad, en caso de no estarlo serán recursos open-source.
  - *RIESGOS*: Falta de claridad, definir la funcionalidad a desarrollar, Presión de tiempo, se cuenta con menos del tiempo académico mensionado, la implementación surge sobre las 8 semanas de estudio.
  

