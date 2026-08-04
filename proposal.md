# Propuesta TP DSW

## Grupo
### Integrantes
* 51414 - Rossi, Valentina
* 52707 - Waigandt, Avril
* 52765 - Fracchia, Matias

### Repositorios
* [frontend app](https://github.com/avrilwaigandt/cafeterias-front)
* [backend app](https://github.com/avrilwaigandt/cafeterias-back)

## Tema
### Descripción
*El sistema bajo desarrollo busca abarcar todas las cuestiones referidas a la gestión de Cafeterías y la administración de las mismas. Permitiendo a los usuarios del sistema interactuar, buscar y filtrar las cafeterías. Además, permite a los propietarios subir sus cafeterías, editarlas y visualizar los comentarios recibidos, mientras los administradores pueden aprobar o rechazar cafeterías, gestionar usuarios, etc.*

### Modelo
[imagen del modelo](https://drive.google.com/file/d/1pVub1tAT_0DuA5hhEC5CTd_3GG3dD1du/view?usp=sharing)

## Alcance Funcional 

### Alcance Mínimo

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Usuario<br>2. CRUD Sucursal<br>3. CRUD Servicio|
|CRUD dependiente|1. CRUD  Cafeteria {depende de} CRUD Usuario y CRUD Sucursal<br>2. CRUD Producto {depende de} CRUD Cafeteria<br>3. CRUD Cartas {depende de} CRUD Usuarios y CRUD Cafeterias
|Listado<br>+<br>detalle| 1. Listado de cafeterías por zona y puntaje, muestra nombre y puntaje -> detalle: muestra datos completos, servicios, opiniones y su carta digital (lista de productos y precios)<br> 2. Listado de cafeterías pendientes filtrado por fecha, nombre y propietario -> detalle: muestra solicitud completa para revisión (para el administrador)|
|CUU/Epic|1. Registrar una nueva cafetería (estado inicial en pendiente)<br>2. Aprobar o rechazar solicitud de nueva|


### Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Usuario<br>2. CRUD Sucursal<br>3. CRUD Servicio<br>4. CRUD Cafetería<br>5. CRUD Producto<br>6. CRUD Reseña<br>7. CRUD Favoritos|
|CUU/Epic|1. Registrar una nueva cafetería (estado inicial en pendiente)<br>2. Aprobar o rechazar solicitud de nueva cafetería<br>3. Calificar y comentar una cafetería (opiniones/reseñas)|


### Alcance Adicional Voluntario

|Req|Detalle|
|:-|:-|
|Listados |1. Opiniones filtradas por cafetería y rango temporal, muestra historial de comentarios, puntaje y usuario|
|CUU/Epic|1. Gestión de favoritos (marcar/desmarcar cafeterías)|
|Otros|1. Envío de notificación por email al propietario cuando se aprueba o rechaza su cafetería<br>2. Manejo de archivos: subida de imagen de perfil de la cafetería o el usuario<br>3. Manejo de errores|
