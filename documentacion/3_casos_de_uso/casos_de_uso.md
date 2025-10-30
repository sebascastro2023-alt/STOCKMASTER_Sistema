# Casos de Uso y Diagramas Asociados

## 1. Introducción
Este documento describe los casos de uso principales del sistema de gestión de inventarios, los actores involucrados y los diagramas asociados que permiten visualizar las interacciones entre usuarios y el sistema.

---

## 2. Actores
- **Administrador:** Usuario con permisos para gestionar materiales, proveedores y usuarios.
- **Empleado:** Usuario que realiza entradas y salidas de materiales.
- **Sistema externo:** Otros sistemas que interactúan con la base de datos (opcional).

---

## 3. Casos de Uso Principales

### Caso de Uso 1: Registrar Material
- **Actor principal:** Administrador
- **Descripción:** Permite registrar un nuevo material en el inventario.
- **Precondición:** El administrador ha iniciado sesión correctamente.
- **Postcondición:** El material queda almacenado en la base de datos.
- **Flujo principal:**
  1. Administrador selecciona "Registrar Material".
  2. Ingresa los datos del material.
  3. Sistema valida la información.
  4. Sistema guarda el material.
- **Excepciones:** Datos incompletos o duplicados.
- **Diagrama asociado:**
  ![Diagrama de caso de uso - Registrar Material](ruta/a/tu/imagen/registrar_material.png)

---

### Caso de Uso 2: Generar Reporte de Inventario
- **Actor principal:** Administrador
- **Descripción:** Permite generar un reporte de stock actual.
- **Precondición:** El usuario tiene permisos de consulta.
- **Postcondición:** El reporte se muestra en pantalla y se puede exportar.
- **Flujo principal:**
  1. Usuario selecciona "Generar Reporte".
  2. Sistema obtiene los datos de la base de datos.
  3. Sistema muestra el reporte.
- **Excepciones:** Error de conexión a la base de datos.
- **Diagrama asociado:**
  ![Diagrama de caso de uso - Generar Reporte](ruta/a/tu/imagen/reporte_inventario.png)

---

### Caso de Uso 3: Registrar Entrada/Salida de Material
- **Actor principal:** Empleado
- **Descripción:** Permite registrar movimientos de entrada o salida de materiales.
- **Precondición:** El empleado ha iniciado sesión.
- **Postcondición:** Se actualiza el inventario y el historial de movimientos.
- **Flujo principal:**
  1. Empleado selecciona "Registrar Movimiento".
  2. Ingresa el material y la cantidad.
  3. Sistema valida y guarda el movimiento.
- **Excepciones:** Cantidad excede el stock disponible.
- **Diagrama asociado:**
  ![Diagrama de caso de uso - Registrar Movimiento](ruta/a/tu/imagen/registrar_movimiento.png)

---

## 4. Diagramas de Casos de Uso
- Diagrama general mostrando todos los casos de uso y actores:  
  ![Diagrama general de casos de uso](ruta/a/tu/imagen/diagrama_general.png)

---

## 5. Notas
- Las imágenes de diagramas deben crearse previamente en alguna herramienta UML (StarUML, Lucidchart, Draw.io, etc.) y colocarse en la ruta indicada.
- Este documento se actualizará a medida que se agreguen nuevas funcionalidades.
