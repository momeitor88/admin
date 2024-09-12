# Proyecto NestJS con Prisma

Este proyecto es una aplicación **NestJS** que utiliza **Prisma** como ORM para interactuar con una base de datos **PostgreSQL**. El proyecto incluye un CRUD básico de usuarios, así como autenticación mediante el registro y login de usuarios, con la opción de utilizar **JWT** para la autenticación de las solicitudes.

## Características

- CRUD de usuarios (Crear, Leer, Actualizar, Eliminar).
- Registro de usuarios.
- Autenticación con login y generación de JWT (opcional).
- Encriptación de contraseñas usando **bcrypt**.
- Validación de datos con **class-validator**.
- Gestión de la base de datos usando **Prisma**.

## Requisitos previos

- **Node.js** v14 o superior.
- **PostgreSQL** instalado y en ejecución.
- **NestJS CLI** instalado globalmente (opcional, pero recomendado).

## Instalación

1. Clona este repositorio:

   ```bash
   git clone https://github.com/tu-usuario/proyecto-nest-prisma.git
   cd proyecto-nest-prisma

2. Instala las dependencias:

   ```bash
   pnpm install

3. Crea el archivo .env en la raíz del proyecto con la URL de tu base de datos PostgreSQL: (**Reemplaza usuario, contraseña, y nombre_base_de_datos con los valores correspondientes.)

   ```bash
   DATABASE_URL="postgresql://usuario:contraseña@localhost:5432/nombre_base_de_datos?schema=public"

4. Ejecuta las migraciones de Prisma para crear la tabla de usuarios:

  ```bash
  npx prisma migrate dev --name init

5. Genera el cliente de Prisma:

  ```bash
  npx prisma generate

## Iniciar el servidor

  ```bash
  pnpm run start:dev
