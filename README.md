# SIRAA – Sistema Integral de Rescate y Adopción Animal

**Universidad Técnica de Manabí (UTM)**  
**Carrera:** Tecnologías de la Información  
**Asignatura:** Desarrollo de Sistemas Informáticos  
**Unidad 1:** Desarrollo de software: Introducción y Paradigmas de Diseño  
**Estudiante:** Abrahan Isaac Velásquez Ferrín

## Descripción del proyecto

SIRAA es una propuesta de arquitectura lógica de software orientada a gestionar los procesos de rescate, atención y adopción de animales en un refugio.

El sistema permite registrar casos de rescate, clasificar animales según su especie, asignar responsables, actualizar estados, registrar tratamientos veterinarios y gestionar solicitudes de adopción cuando corresponda.

## Actores del sistema

- Ciudadano o reportante.
- Voluntario.
- Veterinario.
- Administrador del refugio.

## Requerimientos principales

- Registrar expedientes de rescate.
- Clasificar animales: perros, gatos y fauna silvestre.
- Asignar voluntarios o veterinarios responsables.
- Consultar y actualizar el estado de los rescates.
- Gestionar tratamientos y adopciones aplicables.
- Notificar automáticamente al personal correspondiente.

## Patrones de diseño

### Singleton

Se utiliza en la clase `GestorRescates` para centralizar el acceso a la gestión de expedientes mediante una instancia única.

### Observer

Se aplica mediante `ObservadorRescate` y `NotificadorRescate`, permitiendo que voluntarios y veterinarios reciban notificaciones sobre nuevos rescates.

### Factory Method

Se aplica mediante `FabricaExpedientes` y `FabricaExpedientesConcreta` para delegar la creación de expedientes según la especie del animal.

## Arquitectura lógica

El diseño propone cuatro capas:

1. Presentación.
2. Control.
3. Lógica de negocio.
4. Datos.

## Diagramas desarrollados

- Diagrama UML de casos de uso.
- Diagrama UML de clases.
- Diagrama UML de secuencia.
- Diagrama de arquitectura lógica general.

Los archivos editables y sus imágenes se encuentran en la carpeta `diagramas`.

## Control de versiones: Gitflow

El proyecto utiliza las siguientes ramas:

- `master`: versión estable del diseño.
- `develop`: integración de avances.
- `feature/documentacion-uml`: desarrollo y documentación del diseño UML.

Los cambios se registran mediante commits y se integran entre ramas siguiendo un flujo de trabajo Gitflow.

## Estado del proyecto

Proyecto académico de diseño conceptual. No corresponde todavía a una aplicación funcional implementada.