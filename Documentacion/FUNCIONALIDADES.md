# GMAO — Funcionalidades (visión pública)

Sistema: GMAO — Gestión de Mantenimiento Institucional · 2026

---

## 1. Requerimientos funcionales por módulo

### RF-01 · Autenticación y cuentas
Registro con verificación de correo, inicio de sesión con contraseña o con Google, segundo factor TOTP y recuperación de contraseña.

### RF-02 · Gestión de usuarios
Administración de cuentas, asignación de roles y control de acceso por perfil.

### RF-03 · Solicitudes de mantenimiento
Reporte de daños con descripción, ubicación y fotografías; seguimiento del estado por parte del solicitante.

### RF-04 · Órdenes de trabajo (flujo correctivo)
Clasificación de la solicitud, creación de la orden, asignación de técnico, ejecución con evidencias, aprobación del solicitante y calificación del servicio. Cada transición queda registrada en bitácora.

### RF-05 · Mantenimiento preventivo
Cronograma de rutinas por equipo con periodicidad configurable; el sistema genera automáticamente las órdenes preventivas cuando vencen.

### RF-06 · Inventario de equipos
Catálogo de equipos por áreas, categorías y tipologías, con hoja de vida e importación masiva.

### RF-07 · Insumos e inventario de materiales
Existencias de almacén, solicitudes de material desde las órdenes y despachos con descargo automático.

### RF-08 · Indicadores, informes y seguimiento
Tablero de indicadores para la dirección, informes por periodo y exportación de datos.

## 2. Atributos de calidad (requerimientos no funcionales)

| Atributo | Enfoque |
| --- | --- |
| Seguridad | Autenticación robusta, autorización por rol en el servidor y auditoría de acciones |
| Disponibilidad y operación | Despliegue en contenedores, sondas de salud y respaldos programables |
| Integridad de datos | Transacciones, validaciones en el servidor y bitácoras de cambios |
| Usabilidad | Un panel por rol, interfaz en español, flujos guiados para usuarios no técnicos |
| Rendimiento | API compilada en Rust y consultas optimizadas |
| Mantenibilidad | Código modular por dominio, migraciones versionadas y pruebas end-to-end |
