# Aplicación de Control de Tareas y Metas Personales

Esta es una aplicación web diseñada para ayudarte a llevar un registro de tus tareas y metas personales. Puedes agregar nuevas tareas y metas, establecer fechas límite para su cumplimiento y eliminarlas cuando lo desees.

## Tecnologías Utilizadas

- Node.js
- Express.js

## Instrucciones de Ejecución

1. **Clonar el Repositorio**: Clona este repositorio en tu máquina local usando el siguiente comando:

git clone https://github.com/Geracu/myapp.git


2. **Instalar Dependencias**: Asegúrate de tener Node.js instalado en tu sistema. Puedes descargarlo desde [aquí](https://nodejs.org/). Luego, navega hasta el directorio del proyecto y ejecuta el siguiente comando para instalar las dependencias:

npm install


3. **Configurar la API Key**: Crea un archivo `.env` en la raíz del proyecto y agrega tu API Key de la siguiente manera:

API_KEY=tu_api_key_aqui


4. **Iniciar el Servidor**: Ejecuta el siguiente comando para iniciar el servidor:

npm start


El servidor estará en funcionamiento en http://localhost:3000.

## Endpoints Disponibles

- `GET /getTasks`: Obtiene todas las tareas.
- `GET /getGoals`: Obtiene todas las metas.
- `DELETE /removeTask`: Elimina una tarea.
- `DELETE /removeGoal`: Elimina una meta.
- `POST /addTask`: Agrega una nueva tarea.
- `POST /addGoal`: Agrega una nueva meta.

Recuerda incluir el parámetro `Authorization` en el header de tus solicitudes con tu API Key.

## Datos y Persistencia

Los datos de las tareas y metas no se almacenan en una base de datos. Se gestionan en memoria y se reinician si la aplicación se detiene.

