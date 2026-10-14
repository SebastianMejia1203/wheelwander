# WheelWander

Sistema web de alquiler de motocicletas desarrollado con ASP.NET Core MVC. Reúne la consulta del catálogo, las reservas y la administración de la flota en una aplicación con vistas Razor.

## Funcionalidades

- Catálogo de motocicletas y gestión de reservas.
- Registro, inicio de sesión y administración de usuarios.
- Gestión de motocicletas y consulta de información del negocio.
- Exportación a Excel y generación de documentos PDF.
- Servicios de correo electrónico y carga de imágenes mediante ImgBB.

## Tecnologías

C#, .NET 8, ASP.NET Core MVC, SQL Server, Razor, Bootstrap y jQuery. El proyecto incluye bibliotecas de acceso a SQL Server, ClosedXML, QuestPDF, iText y MailKit.

## Inicio local

1. Instala el SDK de .NET 8 y prepara una instancia de SQL Server.
2. Revisa la conexión en `ProyectoWheelWander/Datos/ConexionDB.cs` y configura una base de datos compatible con las consultas del proyecto.
3. Configura los servicios de correo e imágenes en tu entorno local antes de utilizar esas funciones.
4. Restaura y ejecuta la aplicación:

```bash
dotnet restore ProyectoWheelWander.sln
dotnet run --project ProyectoWheelWander/ProyectoWheelWander.csproj
```

Utiliza la URL que indique la consola. La puesta en marcha requiere preparar la base de datos; este repositorio no incluye un script SQL de inicialización.

## Estructura

| Ruta | Contenido |
| --- | --- |
| `ProyectoWheelWander/Controllers/` | Controladores MVC |
| `ProyectoWheelWander/Datos/` | Consultas y conexión a SQL Server |
| `ProyectoWheelWander/Models/` | Modelos y datos para las vistas |
| `ProyectoWheelWander/Views/` | Vistas Razor |
| `ProyectoWheelWander/Services/` | Servicios de correo y carga de imágenes |
| `ProyectoWheelWander/wwwroot/` | Recursos estáticos |

## Compilación

```bash
dotnet build ProyectoWheelWander.sln
```

