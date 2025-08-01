# ToDoList: Sistema de Gestión de Tareas

Este es un proyecto Full-Stack desarrollado con Next.js, Prisma y TypeScript. La aplicación permite a los usuarios gestionar su propia lista de tareas.

## Características Principales

- **Gestión de Tareas:** CRUD completo para tareas.
- **Interfaz Moderna:** Interfaz de usuario reactiva y amigable construida con Next.js y Tailwind CSS.
- **Backend Robusto:** API RESTful construida con Next.js API Routes y Prisma.

## Tecnologías Utilizadas

### Frontend

- **Framework:** [Next.js](https://nextjs.org/)
- **Lenguaje:** [TypeScript](https://www.typescriptlang.org/)
- **Estilos:** [Tailwind CSS](https://tailwindcss.com/)
- **Gestión de Estado:** React Context API

### Backend

- **Entorno de Ejecución:** [Node.js](https://nodejs.org/)
- **Framework:** [Next.js API Routes](https://nextjs.org/docs/api-routes/introduction)
- **ORM:** [Prisma](https://www.prisma.io/)
- **Base de Datos:** [SQLite](https://www.sqlite.org/index.html)

## Prerrequisitos

- [Node.js](https://nodejs.org/en/) (v18 o superior)
- [npm](https://www.npmjs.com/) o [yarn](https://yarnpkg.com/)

## Instalación

1.  **Clonar el repositorio:**

    ```bash
    git clone https://github.com/EmanuelRigo/ToDoList-NextJS-prisma-TS.git
    cd ToDoList-NextJS-prisma-TS
    ```

2.  **Instalar dependencias:**

    ```bash
    npm install
    ```

3.  **Ejecutar las migraciones de Prisma:**
    ```bash
    npx prisma migrate dev
    ```

## Configuración

1.  **Variables de Entorno:**
    - Crea un archivo `.env` a partir del archivo `.env.example` (si existe) o créalo desde cero.
    - Añade las siguientes variables:
      ```env
      DATABASE_URL="file:./dev.db"
      ```

## Cómo Ejecutar la Aplicación

1.  **Iniciar la aplicación:**
    Desde el directorio raíz del proyecto:
    ```bash
    npm run dev
    ```
    La aplicación Next.js se ejecutará en `http://localhost:3000`.

Abre [http://localhost:3000](http://localhost:3000) en tu navegador para ver la aplicación en funcionamiento.

## Estructura del Proyecto

```
.
├── prisma/             # Esquema y migraciones de Prisma
│   ├── dev.db
│   └── schema.prisma
├── public/             # Archivos estáticos
├── src/                # Código fuente de la aplicación
│   ├── app/            # Páginas y rutas de la aplicación
│   │   ├── api/        # Rutas de la API
│   │   ├── new/        # Página para crear tareas
│   │   └── task/       # Páginas para editar tareas
│   ├── components/     # Componentes de React
│   └── libs/           # Clientes de base de datos y Prisma
├── package.json
└── README.md
```

- **`/prisma`**: Contiene el esquema de la base de datos y las migraciones de Prisma.
- **`/src/app`**: Contiene las páginas y rutas de la aplicación Next.js.
- **`/src/app/api`**: Contiene las rutas de la API para gestionar las tareas.
- **`/src/components`**: Contiene los componentes de React utilizados en la aplicación.
- **`/src/libs`**: Contiene la configuración del cliente de Prisma.
