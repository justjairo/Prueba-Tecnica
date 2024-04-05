# Prueba Técnica para Desarrollador Full Stack

## Descripción
El objetivo de esta prueba es evaluar tus habilidades en el desarrollo de aplicaciones full stack, creando un sistema simple de gestión de usuarios con autenticación. Este sistema deberá incluir un back-end desarrollado en **JavaScript** o **TypeScript** y un front-end utilizando **React**.

### Requisitos Generales

- **Back-End**:
  - Lenguaje: JavaScript o TypeScript.
  - Base de Datos: Utilizar una base de datos postgres.
  - Autenticación: Implementar JWT para la autenticación.
  - Protección de Rutas: Todas las rutas deben estar protegidas, excepto la de login.
  - Hashing de Contraseñas: Las contraseñas de los usuarios deben ser hasheadas antes de almacenarse.

- **Front-End**:
  - Tecnología: React.
  - Funcionalidades:
    - **Página de Inicio de Sesión**: Implementar una página para que los usuarios puedan iniciar sesión.
    - **Manejo de Estado**: Utilizar Context, Redux, o Zustand para gestionar el estado de autenticación de la aplicación.
    - CRUD de usuarios.
    - Formulario para crear usuarios.
    - Tabla para mostrar usuarios, con paginación y capacidad para filtrar por roles y por coincidencia en nombre y correo.
    - Opciones para eliminar y actualizar usuarios.

### Especificaciones de la Base de Datos

#### Tablas

1. **User**
   - Nombre (string)
   - Apellido Paterno (string)
   - Apellido Materno (string)
   - Correo (string, único)
   - Número Telefónico (string)
   - Contraseña (string)
   - Fecha de Nacimiento (date)
   - Referencia a Rol (foreign key)

2. **Rol**
   - Nombre (string)
   - Descripción (string)

### Datos Iniciales

- Debes incluir un script de seed que:
  - Cree roles de forma automática.
  - Genere un usuario de prueba con permisos de administrador.

### Roles y Permisos

- Solo los usuarios con rol de administrador pueden crear nuevos usuarios.

## Entrega

- El proyecto debe ser subido a un repositorio GitHub.
- Incluir instrucciones detalladas para la instalación y ejecución de la aplicación en el archivo `README.md`.
- Asegurarse de que todas las dependencias necesarias estén claramente documentadas.

## Evaluación

Se evaluará la prueba técnica basándose en los siguientes criterios:

- Funcionalidad: La aplicación cumple con todos los requisitos funcionales.
- Código Limpio: El código es legible, bien organizado y sigue las buenas prácticas de desarrollo.
- Seguridad: Implementación adecuada de la autenticación y protección de rutas.
- Documentación: Claridad en la documentación del proyecto y facilidad de despliegue.

### ¡Éxito en tu prueba técnica!
