Propósito del Proyecto:
Este proyecto consiste en una aplicación web que administra tareas. La aplicación tiene dos partes principales:

Backend: Usando Spring Boot para crear una API REST que maneja las tareas.
Frontend: Usando React para crear una interfaz de usuario que interactúa con la API.

Arquitectura Hexagonal: La Arquitectura Hexagonal (también conocida como Arquitectura de Puertos y Adaptadores) permite que el sistema sea más flexible y fácil de mantener. En este caso:

	Capa de Dominio: Representa las entidades centrales del sistema, como la clase Task.

	Capa de Aplicación: Contiene la lógica de negocio, representada por el servicio TaskService, que ofrece las operaciones relacionadas con las tareas.

	Adaptadores (Puertos): Los adaptadores permiten la interacción con el sistema desde el exterior. En el caso del backend, el adaptador es un controlador REST (TaskController) que expone los servicios del backend a través de endpoints HTTP.

	Código Limpio y Refactorización: El código está organizado de manera que sigue los principios de Código Limpio:

Las clases tienen una única responsabilidad:
•	Las funciones son pequeñas y claras.
•	La estructura del proyecto es modular, lo que facilita la refactorización y el mantenimiento.
