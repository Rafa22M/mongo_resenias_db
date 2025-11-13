# mongo_resenias_db
Proyecto: Base de Datos NoSQL para Plataforma de Reseñas de películas y series

Este proyecto implementa una base de datos NoSQL en MongoDB para una plataforma de reseñas de películas y series.
Permite gestionar usuarios, títulos y reseñas, donde cada usuario puede valorar y comentar diferentes películas o series.

Estructura del Proyecto

mongo_resenias_db/
├── README.md                → Descripción general del proyecto
├── database.js              → Creación de la base de datos y colecciones
├── consultas_basicas.js     → Consultas básicas (insertar, actualizar, eliminar, buscar)
├── consultas_agregacion.js  → Consultas de agregación (promedio, suma, conteo, etc.)

Estructura de la Base de Datos

Base de datos: `resenias_db`
Colecciones:
`usuario` → Guarda la información de los usuarios registrados.
 `titulo` → Contiene los títulos de películas o series.
 `resenia` → Registra las reseñas y puntuaciones de los usuarios sobre los títulos.

Ejecución

1. Abre el MongoDB Shell o tu entorno de consola conectado a Atlas.
2. Copia y ejecuta el contenido de `database.js` para crear la base de datos y las colecciones.
3. Ejecuta las inserciones.
4. Prueba las consultas básicas desde `consultas_basicas.js`.
5. Ejecuta las consultas de agregación con `consultas_agregacion.js`.

 Consultas Implementadas

Consultas Básicas:
Insertar nuevos documentos.
Actualizar información existente.
Eliminar documentos.
Consultar registros específicos.

Consultas de Agregación:
Calcular promedio de calificaciones.
Contar cantidad de reseñas por título.
Sumar puntuaciones totales.

Análisis General

MongoDB fue elegido porque permite manejar información variable (usuarios, reseñas y títulos) sin estructuras fijas.
Esto facilita el crecimiento del sistema a medida que aumenta la cantidad de usuarios y reseñas, y evita las restricciones de los modelos relacionales tradicionales.
