# CUT-POS-Updates
Actualizaciones para [CUT] Sistema de Gestion de Punto de Ventas y Taller de Reparaciones.


# Actualización del Sistema - Version 1.2.0 Diciembre 2025

Esta actualización introduce mejoras significativas en la gestión de suplidores y el control de inventario, diseñadas para agilizar el flujo de trabajo y proporcionar una mayor visibilidad de sus operaciones.

## 🚀 Resumen de Novedades

### 1. Gestión Ágil de Suplidores
*   **Acceso Directo**: Se ha añadido un botón **"+"** al lado del campo de suplidor en el formulario de productos.
*   **Creación al Instante**: Ahora puede registrar un suplidor nuevo sin salir de la pantalla de creación de productos, eliminando interrupciones en su flujo de trabajo.

### 2. Automatización de Historial de Compras
*   **Registro Inteligente**: Cada vez que asocie un producto a un suplidor (ya sea al crear un producto nuevo o al editar uno existente), el sistema genera automáticamente una entrada en el historial de ese suplidor.
*   **Control Total**: Mantenga un registro automático de qué productos le provee cada empresa sin necesidad de entradas manuales adicionales.

### 3. Visibilidad Mejorada en Inventario
*   **Nueva Columna de Suplidor**: La tabla principal de inventario ahora incluye una columna que muestra el nombre del suplidor para cada artículo.
*   **Identificación Rápida**: Identifique de un vistazo el origen de sus productos directamente desde la lista general.

### 4. Historial de Compras Detallado
*   **Vista Expandible**: El historial de compras de los suplidores ahora es interactivo. Al hacer clic en una compra, se despliega un desglose detallado.
*   **Información Desglosada**: Visualice exactamente qué se incluyó en cada registro, incluyendo:
    *   Nombre del producto.
    *   Cantidad asociada.
    *   Precio de compra unitario.
    *   Subtotales por artículo.

### 5. Correcciones y Estabilidad
*   Se ha resuelto un problema que impedía la carga correcta de los detalles en el historial de compras en ciertas condiciones.
*   Optimización del sistema de capas visuales para permitir el uso de múltiples ventanas emergentes (modales) de forma fluida.


# Version 1.1.9
Corrección de error: "UNIQUE constraint failed: settings.key " al activar la licencia


# Version 1.1.8
Corrección de error: "Entrada incompleta" al activar la licencia



# CUT-POS and Repair Shop

![Dashboard Preview](screenshots/dashboard.PNG)

**CUT-POS and Repair Shop** es un sistema de gestión robusto diseñado para negocios que combinan la venta al detalle con un taller de servicios técnicos o reparaciones. Construido con Electron y React, ofrece una solución rápida, local y confiable para las operaciones diarias.

## 📸 Vistas del Sistema

| Punto de Venta | Gestión de Reparaciones |
| :---: | :---: |
| ![POS](screenshots/pos.PNG) | ![Repairs](screenshots/repairs.PNG) |

| Inventario | Reportes y Dashboard |
| :---: | :---: |
| ![Inventory](screenshots/inventory.PNG) | ![Reports](screenshots/reports.PNG) |


## 🚀 Características Principales

### 🛒 Punto de Venta (POS)
- **Búsqueda Rápida**: Encuentra productos por nombre, SKU o código de barras.
- **Gestión de Carrito**: Cálculos de impuestos y totales en tiempo real con estado persistente.
- **Múltiples Métodos de Pago**: Efectivo, Tarjeta, Transferencia y Crédito (Cuentas por Cobrar).
- **Generación de Facturas**: Numeración automática de facturas y cumplimiento de impresión de recibos profesionales.
- **Notificaciones de Éxito**: Confirmación visual tras cada transacción exitosa.

### 🔧 Gestión de Taller de Reparaciones
- **Seguimiento de Órdenes**: Ciclo de vida completo para reparaciones (Recibido → En Proceso → Completado → Entregado).
- **Detalles del Servicio**: Seguimiento de técnicos, información del dispositivo, fallas específicas y costos estimados vs. reales.
- **Tickets de Reparación**: Impresión de tickets de doble copia (Cliente e Interno) para nuevas órdenes.
- **Historial**: Consulta el historial completo de reparaciones de cualquier cliente.

### 📦 Inventario y Productos
- **Stock en Tiempo Real**: Deducción automática de stock en ventas e incrementos en compras.
- **Gestión de Categorías**: Organiza productos para mejores reportes.
- **Alertas de Bajo Stock**: Indicadores visuales y reportes dedicados para productos que necesitan reposición.
- **Soporte para Servicios**: Compatibilidad con ítems tipo "Servicio" que no requieren inventario físico.

### 💵 Caja y Finanzas
- **Sesiones Diarias**: Seguimiento de balance de apertura y cierre con conteo físico de denominaciones.
- **Movimientos de Efectivo**: Registro de ingresos (depósitos) y egresos (retiros) directamente a la sesión.
- **Caja Chica**: Gestión integrada de caja chica para gastos menores.
- **Resumen Financiero**: Resumen de ventas en tiempo real y cálculo de balance esperado.

### 👥 Gestión de Clientes y Suplidores
- **Perfiles de Clientes**: Almacenamiento de información de contacto, balance de deudas e historial de transacciones.
- **Seguimiento de Suplidores**: Gestión de historial de compras y pagos pendientes.

### 📊 Reportes
- **Reportes de Ventas**: Resúmenes diarios y reportes detallados por ítem.
- **Análisis Financiero**: Seguimiento de ingresos, impuestos y métodos de pago en rangos de fechas personalizados.

---

## 🛠 Tecnologías Utilizadas

- **Núcleo**: Electron (v33+)
- **Frontend**: React (v18.3) con Vite
- **Estilos**: Tailwind CSS y Lucide React
- **Gestión de Estado**: Zustand (Auth, Carrito, Tema)
- **Captura de Datos**: TanStack Query (React Query)
- **Base de Datos**: SQLite (vía `better-sqlite3`)
- **Utilidades de Backend**: BCrypt (Encriptación de contraseñas), Date-fns (Formateo de fechas)

---

## 🔐 Acceso Basado en Roles

El sistema soporta múltiples roles de usuario con diferentes permisos:
- **Admin**: Acceso total a todas las funciones, incluyendo configuración del sistema y registros.
- **Manager**: Acceso a reportes, inventario y ventas.
- **Cajero**: Acceso optimizado para operaciones de POS y caja.
- **Técnico**: Acceso enfocado en el módulo de Reparaciones.

---

## 📄 Licencia
Este proyecto está bajo la Licencia MIT.

Desarrollado con ❤️ por **Eduardo Britto**.
