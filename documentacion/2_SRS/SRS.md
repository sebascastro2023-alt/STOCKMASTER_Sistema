# Especificación de Requerimientos de Software (SRS)

## 1. Introducción

### 1.1 Propósito
El propósito de este documento es especificar los requerimientos funcionales y no funcionales del sistema integral de gestión de inventarios, asegurando que todos los participantes comprendan el alcance y las funciones del sistema.

### 1.2 Alcance del sistema
El sistema permitirá:
- Gestionar inventarios de materiales y productos
- Registrar entradas y salidas de inventario
- Controlar proveedores
- Generar reportes y métricas
- Integrar con base de datos relacional

### 1.3 Definiciones, acrónimos y abreviaturas
- **SRS**: Software Requirements Specification  
- **DB**: Base de datos  
- **UI**: Interfaz de usuario  

---

## 2. Requerimientos generales

### 2.1 Requerimientos funcionales
1. Registrar materiales y productos en el inventario.  
2. Registrar entradas y salidas de inventario.  
3. Gestionar proveedores.  
4. Generar reportes por período y por tipo de material.  
5. Buscar y filtrar información del inventario.  

### 2.2 Requerimientos no funcionales
- Rendimiento: el sistema debe procesar consultas de inventario en menos de 3 segundos.  
- Seguridad: solo usuarios autenticados pueden acceder al sistema.  
- Compatibilidad: compatible con navegadores modernos.  
- Escalabilidad: debe soportar al menos 5000 registros de inventario sin degradación.  

### 2.3 Restricciones
- El sistema será desarrollado en tecnologías web (HTML, CSS, JavaScript) y base de datos relacional (MySQL/PostgreSQL).  
- El proyecto debe completarse antes del 30 de diciembre de 2025.  

---

## 3. Priorización de requerimientos
| Requerimiento | Prioridad | Responsable |
|---------------|-----------|------------|
| Registrar materiales | Alta | Sebastián Ariza Castro |
| Gestionar proveedores | Media | Julián Ramírez Rodríguez |
| Generar reportes | Alta | Sebastián Ariza Castro |
| Consultas rápidas | Alta | Sebastián Ariza Castro y Julián Ramírez Rodríguez |
