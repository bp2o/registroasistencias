# Sistema de Gestión de Asistencias

Aplicación hecha con Java (MVC), y con base de datos MySQL para gestionar horarios y asistencias de funcionarios.

## Estructura del proyecto
📦 src
└── 📁 app
　　├── 🎮 controllers
　　│　 ├── LoginController.java
　　│　 └── RegisterController.java
　　│
　　├── 🗃️ dao
　　│　 ├── AdminDAO.java
　　│　 ├── FuncionarioDAO.java
　　│　 ├── HorarioDAO.java
　　│　 └── JustificacionDAO.java
　　│
　　├── 🧠 models
　　│　 ├── Administrador.java
　　│　 ├── Funcionario.java
　　│　 ├── HorarioProgramado.java
　　│　 └── Justificacion.java
　　│
　　├── ⚙️ utils
　　│　 ├── DBConnection.java
　　│　 ├── PasswordUtils.java
　　│　 └── UITheme.java
　　│
　　├── 🪟 views
　　│　 ├── AdminDashboardView.java
　　│　 ├── AdminHorariosView.java
　　│　 ├── AdminJustificacionesView.java
　　│　 ├── FuncionarioCrearJustificacionView.java
　　│　 ├── FuncionarioDashboardView.java
　　│　 ├── FuncionarioHorariosView.java
　　│　 ├── HorarioFormView.java
　　│　 ├── LoginView.java
　　│　 └── RegisterView.java
　　│
　　└── 🚀 Main.java

## Funcionalidades principales
- Inicio de sesión para Administradores y Funcionarios
- Registro y visualización de horarios de entrada/salida
- revisión de justificaciones
- Arquitectura Modelo - Vista - Controlador (MVC)
- Conexión MySQL con JDBC

## Tecnologías utilizadas
- IntelliJ IDEA
- Eclipse IDE
- XAMPP
- MySQL 8
- Swing (interfaz gráfica)

## Cómo ejecutar
1. Descargar el archivo registroasistencias.zip

2. Extraer el archivo y entrar en el archivo java "App"

## En caso de no se conecte base de datos
- Puedes entrar en los archivos locales, para editar los datos de tu servidor
```bash
C:\...\RegistroAsistencia\src\utils\DBConnection.java

         y en esta parte del código puede editarlo

   // === EDITAR ESTOS DATOS SEGÚN EL SERVIDOR ======= //

    private static final String URL = "jdbc:mysql://localhost:33065/empresa_asistencia2"; // Editar tu url
    private static final String USER = "root"; // Editar tu user
    private static final String PASS = ""; // Editar tu contraseña

    private static Connection connection = null;

    // ================================================ //
