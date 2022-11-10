
**Diccionario de Datos**

**Table Name: Agenda**

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|FechaHoraInicio|||Y|Datetime|LT|
|3|FechaHoraFin|||Y|Datetime|LT||


|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: |
|Agenda\_PK|PK|Codigo|ASC|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|AgendaPorVeterinario\_Agenda\_FK|AgendaPorVeterinario|Y|Y|Agenda|Codigo|




|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | 
|AgendaPorVeterinario\_Agenda\_FK|AgendaPorVeterinario|Y|Y|Agenda|Codigo|





**Table Name:AgendaPorVeterinario**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Veterinario||F|Y|Integer|LT|
|3|Agenda||F|Y|Integer|LT|

Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: |  
|AgendaPorVeterinario\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|AgendaPorVeterinario\_Agenda\_FK|Agenda|Y|Y|Agenda|Codigo||
|AgendaPorVeterinario\_Veterinario\_FK|Veterinario|Y|Y|Veterinario|Codigo||
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|NovedadAgenda\_AgendaPorVeterinario\_FK|NovedadAgenda|Y|Y|AgendaPorVeterinario|Codigo|





**Table Name: Animal**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Nombre|||Y|VARCHAR (20) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: |
|Animal\_PK|PKCodigo|ASC|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | 
|Raza\_Animal\_FK|Raza|Y|Y|Animal|Codigo|





**Table Name: Cita**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Estado||F|Y|Integer|LT|
|3|Mascota||F|Y|Integer|LT|
|4|FechaHoraInicio|||Y|Datetime|LT|
|5|FechaHoraFin|||Y|Datetime|LT|

Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | 
|Cita\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Cita\_EstadoCita\_FK|EstadoCita|Y|Y|Estado|Codigo|
|Cita\_Mascota\_FK|Mascota|Y|Y|Mascota|Codigo|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Consultorio\_Cita\_FK|Consultorio|Y|Y|Cita|Codigo|
|DetalleHistoriaClinica\_Cita\_FK|DetalleHistoriaClinica|Y|Y|Cita|Codigo|
|Notificacion\_Cita\_FK|Notificacion|Y|Y|Cita|Codigo||





**Table Name: Ciudad**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Departamento||F|Y|Integer|LT|
|3|Nombre|||Y|VARCHAR (20) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | 
|Ciudad\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | 
|Ciudad\_Departamento\_FK|Departamento|Y|Y|Departamento|Codigo|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | 
|Dueno\_Ciudad\_FK|Dueno|Y|Y|Ciudad|Codigo|
|Sede\_Ciudad\_FK|Sede|Y|Y|Ciudad|Codigo|


**Table Name: Consultorio**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Cita||F|Y|Integer|LT|

Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: |
|Consultorio\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | 
|Consultorio\_Cita\_FK|Cita|Y|Y|Cita|Codigo|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Sede\_Consultorio\_FK|Sede|Y|Y||Consultorio|Codigo|



**Table Name: Departamento**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Pais||F|Y|Integer|LT|
|3|Nombre|||Y|VARCHAR (20) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: |
|Departamento\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Departamento\_Pais\_FK|Pais|Y|Y|Pais|Codigo|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Ciudad\_Departamento\_FK|Ciudad|Y|Y|Departamento|Codigo|





**Table Name:DetalleFormula**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Medicamento||F|Y|Integer|LT|
|3|Formula||F|Y|Integer|LT|
|4|Indicaciones|||Y|VARCHAR (800) |LT|
|5|Candidad|||Y|VARCHAR (100) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: |
|DetalleFormula\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|DetalleFormula\_Medicamento\_FK|Medicamento|Y|Y|Medicamento|Codigo|
|DetalleFormula\_Formula\_FK|Formula|Y|Y|Formula|Codigo||





**Table Name: DetalleHistoriaClinica**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Cita||F|Y|Integer|LT|
|3|Diagnostico|||Y|VARCHAR (200) |LT|
|4|Peso|||Y|VARCHAR (10) |LT|
|5|Tamano|||Y|VARCHAR (10) |LT|
|6|ObservacionesVARCHAR (100) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: |
|DetalleHistoriaClinica\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|DetalleHistoriaClinica\_Cita\_FK|Cita|Y|Y|Cita|Codigo|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | 
|Formula\_DetalleHistoriaClinica\_FK|Formula|Y|Y|DetalleHistoriaClinica|Codigo|
|HistoriaClinica\_DetalleHistoriaClinica\_FK|HistoriaClinica|Y|Y|DetalleHistoriaClinica|Codigo|





**Table Name: Dueno**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Ciudad||F|Y|Integer|LT|
|3|TipoDocumento||F|Y|Integer|LT|
|4|Veterinaria||F|Y|Integer|LT|
|5|Nombre|||Y|VARCHAR (20) |LT|
|6|Apellido|||Y|VARCHAR (20) |LT|
|7|NumeroDocumento|||Y|VARCHAR|LT|
|8|DireccionVARCHAR (30) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | 
|Dueno\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Dueno\_TipoDocumento\_FK|TipoDocumento|Y|Y|TipoDocumento|Codigo|
|Dueno\_Veterinaria\_FK|Veterinaria|Y|Y|Veterinaria|Codigo|
|Dueno\_Ciudad\_FK|Ciudad|Y|Y|Ciudad|Codigo|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Mascota\_Dueno\_FK|Mascota|Y|Y|Dueno|Codigo|





**Table Name: EstadoCita**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|DescripcionVARCHAR (10) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|EstadoCita\_PK|PKCodigo|ASC|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Cita\_EstadoCita\_FK|Cita|Y|Y|Estado|Codigo|





**Table Name: Formula**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|DetalleHistoriaClinica||F|Y|Integer|LT|
|3|DuracionTratamiento|||Y|VARCHAR (50) |LT|
|4|ObservacionesVARCHAR (100) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Formula\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Formula\_DetalleHistoriaClinica\_FK|DetalleHistoriaClinica|Y|Y|DetalleHistoriaClinica|Codigo|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | 
|DetalleFormula\_Formula\_FK|DetalleFormula|Y|Y|Formula|Codigo|





**Table Name: HistoriaClinica**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Mascota||F|Y|Integer|LT|
|3|DetalleHistoriaClinica||F|Y|Integer|LT|
|4|FechaUltimaRevision|||Y|Datetime|LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|HistoriaClinica\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|HistoriaClinica\_Mascota\_FK|Mascota|Y|Y|Mascota|Codigo|
|HistoriaClinica\_DetalleHistoriaClinica\_FK|DetalleHistoriaClinica|Y|Y|DetalleHistoriaClinica|Codigo|





**Table Name: Mascota

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Raza||F|Y|Integer|LT|
|3|Dueno||F|Y|Integer|LT|
|4|Nombre|||Y|VARCHAR (20) |LT|
|5|FechaNacimiento|||Y|Datetime|LT|
|6|SexoVARCHAR (10) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Mascota\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | 
|Mascota\_Raza\_FK|Raza|Y|Y|Raza|Codigo|
|Mascota\_Dueno\_FK|Dueno|Y|Y|Dueno|Codigo|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | 
|Cita\_Mascota\_FK|Cita|Y|Y|Mascota|Codigo|
|HistoriaClinica\_Mascota\_FK|HistoriaClinica|Y|Y|Mascota|Codigo|





**Table Name: Medicamento**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Nombre|||Y|VARCHAR (100) |LT|
|3|Concentracion|||Y|VARCHAR (50) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Medicamento\_PK|PKCodigo|ASC|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | 
|DetalleFormula\_Medicamento\_FK|DetalleFormula|Y|Y|Medicamento|Codigo|





**Table Name: Notificacion**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Cita||F|Y|Integer|LT|
|3|TipoNotificacion||F|Y|Integer|LT|
|4|Titulo|||Y|VARCHAR (30) |LT|
|5|MensajeVARCHAR (80) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Notificacion\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | 
|Notificacion\_Cita\_FK|Cita|Y|Y|Cita|Codigo|
|Notificacion\_TipoNotificacion\_FK|TipoNotificacion|Y|Y|TipoNotificacion|Codigo|





**Table Name: NovedadAgenda**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|AgendaPorVeterinario||F|Y|Integer|LT|
|3|Motivo|||Y|VARCHAR (80) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|NovedadAgenda\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | 
|NovedadAgenda\_AgendaPorVeterinario\_FK|AgendaPorVeterinario|Y|Y|AgendaPorVeterinario|Codigo|





**Table Name: Pais**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Nombre|||Y|VARCHAR (20) |LT|

Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Pais\_PK|PKCodigo|ASC|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Departamento\_Pais\_FK|Departamento|Y|Y|Pais|Codigo|





**Table Name: Raza**

Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Animal||F|Y|Integer|LT|
|3|Nombre|||Y|VARCHAR (20) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Raza\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | 
|Raza\_Animal\_FK|Animal|Y|Y|Animal|Codigo|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | 
|Mascota\_Raza\_FK|Mascota|Y|Y|Raza|Codigo|





|Table Name|Sede|
| :- | :- |
|Functional Name||
|Abbreviation||
|Classification Type Name||
|Object Type Name||
|MV Prebuilt||
|MV Query||


|Number Of Columns|6|
| :- | :- |
|Number Of Rows Min.|0|
|Number Of Rows Max.|9999999|
|Expected Number Of Rows|0|
|Expected Growth|0|
|Growth Interval|Year|
Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|TipoSede||F|Y|Integer|LT|
|3|Ciudad||F|Y|Integer|LT|
|4|Consultorio||F|Y|Integer|LT|
|5|Direccion|||Y|VARCHAR (50) |LT|
|6|Correo|||Y|VARCHAR (30) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Sede\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Sede\_TipoSede\_FK|TipoSede|Y|Y||TipoSede|Codigo||
|Sede\_Consultorio\_FK|Consultorio|Y|Y||Consultorio|Codigo||
|Sede\_Ciudad\_FK|Ciudad|Y|Y||Ciudad|Codigo||
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Veterinaria\_Sede\_FK|Veterinaria|Y|Y||Sede|Codigo||
|Veterinario\_Sede\_FK|Veterinario|Y|Y||Sede|Codigo||





|Table Name|TipoDocumento|
| :- | :- |
|Functional Name||
|Abbreviation||
|Classification Type Name||
|Object Type Name||
|MV Prebuilt||
|MV Query||


|Number Of Columns|2|
| :- | :- |
|Number Of Rows Min.|0|
|Number Of Rows Max.|9999999|
|Expected Number Of Rows|0|
|Expected Growth|0|
|Growth Interval|Year|
Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Descipcion|||Y|VARCHAR (10) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|TipoDocumento\_PK|PKCodigo|ASC|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Dueno\_TipoDocumento\_FK|Dueno|Y|Y||TipoDocumento|Codigo||
|Veterinario\_TipoDocumento\_FK|Veterinario|Y|Y||TipoDocumento|Codigo||





|Table Name|TipoNotificacion|
| :- | :- |
|Functional Name||
|Abbreviation||
|Classification Type Name||
|Object Type Name||
|MV Prebuilt||
|MV Query||


|Number Of Columns|4|
| :- | :- |
|Number Of Rows Min.|0|
|Number Of Rows Max.|9999999|
|Expected Number Of Rows|0|
|Expected Growth|0|
|Growth Interval|Year|
Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Descripcion|||Y|VARCHAR (20) |LT|
|3|Titulo|||Y|VARCHAR (20) |LT|
|4|MensajeVARCHAR (50) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|TipoNotificacion\_PK|PKCodigo|ASC|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Notificacion\_TipoNotificacion\_FK|Notificacion|Y|Y||TipoNotificacion|Codigo||





|Table Name|TipoSede|
| :- | :- |
|Functional Name||
|Abbreviation||
|Classification Type Name||
|Object Type Name||
|MV Prebuilt||
|MV Query||


|Number Of Columns|2|
| :- | :- |
|Number Of Rows Min.|0|
|Number Of Rows Max.|9999999|
|Expected Number Of Rows|0|
|Expected Growth|0|
|Growth Interval|Year|
Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|NombreVARCHAR (20) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|TipoSede\_PK|PKCodigo|ASC|
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Sede\_TipoSede\_FK|Sede|Y|Y||TipoSede|Codigo||





|Table Name|Veterinaria|
| :- | :- |
|Functional Name||
|Abbreviation||
|Classification Type Name||
|Object Type Name||
|MV Prebuilt||
|MV Query||


|Number Of Columns|5|
| :- | :- |
|Number Of Rows Min.|0|
|Number Of Rows Max.|9999999|
|Expected Number Of Rows|0|
|Expected Growth|0|
|Growth Interval|Year|
Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|Sede||F|Y|Integer|LT|
|3|NIT|||Y|VARCHAR (15) |LT|
|4|Nombre|||Y|VARCHAR (20) |LT|
|5|Correo|||Y|VARCHAR (30) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Veterinaria\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Veterinaria\_Sede\_FK|Sede|Y|Y||Sede|Codigo||
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Dueno\_Veterinaria\_FK|Dueno|Y|Y||Veterinaria|Codigo||





|Table Name|Veterinario|
| :- | :- |
|Functional Name||
|Abbreviation||
|Classification Type Name||
|Object Type Name||
|MV Prebuilt||
|MV Query||


|Number Of Columns|7|
| :- | :- |
|Number Of Rows Min.|0|
|Number Of Rows Max.|9999999|
|Expected Number Of Rows|0|
|Expected Growth|0|
|Growth Interval|Year|
Columns

|**No**|**Column Name**|**PK**|**FK**|**M**|**Data Type**|**DT <br>kind**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|Codigo|P||Y|Integer|LT|
|2|TipoDocumento||F|Y|Integer|LT|
|3|Sede||F|Y|Integer|LT|
|4|NumeroDocumento|||Y|VARCHAR|LT|
|5|Nombre|||Y|VARCHAR (20) |LT|
|6|Apeliido|||Y|VARCHAR (20) |LT|
|7|Correo|||Y|VARCHAR (30) |LT|
Indexes

|**Index Name**|**State**|**Column Name**|**Sort<br>Order**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Veterinario\_PK|PKCodigo|ASC|
Foreign Keys (referring to)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|Veterinario\_Sede\_FK|Sede|Y|Y||Sede|Codigo||
|Veterinario\_TipoDocumento\_FK|TipoDocumento|Y|Y||TipoDocumento|Codigo||
Foreign Keys (referred from)

|**Name**|**Referred From**|**Mandatory**|**Transferable**|**In Arc**|**Columns**|**Referred Columns**|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|AgendaPorVeterinario\_Veterinario\_FK|AgendaPorVeterinario|Y|Y||Veterinario|Codigo||

