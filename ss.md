#### 4. Requerimientos del módulo de Control
Caso de Uso #1:  Registro de disponibilidad de conductores
| Código | R401 | 
|----------|----------|
|Objetivo |Asignarle el traslado de un determinado pedido|
|Descripción | El usuario verifica en base a los datos del conductor como nombre completo, id conductor, número de licencia, fecha de vencimiento de licencia, fecha y hora de última actividad, para registrar su disponibilidad y poder asignarle un pedido. |
|Actor Primario | Transportista|
|Actor Secundario|N/A |
|Precondiciones|Registro de conductores en sistema|
|Paso|Acción|
|1|El usuario selecciona la opción "Transporte" y luego le da a segunda opción "Conductor"|
|2|Verifica los atributos específicos del conductor como: nombre completo, id conductor,fecha de contratación, fecha de vencimiento de licencia, fecha y hora de último traslado|
|3|Registra su disponibilidad|
|4|Verifica los datos y confirma el registro|
|5|El sistema actualiza el registro con el nuevo ingreso|

Caso de Uso #2: Registro de disponibilidad de vehículos
| Código | R402 | 
|----------|----------|
|Objetivo |Asignar a un conductor como medio de traslado del pedido|
|Descripción | El usuario verifica en base a los datos del vehículo como número de placa, modelo,año de fabricación, capacidad de carga, fecha de último mantenimiento, fecha y hora de última de actividad, para registrar su disponibilidad y poder asignarle como medio de traslado de un pedido. |
|Actor Primario | Transportista|
|Actor Secundario|N/A |
|Precondiciones|Registro de vehículos en sistema|
|Paso|Acción|
|1|El usuario selecciona la opción "Transporte" y le da a segunda opción "Vehículo"|
|2|Verifica los atributos específicos del vehículo como: número de placa, modelo,año de fabricación, capacidad de carga, fecha de último mantenimiento, fecha y hora de última de actividad |
|3|Registra su disponibilidad |
|4|Verifica los datos y confirma el registro|
|5|El sistema actualiza el registro con el nuevo ingreso|

Caso de Uso #3: Registro de nueva incidencia
| Código | R403 | 
|----------|----------|
|Objetivo |Gestionar los procesos de traslado de productos de San Fernando |
|Descripción | El usuario ingresa los datos del incidente como descripción detallada del incidente, fecha incidente, hora incidente, tipo de incidencia y el estado de atencion frente a determinada incidencia.
|Actor Primario | Encargado de almacén|
|Actor Secundario|Almacenero y Transportista|
|Precondiciones|Comunicación con cada módulo sobre incidencias en sus procesos internos|
|Paso|Acción|
|1|El usuario selecciona la opción "Incidencia"|
|2|El usuario selecciona el apartado "Nuevo"|
|2|Ingresa la información del incidente: descripción detallada del incidente,fecha incidente,hora de incidente, tipo de incidencia así como el procedimiento a realizar y la norma sobre la que se basa.|
|3|Verifica los datos y confirma el registro|
|4|El sistema actualiza el registro con el nuevo ingreso que será enviado al listado general de incidencias|

Caso de Uso #4: Registro de estado de incidencia
| Código | R404 | 
|----------|----------|
|Objetivo |Gestionar y actualizar el estado de las incidencias registradas. |
|Descripción | El usuario actualiza el estado de una incidencia previamente registrada que puede ser "Solucionada" o "Pendiente".|
|Actor Primario | Encargado de almacén|
|Actor Secundario|Almacenero y Transportista|
|Precondiciones|Existencia de incidencias previamente registradas en el sistema.|
|Paso|Acción|
|1|El usuario selecciona la opción "Incidencia"|
|2|El usurario selecciona el apartado "Registro"|
|3|Accede a un listado de incidencias registradas hasta el momento|
|4| Selecciona el estado de atención de determinada incidencia |
|5|El sistema actualiza el registro con el nuevo ingreso|


#### 4. Prototipos del Módulo de Control

|                  |                                                                                     |
| ---------------- | --------------------------------------------------------------------------------------------------- |
| Requerimientos relacionados         | R401          |
| Código      | I401 |
| Prototipo   | ![image](https://github.com/Alexclb0/Holamundo/assets/164266999/19f371dd-9641-432a-be42-277e3a5aeff5)|

|                  |                                                                                     |
| ---------------- | --------------------------------------------------------------------------------------------------- |
| Requerimientos relacionados         | R402       |
| Código      | I402 |
| Prototipo   | ![image](https://github.com/Alexclb0/Holamundo/assets/164266999/d60ac6e0-63a1-442b-a8ad-cb4c5f553f57)
|

|                  |                                                                                     |
| ---------------- | --------------------------------------------------------------------------------------------------- |
| Requerimientos relacionados         | R403       |
| Código      | I403 |
| Prototipo   | ![image](https://github.com/Alexclb0/Holamundo/assets/164266999/b3f27df0-6695-4dea-9ffd-e92b6dde286f)|

|                  |                                                                                     |
| ---------------- | --------------------------------------------------------------------------------------------------- |
| Requerimientos relacionados         | R403       |
| Código      | I404 |
| Prototipo   | ![image](https://github.com/Alexclb0/Holamundo/assets/164266999/daa1d0bb-037f-431b-85c7-b8c02fc70725)|

|                  |                                                                                     |
| ---------------- | --------------------------------------------------------------------------------------------------- |
| Requerimientos relacionados         | R403       |
| Código      | I405 |
| Prototipo   | ![image](https://github.com/Alexclb0/Holamundo/assets/164266999/9076b0dd-ac6e-4d68-a282-e7b3456107f0)|

|                  |                                                                                     |
| ---------------- | --------------------------------------------------------------------------------------------------- |
| Requerimientos relacionados         | R403       |
| Código      | I406 |
| Prototipo   | ![image](https://github.com/Alexclb0/Holamundo/assets/164266999/b96ec223-9a34-4d13-8ab2-387a5b8aa16e)|

|                  |                                                                                     |
| ---------------- | --------------------------------------------------------------------------------------------------- |
| Requerimientos relacionados         | R403, R404   |
| Código      | I407 |
| Prototipo   | ![image](https://github.com/Alexclb0/Holamundo/assets/164266999/4fe0cbda-ba9d-496b-8b3f-856d9b24307c)|



### 4. Sentencias SQL módulo de Control

### Caso 1
<table>
   <tr>
      <td>Código Requerimiento</td>
      <td>R401</td>
   </tr>
   <tr>
      <td>Código interfaz</td>
      <td>I401</td>
   </tr>
   <tr>
      <td>Imagen interfaz</td>
      <td>
         <img src="https://github.com/Alexclb0/Holamundo/assets/164266999/7e011093-b923-4e2f-bcd7-b79752030cca">
      </td>
   </tr>
   <tr>
      <td colspan="2">Sentencias SQL</td>
   </tr>
</table>

## Evento:
### Ver conductores: 
Se mostrará en pantalla la lista de todos los conductores para poder registrar su disponibilidad en base a los datos correspondiente a cada uno.
``` sql
SELECT 
    t.cod_transportista AS "Código del Conductor",
    t.cod_empleado AS "Código del Empleado",
    lt.descripcion AS "Tipo de Licencia",
    t.fecha_vencimiento_licencia AS "Fecha de Vencimiento de Licencia",
    t.fecha_ultimo_traslado AS "Fecha Último Traslado",
    t.hora_ultimo_traslado AS "Hora Último Traslado",
    te.descripcion AS "Estado del Conductor"
FROM 
    transportista t
JOIN 
    licencia_tipo lt ON t.cod_tipo_licencia = lt.cod_tipo_licencia
JOIN 
    transportista_estado te ON t.cod_estado_transportista = te.cod_estado_transportista;
```

### Caso 2
<table>
   <tr>
      <td>Código Requerimiento</td>
      <td>R401</td>
   </tr>
   <tr>
      <td>Código interfaz</td>
      <td>I401</td>
   </tr>
   <tr>
      <td>Imagen interfaz</td>
      <td>
         <img src="https://github.com/Alexclb0/Holamundo/assets/164266999/bd878778-adab-451b-bc31-8941ec9f724d">
      </td>
   </tr>
   <tr>
      <td colspan="2">Sentencias SQL</td>
   </tr>
</table>

## Evento:
### Botón Estado: 
El botón sirve para que el administrador pueda cambiar el estado de disponibilidad del conductor  que puede ser Disponible, No Disponible y Cuarentena.
``` sql
UPDATE Conductor SET cod_estado_transportista = <1> WHERE cod_estado_transportista = 2 AND cod_transportista = <2>
```

### Caso 3
<table>
   <tr>
      <td>Código Requerimiento</td>
      <td>R402</td>
   </tr>
   <tr>
      <td>Código interfaz</td>
      <td>I402</td>
   </tr>
   <tr>
      <td>Imagen interfaz</td>
      <td>
         <img src="https://github.com/Alexclb0/Holamundo/assets/164266999/60d1f8e1-606a-4945-9a68-7de18b34573a">
      </td>
   </tr>
   <tr>
      <td colspan="2">Sentencias SQL</td>
   </tr>
</table>

## Evento:
### Ver Vehículos: 
Se mostrará en pantalla la lista de todos los vehículos para poder registrar su disponibilidad en base a los datos correspondiente a cada uno.
``` sql
SELECT 
    v.cod_vehiculo AS "Código del Vehículo",
    v.año_fabricacion AS "Año de Fabricación",
    v.fecha_ultimo_mantenimiento AS "Fecha de Último Mantenimiento",
    v.capacidad_carga AS "Capacidad de Carga",
    vm.descripcion AS "Modelo",
    v.placa AS "Placa",
    pt.tipo_pedido AS "Tipo de Pedido",
    v.fecha_ultimo_viaje AS "Fecha Último Viaje",
    v.hora_ultimo_viaje AS "Hora Último Viaje",
    ve.descripcion AS "Estado del Vehículo"
FROM 
    vehiculo v
JOIN 
    vehiculo_modelo vm ON v.cod_vehiculo_modelo = vm.cod_vehiculo_modelo
JOIN 
    vehiculo_estado ve ON v.cod_vehiculo_estado = ve.cod_vehiculo_estado
JOIN 
    pedido_tipo pt ON v.cod_pedido_tipo = pt.cod_pedido_tipo;

```

### Caso 4
<table>
   <tr>
      <td>Código Requerimiento</td>
      <td>R402</td>
   </tr>
   <tr>
      <td>Código interfaz</td>
      <td>I402</td>
   </tr>
   <tr>
      <td>Imagen interfaz</td>
      <td>
         <img src="https://github.com/Alexclb0/Holamundo/assets/164266999/667ef75e-8da5-4687-8098-1134ab6a3791">
      </td>
   </tr>
   <tr>
      <td colspan="2">Sentencias SQL</td>
   </tr>
</table>

## Evento:
### Botón estado: 
El botón sirve para que el administrador pueda cambiar el estado de disponibilidad del vehículo  que puede ser Disponible, No Disponible y Cuarentena.
``` sql
UPDATE Vehículo SET cod_estado_vehiculo = <1> WHERE cod_estado_vehiculo = 2 AND cod_vehiculo = <2>

```

### Caso 5
<table>
   <tr>
      <td>Código Requerimiento</td>
      <td>R403</td>
   </tr>
   <tr>
      <td>Código interfaz</td>
      <td>I403,I404,I405,I406,I407</td>
   </tr>
   <tr>
      <td>Imagen interfaz</td>
      <td>
         <img src="https://github.com/Alexclb0/Holamundo/assets/164266999/df6a3f0e-8aa9-4057-8a2e-e6883df7b452">
         <img src="https://github.com/Alexclb0/Holamundo/assets/164266999/ba0aba03-5d69-4d5c-8bce-a7fb805b1b7d">
         <img src="https://github.com/Alexclb0/Holamundo/assets/164266999/4555d051-cfc8-4429-b148-a9baeae1fc67">
         <img src="https://github.com/Alexclb0/Holamundo/assets/164266999/53e66fca-232a-4d5f-b750-3e882732056b">
      </td>
   </tr>
   <tr>
      <td colspan="2">Sentencias SQL</td>
   </tr>
</table>

## Evento:
### Nueva incidencia: 
El administrador podrá registrar una nueva incidencia primero seleccionando el tipo de incidencia que se presenta, dependiendo de la opción del tipo de incidencia que elija le corresponderá un tipo de procedimiento específico basado en un tipo de norma respectivamente.
### Opción 1
Al elegirse esta opción, se está eligiendo un tipo de incidencia relacionado con retraso en la entrega, por ello el tipo de procedimiento también debe ser correspondiente al tipo de incidencia, es decir de tipo A; análogamente sucede con el tipo de norma en el cual se basa el procedimiento para posteriormente darle a registrar. 
``` sql
INSERT INTO incidencia VALUES (cod_incidencia, <6>, fecha_ocurrencia , hora_ocurrencia , <1>, <7> ,<12>)

```
### Opción 2
Al elegirse esta opción, se está eligiendo un tipo de incidencia relacionado con errores en el etiquetado o embalaje, por ello el tipo de procedimiento también debe ser correspondiente al tipo de incidencia, es decir de tipo B; análogamente sucede con el tipo de norma en el cual se basa el procedimiento para posteriormente darle a registrar. 
``` sql
INSERT INTO incidencia VALUES (cod_incidencia,<6>, fecha_ocurrencia , hora_ocurrencia , <2>, <8> ,<12>)

```
### Opción 3
Al elegirse esta opción, se está eligiendo un tipo de incidencia relacionado con fallas en la documentación, por ello el tipo de procedimiento también debe ser correspondiente al tipo de incidencia, es decir de tipo C; análogamente sucede con el tipo de norma en el cual se basa el procedimiento para posteriormente darle a registrar. 
``` sql
INSERT INTO incidencia VALUES (cod_incidencia,<6>, fecha_ocurrencia , hora_ocurrencia , <3>, <9> ,<13>)

```
### Opción 4
Al elegirse esta opción, se está eligiendo un tipo de incidencia relacionado con problemas mecánicos del vehículo, por ello el tipo de procedimiento también debe ser correspondiente al tipo de incidencia, es decir de tipo D; análogamente sucede con el tipo de norma en el cual se basa el procedimiento para posteriormente darle a registrar. 
``` sql
INSERT INTO incidencia VALUES (cod_incidencia,<6>, fecha_ocurrencia , hora_ocurrencia , <4>, <10> ,<14>)

```
### Opción 5
Al elegirse esta opción, se está eligiendo un tipo de incidencia relacionado con error en la asignación de la ruta, por ello el tipo de procedimiento también debe ser correspondiente al tipo de incidencia, es decir de tipo E; análogamente sucede con el tipo de norma en el cual se basa el procedimiento para posteriormente darle a registrar. 
``` sql
INSERT INTO incidencia VALUES (cod_incidencia,<6>, fecha_ocurrencia , hora_ocurrencia , <5>, <11> ,<15>)

```

### Caso 6
<table>
   <tr>
      <td>Código Requerimiento</td>
      <td>R403</td>
   </tr>
   <tr>
      <td>Código interfaz</td>
      <td>I407</td>
   </tr>
   <tr>
      <td>Imagen interfaz</td>
      <td>
         <img src="https://github.com/Alexclb0/Holamundo/assets/164266999/233260db-d6b7-44d9-867c-23bcf10d1257">
      </td>
   </tr>
   <tr>
      <td colspan="2">Sentencias SQL</td>
   </tr>
</table>

## Evento:
### Ver Incidencias: 
Se mostrará en pantalla la lista de todas las incidencias para poder registrar el grado de atención brindado en base a los datos correspondiente a cada uno.

``` sql
SELECT 
    i.cod_incidencia AS "Código de Incidencia",
    i.id_traslado AS "Código de Traslado",
    it.descripcion AS "Descripción del Tipo de Incidencia",
    i.fecha_ocurrencia AS "Fecha de Ocurrencia",
    i.hora_ocurrencia AS "Hora de Ocurrencia",
    i.cod_estado_incidencia AS "Código de Estado de Incidencia"
FROM 
    incidencia i
JOIN 
    incidencia_tipo it ON i.cod_tipo_incidencia = it.cod_tipo_incidencia;

```

### Caso 7
<table>
   <tr>
      <td>Código Requerimiento</td>
      <td>R404</td>
   </tr>
   <tr>
      <td>Código interfaz</td>
      <td>I408</td>
   </tr>
   <tr>
      <td>Imagen interfaz</td>
      <td>
         <img src="https://github.com/Alexclb0/Holamundo/assets/164266999/6c2860f5-ae9d-4816-9465-e2ef1818c52c">
      </td>
   </tr>
   <tr>
      <td colspan="2">Sentencias SQL</td>
   </tr>
</table>

## Evento:
### Botón Estado: 
El botón sirve para que el administrador pueda cambiar el estado de atención de la incidencia  que puede ser Solucionado o Pendiente. 

``` sql
El botón sirve para que el administrador pueda cambiar el estado de atención de la incidencia  que puede ser Solucionado o Pendiente. 

```

### Caso 8
<table>
   <tr>
      <td>Código Requerimiento</td>
      <td>R404</td>
   </tr>
   <tr>
      <td>Código interfaz</td>
      <td>I409</td>
   </tr>
   <tr>
      <td>Imagen interfaz</td>
      <td>
         <img src="https://github.com/Alexclb0/Holamundo/assets/164266999/02de333f-76ab-493f-a5d7-f57006eb0581">
      </td>
   </tr>
   <tr>
      <td colspan="2">Sentencias SQL</td>
   </tr>
</table>

## Evento:
### Mostrar incidencias filtradas: 
Se mostrará en pantalla el listado de incidencias filtradas por determinado periodo. 

``` sql
SELECT 
    cod_incidencia AS "Código de Incidencia",
    id_traslado AS "Código de Traslado",
    (SELECT descripcion FROM incidencia_tipo WHERE incidencia_tipo.cod_tipo_incidencia = incidencia.cod_tipo_incidencia) AS "Descripción del Tipo de Incidencia",
    fecha_ocurrencia AS "Fecha de Ocurrencia",
    hora_ocurrencia AS "Hora de Ocurrencia",
    cod_estado_incidencia AS "Código de Estado de Incidencia"
FROM 
    incidencia
WHERE 
    fecha_ocurrencia >= <1> AND fecha_ocurrencia <  <1>;

```

### 4. Funcionalidad Primaria del Módulo de Control

**Funcionalidad primaria elegida:** Registrar una nueva incidencia durante el traslado de un pedido y verificar el estado de atención de las incidencia. <br>
**Sustentación:** Registrar una nueva incidencia permite una rápida identificación y registro de problemas que ocurren durante el proceso de traslado, asegurando que sean abordados de manera oportuna. Análogamente, verificar el estado de atención de una incidencia es esencial para monitorizar el progreso de la resolución, garantizando que se tomen las acciones necesarias y se mantenga la transparencia en el proceso de gestión de incidencias.
Esta funcionalidad permitirá cumplir con los requerimientos de Registrar Nueva Incidencia (R-008), Pantalla de Incidencias (R-009), Estado de atención a Incidencia (R-010), Mostrar Incidencias filtradas (R-011) los cuales se encuentran relacionados con las interfaces I-008, I-009, I-010, I-011, I-012, I-013 y I-014.
Tendrás dos apartados, uno para registrar una nueva incidencia y otro para verificar el estado de atención de las incidencias

### Registro de nueva incidencia
<table>
   <tr>
      <th>Actividad</th>
      <th>Descripción</th>
   </tr>
   <tr>
      <td>1</td>
      <td>Al darle clic en la opción de Incidencias, hay un apartado que dice "Nuevo" que nos permitirá registrar una nueva incidencia, como se muestra en la pantalla I403. Se presentan las opciones "Tipo de incidencia", la "Descripción" de la incidencia, así como el "Tipo de Procedimiento" y "Tipo de Norma" que toman diversos valores respectivamente dependiendo la incidencia presentada. Adicionalmente, el registro de la fecha y hora en que se registra la nueva incidencia se completa automáticamente por el mismo sistema. Esto último será vital porque permitirá llevar un seguimiento cronológico de las incidencias reportadas, lo cual es fundamental para el análisis y resolución oportuna de las mismas.
	<p align="center">
           <img style="width: 80%;" src="https://github.com/Alexclb0/Holamundo/assets/164266999/0dc70229-c8f0-4a79-a489-a87abaae5689">
	</p>
      </td>
   </tr>
	
   <tr>
      <td>2</td>
      <td>Al seleccionar la opción “Tipo de Incidencia”, se muestra la pantalla I404 con cinco opciones. Debes elegir la que represente la incidencia presentada en ese momento. Estas incidencias se clasifican por tipos, que van desde la A hasta la E. Cada tipo corresponde a una categoría específica de incidencia, como retraso en la entrega, errores en el etiquetado o embalaje, fallas en la documentación, problemas mecánicos con el vehículo o error en la asignación de ruta.
          <p align="center">
             <img style="width: 80%;" src="https://github.com/Alexclb0/Holamundo/assets/164266999/b29f2e2b-b699-4dc0-8e18-5afd83c58870">
          </p> 
      </td>
   </tr>
   
   <tr>
      <td>3</td>
      <td>
	Al seleccionar la opción “Tipo de Procedimiento”, se muestra la pantalla I405 con cinco opciones. Debes elegir la que represente el tipo de procedimiento a realizar, según la incidencia que se presente en ese momento. Estos procedimientos se clasifican por tipos, que van desde la A hasta la E, de manera similar a cuando se elige el tipo de incidencia.
      <p align="center">
        <img style="width: 80%;" src="https://github.com/Alexclb0/Holamundo/assets/164266999/6830d77a-5de3-4f68-ba41-9c9646efe797">
      </p> 
      </td>
   </tr>

   <td>4</td>
      <td>
	 Al seleccionar la opción “Tipo de Norma”, se muestra la pantalla I406 con cuatro opciones. Cada una representa un tipo de norma relacionado con el procedimiento a realizar. Por ejemplo, la norma NTP 209.027 es válida para procedimientos de tipo A y B, mientras que el ISO 17712 se aplica a procedimientos de tipo C. El ISO 22000 corresponde a procedimientos de tipo D, y el ISO 9001 se utiliza para procedimientos del tipo E.
      <p align="center">
        <img style="width: 80%;" src="https://github.com/Alexclb0/Holamundo/assets/164266999/d1cfb534-90f5-4d74-be36-06ea8073f54e">
      </p> 
      </td>
   </tr>

   <td>5</td>
      <td>
	 Una vez que hayas completado cada campo en el formulario de ‘Registro de Nueva Incidencia’, haz clic en la opción ‘Registrar’. Esto añadirá una nueva incidencia al listado de ‘Registro de Incidencias’, que es una sección dentro del campo de Incidencias y forma parte de otra actividad. Sin embargo, si ocurre algún error o falta llenar algún campo en el ‘Registro de Nueva Incidencia’, puedes seleccionar la opción ‘Descartar’
      <p align="center">
        <img style="width: 80%;" src="https://github.com/Alexclb0/Holamundo/assets/164266999/85ed95c3-aad1-471e-bba4-7ae8b3b3c1c9">
      </p> 
      </td>
   </tr>
   
</table>


### Verificación de estado de atención de incidencia

<table>
   <tr>
      <th>Actividad</th>
      <th>Descripción</th>
   </tr>
   <tr>
      <td>1</td>
      <td>Al hacer clic en la opción de “Incidencias”, accedemos al apartado de “Registro”, donde se nos mostrará la pantalla I-000. En esta pantalla se presenta un listado de todas las incidencias registradas hasta el momento, con los siguientes datos: código de incidencia, código de traslado, tipo de incidencia, fecha y hora de ocurrencia, y el estado actual de la incidencia. 
Adicionalmente, hay un filtro que permite observar el número de incidencias por periodo, así como su estado de atención. Este filtro es útil para registrar los meses y años en los que se produce la mayor cantidad de incidencias. Con base en el estado, la fecha y la hora de ocurrencia, podemos priorizar la atención de determinadas incidencias, brindando así mayor seguridad y demostrando compromiso con el cliente.
	<p align="center">
           <img style="width: 80%;" src="https://github.com/Alexclb0/Holamundo/assets/164266999/3c546455-8ed7-433a-abb0-832c9bee2b56">
	</p>
      </td>
   </tr>
	
   <tr>
      <td>2</td>
      <td>Al hacer clic en la opción de “Incidencias”, accedemos al apartado de “Registro”, donde se nos mostrará la pantalla I-000. En esta pantalla se presenta un listado de todas las incidencias registradas hasta el momento, con los siguientes datos: código de incidencia, código de traslado, tipo de incidencia, fecha y hora de ocurrencia, y el estado actual de la incidencia.
Como administradores, en la pantalla I-000 podemos seleccionar el estado de atención de cada incidencia eligiendo entre las opciones “Solucionado” o “Pendiente”. De esta manera, registramos las incidencias resueltas y damos prioridad a las que faltan por abordar, evitando desconocimiento y sobreesfuerzos al intentar resolver incidencias que ya han sido cubiertas.
          <p align="center">
             <img style="width: 80%;" src="https://github.com/Alexclb0/Holamundo/assets/164266999/fbca4cc8-2e1e-4834-9618-625e25c3008d">
          </p> 
      </td>
   </tr>
   
   
</table>





