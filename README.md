<div align="center">
 <img width="298" height="220" alt="Logo-PetCare" src="https://github.com/user-attachments/assets/4f03ba96-8b25-4d47-ba8a-fd20cf74246c" />
</div>

![Badge en Desarollo](https://img.shields.io/badge/STATUS-EN%20DESAROLLO-green)

## Tabla de Contenido
1. [Información General.](#información-general)
2. [Colaboradores.](#colaboradores)
3. [Tecnologías.](#tecnologías)
4. [Estructuración del Proyecto.](#estructuración-del-proyecto)
5. [Flujo de Trabajo.](flujo-de-trabajo)
6. [Convención de Commits.](convención-de-commits)
7. [Git Flow.](#git-flow)
8. [Instalación.](#instalación)
***
## Información General
Este repositorio [repositorio](https://github.com/Emm3-z/PetCare.git) contiene el desarrollo del producto mínimo viable (MVP) de una aplicación móvil híbrida, la cual permite gestionar y agendar citas de diversos servicios veterinarios y a su vez, reportar mascotas perdidas o encontradas.
***
### Colaboradores
* `Oscar Eduardo Montaño López`
* `Maria José Barrera Martínez`
* `Erika Muñoz Zuñiga`
* `Johan Alexander Realpe Jimenez`
***
### Tecnologías
A continuación se encuentra una lista de las tecnologías usadas durant este proyecto:
- **Backend:** Spring Boot.
- **Frontend:** React Native + Expo.
- **Base de datos:** PostgreSQL.
***
### Estructuración del Proyecto
```
📂proyecto-PetCare/
├── 📂backend/                  # Spring Boot
│   ├── 📂src/
│   │   ├── 📂main/
│   │   │   ├── 📂java/
│   │   │   └── 📂resources/
│   │   └── 📂test/
│   ├── pom.xml              
│   ├── .gitignore
│   └── README.md
│
├── 📂frontend/                 # React
│   ├── 📂public/
│   ├── 📂src/
│   │   ├── 📂components/
│   │   ├── 📂pages/
│   │   ├── 📂services/
│   │   └── App.js
│   ├── package.json
│   ├── .gitignore
│   └── README.md
│
├── 📂database/                 # Scripts PostgreSQL
│   ├── 📂migrations/
│   │   ├── V1__create_tables.sql
│   │   └── V2__seed_data.sql
│   ├── schema.sql
│   └── README.md
│
├── 📂docs/                     # Documentación
│   ├── api-docs.md
│   ├── setup.md
│   └── architecture.md
│
├── .gitignore               # Global
└── README.md                # Documentación principal
```
***
### Flujo de Trabajo
El presente repositorio emplea un modelo de ramificación basado en Git Flow para permitir un control de versiones estructurado, evitar conflictos durante el desarrollo y facilitar el trabajo colaborativo.
- `main:` Rama de producción con versiones estables y aprobadas.
- `develop:` Rama de desarrollo donde se integran las funcionalidades.
- `feature/*:` Ramas para nuevas funcionalidades.
***
### Convención de Commits
Para el desarrollo del presente proyecto se aplicará la especificación **Conventional Commits** para asegurar un historial de cambios estructurado, en donde se encuentra el siguiente formato.
* `feat:` Para indicar una nueva funcionalidad.
* `fix:` Para corrección de errores.
* `docs:` Para inducir cambios en la documentación.
* `style:` Para cambios de formato que no involucren lógica.
* `refactor:` Para refactorizar el código.
* `test:` Para agregar o modificar pruebas.
* `chore:` Para tareas de mantenimiento (configuración, dependencias, etc.)
***
### Git Flow
El presente proyecto implementa una estrategia Git Flow, un flujo de Pull Requests (PR) para integración de código y la especificación Conventional Commits para el control de versiones. A continuación se describe un ejemplo del modelo de flujo de trabajo implementado en este repositorio:
1. Crear una rama de funcionalidad desde `develop`
```
git checkout develop
git pull origin develop
git checkout -b feature/registro-mascotas
```
2. Implementar la funcionalidad y hacer commits
```
git add .
git commit -m "feat: agregar registro de mascotas"
```
3. Subir la rama al repositorio remoto
```
git push origin feature/registro-mascotas
```
4. Crear el Pull Request
   * Ir a Pull Requests → New Pull Request.
   * Seleccionar como base `develop` y en `compare` feature/registro-mascotas.
   * Agregar descripción del PR.
   * Crear Pull Request.
5. Fusionar la rama feature/registro-mascotas en `develop`<br>
   Una vez el código haya sido revisado y aprobado por otro contribuyente, puede procederse a dar click en `Merge Pull Request`.
***
### Instalación
***

