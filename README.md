# 2024-leccion-03-actividad-extra
 Actividad extra para practicar lo aprendido en clase

## Configuración y Ejecución del Proyecto API

Requisitos previos:

.NET SDK: Asegúrate de tener instalado el SDK de .NET en tu sistema. Descarga la versión más reciente desde https://dotnet.microsoft.com/download

### Pasos:

#### 1. Crear la solución

```bash
dotnet new sln -o SolucionAPI
```

Esto crea una nueva solución llamada `SolucionAPI` que servirá como contenedor para tus proyectos.

#### 2. Navegar al directorio de la solución

```bash
cd SolucionAPI
```

#### 3. Crear el proyecto de la API mínima
```bash
dotnet new webapi -minimal -o MinimalAPI
```
Este comando crea un nuevo proyecto de API mínima dentro de la solución, llamado `MinimalAPI`.
#### 4. Agregar el proyecto a la solución

```bash
dotnet sln add MinimalAPI/MinimalAPI.csproj
```
Con este comando, agregas el proyecto recién creado a la solución principal.

#### 5. Ejecutar el proyecto

```bash
dotnet run --project MinimalAPI
```
Este comando inicia la aplicación desde el proyecto `MinimalAPI`.

#### 6. Subir los cambios al repositorio

Recuerda subir los cambios al repositorio para poder revisar el trabajo.

## Personalización

- **Editor de código**: Abre la solución en tu editor de código favorito (Visual Studio, Visual Studio Code, etc.) para modificar el código de la API.
- **Endpoints**: Edita el archivo `Program.cs` dentro del proyecto `MinimalAPI` para agregar nuevos endpoints y funcionalidades a tu API.

## Estructura del proyecto

```text
SolucionAPI/
├── MinimalAPI/
│   ├── MinimalAPI.csproj
│   └── Program.cs
└── SolucionAPI.sln
```

## Nota:

- **Adapta los nombres**: Puedes cambiar los nombres de la solución y del proyecto a tu gusto.
- **Añade más detalles**: Si deseas, puedes agregar más secciones al README.md, como una descripción general del proyecto, instrucciones para la configuración del entorno de desarrollo, o información sobre cómo contribuir al proyecto.

### Ejemplo de personalización con más detalles

```md
## Proyecto API de Ejemplo

Esta es una API mínima creada con ASP.NET Core. Sirve como punto de partida para desarrollar APIs RESTful.

### Requisitos previos
* **.NET SDK 7.0 o superior**

### Configuración
1. **Clonar el repositorio:**
   
   `git clone https://tu-repositorio.git`
   
2. **Restaurar las dependencias:**
   
   `cd ProyectoAPI`
   `dotnet restore`
   
```

## Preguntas frecuentes

### ¿Por qué una solución y un proyecto separados?

Separar la solución del proyecto ofrece numerosos beneficios, como:

* **Mayor organización:** Facilita la gestión de proyectos complejos.
* **Reutilización de código:** Permite compartir código entre diferentes proyectos.
* **Escalabilidad:** Adapta tu proyecto a medida que crece.
* **Mejor gestión de dependencias:** Evita conflictos y permite un control más granular.
* **Pruebas más eficientes:** Facilita la creación de pruebas aisladas.

Al crear una solución, obtienes una vista general de todos tus proyectos y sus relaciones. Por otro lado, cada proyecto se puede gestionar de forma independiente, lo que facilita el desarrollo y el mantenimiento.