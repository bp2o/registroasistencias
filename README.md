# Sistema de Gestión de Asistencias

⚠️Este repositorio es solo un prototipo para una evaluación

Aplicación hecha con Java (MVC), y con base de datos MySQL para gestionar horarios y asistencias de funcionarios.
POR EL MOMENTO ESTA EN DESARROLLO AUN!!

## Estructura del proyecto
src/
└── 📦 app
├── 📂 controllers
│   ├── LoginController.java
│   └── RegisterController.java
├── 📂 dao
│   ├── FuncionarioDAO.java
│   ├── HorarioDAO.java
│   └── JustificationDAO.java
├── 📂 models
│   ├── Funcionario.java
│   ├── HorarioProgramado.java
│   └── Justification.java
├── 📂 utils
│   ├── DBConnection.java
│   ├── PasswordUtils.java
│   └── UITheme.java
├── 📂 views
│   ├── AdminDashboardView.java
│   ├── AdminHorariosView.java
│   ├── AdminJustificacionesView.java
│   ├── FuncionarioCrearJustificationView.java
│   ├── FuncionarioDashboardView.java
│   ├── FuncionarioHorariosView.java
│   ├── FuncionarioVerJustificacion.java
│   ├── HorarioFormView.java
│   ├── LoginView.java
│   └── RegisterView.java
└── Main.java


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
1. Descargar el archivo registroasistencias 0.1.6.zip

2. Extraer el archivo e ingresarlo al archivo local de su IDE

## En caso de no se conecte base de datos

- Crea la base de datos con el archivo de texto "nose" del repositorio y pegalo en MySQL

- Añade el driver de mysql connector al programa

- Puedes entrar en los archivos locales, para editar los datos de tu servidor
  
```bash
C:\...\RegistroAsistencia\src\utils\DBConnection.java

         y en esta parte del código puede editarlo

   // === EDITAR ESTOS DATOS SEGÚN EL SERVIDOR ======= //

    private static final String URL = "jdbc:mysql://localhost:33065/empresa_asistencia2"; // Editar tu url
    private static final String USER = "root"; // Editar tu user
    private static final String PASS = ""; // Editar tu contraseña

    // ================================================ //
