# CodeCash :money_with_wings:
> **Tu dinero, bajo control. Sin estrés.**

![Logo](rsc/Logo.png)

**CodeCash** es una solución integral de finanzas personales diseñada para ayudarte a entender y gestionar tu flujo de dinero de manera **eficiente**. CodeCash automatiza el seguimiento de tus **saldos** y **presupuestos** para que puedas enfocarte en tus metas financieras.

---

## :rocket: Características Principales

-   **Gestión de Cuentas:** Administra múltiples cuentas y mantén un registro preciso del saldo de cada una.
-   **Control de Transacciones:** Registra ingresos y gastos categorizados con facilidad.
-   **Presupuestos Inteligentes:** Define límites mensuales por categoría de gasto y visualiza en tiempo real cuánto has consumido y cuánto te queda disponible.
-   **Actualización Automática:** El sistema recalcula saldos y estados de presupuesto automáticamente con cada nueva transacción.
-   **Reportes Profesionales:** Genera estados de cuenta y reportes de ejecución presupuestaria en PDF.
-   **Interfaz Moderna:** OpenXava ofrece una interfaz web intuitiva, adaptable y fácil de usar.

## :computer: Stack

-   **Lenguaje:** Java 11+
-   **Framework:** [OpenXava](https://www.openxava.org/)
-   **Persistencia:** JPA / Hibernate
-   **Base de Datos:** PostgreSQL (configurable para MySQL, Oracle, etc.)
-   **Reportes:** JasperReports & JFreeChart
-   **Gestión de Dependencias:** Maven


## :file_folder: Estructura del Proyecto

```text
CodeCash/
├── rsc/
│   ├── Logo.png
│   └── diagrama.jpeg
├── src/
    ├── main/
    │   ├── java/
    │   │   └── org/example/CodeCash/
    │   │       ├── actions/
    │   │       │   ├── ReporteEstadoCuenta.java
    │   │       │   ├── SignInAction.java
    │   │       │   └── reportePresupuestoFuncion.java
    │   │       ├── model/
    │   │       │   ├── AppUsuario.java
    │   │       │   ├── BaseEntity.java
    │   │       │   ├── CategoriaGasto.java
    │   │       │   ├── CategoriaIngreso.java
    │   │       │   ├── Cuenta.java
    │   │       │   ├── Gasto.java
    │   │       │   ├── Ingreso.java
    │   │       │   └── Presupuesto.java
    │   │       └── run/
    │   │           └── CodeCash.java
    │   ├── resources/
    │   │   ├── i18n/
    │   │   ├── META-INF/
    │   │   │   └── persistence.xml
    │   │   ├── naviox.properties
    │   │   ├── naviox-users.properties
    │   │   ├── reportes/
    │   │   │   ├── ReporteEstadoCuenta.jrxml
    │   │   │   └── ReportePresupuesto.jrxml
    │   │   ├── xava.properties
    │   │   └── xava/
    │   │       ├── application.xml
    │   │       ├── controllers.xml
    │   │       └── dtds/
    │   └── webapp/
    │       ├── assets/
    │       │   └── Logo.png
    │       ├── META-INF/
    │       │   └── context.xml
    │       ├── naviox/
    │       │   └── welcome.jsp
    │       ├── WEB-INF/
    │       │   └── web.xml
    │       └── xava/
    │           ├── editors/
    │           │   ├── yourEditor.jsp
    │           │   └── js/
    │           │       └── yourEditor.js
    │           └── style/
    │               └── custom.css
    └── test/
        └── resources/
            └── xava-junit.properties
├── .gitignore
├── pom.xml
└── README.md
```

## :hammer_and_wrench: Instalación y Ejecución

### Requisitos previos
-   Java JDK 11 o superior.
-   Maven.
-   PostgreSQL (o configurar otra base de datos en `pom.xml` y `persistence.xml`).

*Nota: IntelliJ IDEA incluye soporte integrado para Maven, Java y OpenXava.*

### Pasos para ejecutar
1.  Clona el repositorio.
    ```bash
    git clone https://github.com/NextVibeCoder/CodeCash.git
    ```
2.  Configura las credenciales del datasource en `src/main/webapp/META-INF/context.xml`.
3.  Verifica la unidad de persistencia en `src/main/resources/META-INF/persistence.xml`.
4.  Compila el proyecto:
    ```bash
    mvn compile openxava:run
    ```
5.  Accede en tu navegador: `http://localhost:8080/CodeCash`

## :brain: Diseño

### Diagrama de Clases


![Diagrama](rsc/diagrama.jpeg)

python>>>>>java
