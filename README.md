# ProyectoIntegrador_BackEnd

Este proyecto fue desarrollado para el curso de Proyecto Integrador (6to. ciclo - Cibertec). Consiste en un sistema que controla la asistencia de los 
empleados y otras funcionalidades que a continuación se mencionarán:

- Gestión de los empleados
- Restricción del sistema dependiendo el rol del empleado
- Registro de actividades donde se generarán varios horarios dependiendo del día elegido
- Registro de actividades en masa (subida de actividades mediante Excel)
- Registro de feriados (si el empleado no trabaja los feriados no se generará ese día)
- Restablecimiento de contraseña que será enviada al correo del empleado
- Generación de un reporte (PDF) con todas las asistencias, tardanzas o faltas de los empleados

Se utilizaron las siguientes tecnologías: 

- Node
- React
- MySQL
- Sequelize
- TailwindCSS

# En la raíz del proyecto deberá crear un archivo .env y deberá colocar las siguientes keys:

PORT= (Elegir un puerto)

SECRET_JWT_SEED= (Deberá generar una key a su elección)

EMAIL= (Ingresar un gmail para el envío de NodeMailer)

PASSWORD= (Deberá generar una clave de aplicación para el gmail ingresado) Video de apoyo: https://www.youtube.com/watch?v=ziBy8j2TbF0

# Deberá cambiar las credenciales de la BD

En el archivo /database/db.js deberá ingresar las credenciales de su MySQL.

# Deberá crear un usuario (administrador) en Postman para empezar a crear a los demás empleados. Se deberá crear con la siguiente estructura:

{
  "nombre":"Ejemplo",
  "apellido":"Ejemplo2",
  "fec_nacimiento":"2000-01-01",
  "dni":12345678,
  "email":"ejemplo@gmail.com",
  "password":"123456",
  "tarifa_hora":16.50,
  "idArea": 1
}

# Ejecutar el proyecto

Al finalizar todos los pasos, deberá ejecutar el backend con el comando "npm run dev"
