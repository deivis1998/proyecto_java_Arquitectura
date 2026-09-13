Sistema de Facturación 

📌 Descripción

Proyecto académico desarrollado en Java para la gestión de un sistema de facturación comercial mediante una arquitectura en capas.

El sistema permite gestionar clientes, productos e inventario, crear y consultar facturas, aplicar reglas de negocio y realizar pruebas automatizadas con JUnit 5.

🏗️ Arquitectura

El proyecto está organizado en cuatro capas:

Presentación
     ↓
Aplicación
     ↓
Dominio
     ↓
Infraestructura

Presentación: interfaz de consola e interacción con el usuario.

Aplicación: coordinación de casos de uso como creación, consulta y anulación de facturas.

Dominio: entidades y reglas principales del negocio.

Infraestructura: implementación de repositorios utilizando almacenamiento en memoria.

🧾 Funcionalidades

Gestión de clientes.

Gestión de productos e inventario.

Creación de facturas.

Cálculo de subtotal, IVA y total.

Validación del estado del cliente.

Validación del stock disponible.

Actualización del inventario.

Consulta de facturas.

Consulta por cliente.

Consulta por rango de fechas.

Consulta del detalle de factura.

Anulación de facturas.

Protección de facturas anuladas.

📋 Reglas de negocio

No se puede facturar una cantidad superior al stock disponible.

No se puede facturar a un cliente inactivo.

No se puede facturar a un cliente bloqueado por mora.

Una factura anulada no puede modificarse.

Una factura anulada no puede anularse nuevamente.

El subtotal se calcula con precio por cantidad.

El IVA se calcula según el porcentaje correspondiente de cada producto.

El total corresponde al subtotal más los impuestos aplicables.

Una factura generada correctamente actualiza el inventario.

🧪 Pruebas automatizadas

El proyecto utiliza JUnit 5.

Se implementaron 8 pruebas para validar:

Cálculo de subtotal, IVA y total.

Actualización del inventario.

Stock insuficiente.

Cliente inactivo.

Cliente bloqueado por mora.

Anulación de factura.

Protección de facturas anuladas.

Consultas por cliente y fecha.

Ejecutar las pruebas:

mvn test

Resultado esperado:

Tests run: 8
Failures: 0
Errors: 0
BUILD SUCCESS

▶️ Ejecución

Requisitos

JDK 17 o superior.

Maven 3.9 o superior.

Compilar y ejecutar

mvn clean compile exec:java

Ejecutar pruebas

mvn test

📁 Estructura

ACA_Facturacion_Java/
├── pom.xml
├── README.md
├── INSTRUCCIONES_DE_TRABAJO.md
└── src/
    ├── main/java/com/aca/facturacion/
    │   ├── aplicacion/
    │   ├── dominio/
    │   ├── infraestructura/
    │   └── presentacion/
    └── test/java/com/aca/facturacion/aplicacion/
        └── ServicioFacturacionTest.java

👥 Trabajo colaborativo



DEIVIS MARTINEZ ARIAS (54452)

JUAN DAVID PUCHE CONDE (53315)

LINA MARCELA NIÑO RODRIGUEZ (53315)


