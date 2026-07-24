# Caso: GymManager
## Contexto

GymManager es un sistema destinado a gimnasios pequeños y medianos que permite administrar socios, entrenadores, rutinas y asistencias.

Actualmente el gimnasio utiliza planillas de Excel y cuadernos para registrar toda la información, lo que provoca pérdidas de datos, errores en los pagos y dificultad para realizar el seguimiento de los clientes.

El propietario desea digitalizar la gestión del gimnasio mediante una aplicación de escritorio desarrollada en Java.

### Objetivos

El sistema deberá permitir administrar:

- socios
- entrenadores
- rutinas
- membresías
- pagos
- asistencia
## Requerimientos iniciales
### Gestión de socios

El sistema debe permitir registrar nuevos socios indicando:

- nombre
- apellido
- documento
- fecha de nacimiento
- teléfono
- correo electrónico

No puede existir dos socios con el mismo documento.

Un socio puede estar:

- Activo
- Suspendido
- Inactivo
### Gestión de entrenadores

El gimnasio posee entrenadores.

De cada entrenador interesa conocer:

- nombre
- apellido
- especialidad
- correo
- teléfono

Un entrenador puede tener varios socios asignados.

Cada socio posee un entrenador principal.

### Rutinas

Cada rutina tiene:

- nombre
- descripción
- nivel
- duración estimada

Una rutina está compuesta por varios ejercicios.

Cada ejercicio posee:

- nombre
- series
- repeticiones
- peso recomendado

Un mismo ejercicio puede pertenecer a muchas rutinas.

### Membresías

El gimnasio ofrece distintos planes.

Por ejemplo:

- Mensual
- Trimestral
- Semestral
- Anual

Cada membresía posee:

- nombre
- precio
- duración en días

Un socio solo puede tener una membresía activa.

### Pagos

Cuando un socio paga su membresía se registra:

- fecha
- importe
- método de pago

Puede ser:

- efectivo
- débito
- crédito
- transferencia
- Asistencia

Cada vez que un socio ingresa al gimnasio se registra:

- fecha
- hora

El sistema debe permitir consultar:

- cantidad de asistencias del mes
- último ingreso
- historial
- Consultas

El propietario desea poder consultar:

- socios activos
- socios con pagos vencidos
- entrenadores y sus socios
- rutinas disponibles
- ingresos del mes
- cantidad de asistencias
### Restricciones
- No se puede eliminar un socio con pagos registrados.
- No se puede registrar un pago para un socio inactivo.
- No puede haber documentos repetidos.
- Una membresía vencida cambia automáticamente el estado del socio a suspendido.
- Las rutinas solo pueden asignarse a socios activos.