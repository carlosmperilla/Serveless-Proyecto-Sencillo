# CRUD Serverless Users

Este proyecto utiliza el Serverless Framework para implementar un servicio CRUD (Crear, Leer, Actualizar, Eliminar) para usuarios en AWS utilizando DynamoDB como base de datos.

## Configuración

Antes de implementar el servicio, asegúrate de tener las siguientes herramientas instaladas:

- [Node.js](https://nodejs.org/) (versión 14.x o superior)
- [Serverless Framework](https://www.serverless.com/)

Luego, clona este repositorio y ejecuta `npm install` para instalar las dependencias del proyecto.

## Variables de entorno

Este proyecto utiliza variables de entorno para configurar algunos aspectos del servicio. Asegúrate de crear un archivo `.env` en el directorio raíz del proyecto con las siguientes variables:

- `ID_CUENTA`: El ID de tu cuenta de AWS.

## Implementación

Para implementar el servicio en AWS, ejecuta el siguiente comando:

```bash
sls deploy
```

Este comando empaquetará e implementará el servicio en tu cuenta de AWS.

## Uso

Una vez que el servicio esté implementado, puedes utilizarlo para realizar operaciones CRUD en usuarios. Las siguientes funciones están disponibles:

- `get-users`: Obtiene información sobre un usuario específico.
- `create-users`: Crea un nuevo usuario.
- `update-users`: Actualiza la información de un usuario existente.
- `delete-users`: Elimina un usuario existente.

Puedes invocar estas funciones utilizando la API HTTP expuesta por Amazon API Gateway. Consulta la salida del comando `sls deploy` para obtener la URL de la API.

## Desinstalación

Para eliminar el servicio de tu cuenta de AWS, ejecuta el siguiente comando:

```bash
sls remove
```

Este comando eliminará todos los recursos creados por el servicio en tu cuenta de AWS.
