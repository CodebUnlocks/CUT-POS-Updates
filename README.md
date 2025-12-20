# CUT-POS-Updates
Actualizaciones para [CUT] Sistema de Gestion de Punto de Ventas y Taller de Reparaciones.



# Actualización del Sistema - Version 1.2.6 20/12/2025

## 🚀 Resumen de Novedades

- **Nuevas Funcionalidades:**
  - **Vista Previa en Ventas:** Ahora puedes ver exactamente cómo saldrá impreso el recibo antes de confirmar la venta, con la opción de corregir si es necesario.
  - **Precios por Cantidad:** El sistema ahora permite definir precios especiales de mayoreo (ej: precio diferente si llevan 3 o más unidades).
  - **Creación Rápida:** Agiliza tu trabajo creando productos nuevos sin salir de la pantalla de reparaciones.

- **Impresión y Reportes:**
  - **Diseño Unificado:** Todos los documentos (facturas, tickets de reparación y reportes) ahora tienen un diseño profesional y consistente para impresoras térmicas.
  - **Vistas Previas Reales:** "Lo que ves es lo que obtienes". Las vistas previas en pantalla son idénticas al papel impreso.
  - **Generación de Reportes Mejorada:** Los reportes diarios y de cierre de caja se generan más rápido y con el formato correcto de ticket.

- **Mejoras Visuales (Interfaz):**
  - **Dashboard Interactivo:** Las tarjetas del panel principal ahora reaccionan al pasar el mouse, haciéndolas sentir más modernas.
  - **Orden Visual:** Se corrigieron alineaciones en los textos para que todo se vea más organizado y limpio.
  - **Historial a la Mano:** Nuevas opciones para ver el historial reciente directamente desde el tablero principal.

- **Correcciones y Estabilidad:**
  - **Cierre de Caja:** Se solucionó un problema que impedía guardar las notas finales al cerrar el turno.
  - **Caja Chica:** Se corrigió la clasificación automática al reponer fondos para que no se marque erróneamente como gasto de transporte.
  - **Estadísticas Precisas:** Se corrigió un error donde los números del tablero no se reiniciaban correctamente después de cerrar caja.
  - **Datos de Ejemplo:** Se actualizaron los datos de prueba para que puedas explorar mejor todas las funciones del sistema.
  - **Limpieza General:** Se eliminaron archivos viejos del sistema para mantenerlo rápido y ligero.



# Actualización del Sistema - Version 1.2.5 20/12/2025

## 🚀 Resumen de Novedades

### 🛠️ Mejoras en Reparaciones
- **Flujo de Impresión Automatizado**: Al crear una nueva orden o guardar cambios, el sistema ahora abre automáticamente la vista previa del ticket.
- **Botones Dinámicos**: Se renombraron los botones a "Crear Orden e Imprimir Ticket" para mayor claridad.
- **Ticket Doble**: Se mantiene y optimiza el formato de ticket doble (Cliente + Taller) para nuevas recepciones.

### 💰 Punto de Venta (POS) y Servicios
- **Lógica de Servicios Virtuales**: Los productos marcados como "Servicio" ahora pueden venderse sin restricciones de stock (incluso con stock 0).
- **Exclusión de Stock Bajo**: Los servicios ya no ensucian las estadísticas de "Stock Bajo" en el Dashboard ni en los filtros de Inventario.
- **Layout de Carrito**: Se optimizó el ancho del panel derecho y el tamaño de las columnas para una mejor experiencia visual.
- **Impuestos por Defecto**: La opción de impuestos ahora viene desactivada por defecto al iniciar el carrito.

### 🖥️ Interfaz de Usuario
- **Modo Aplicación Limpio**: Se eliminó la barra de menú estándar de Windows (Archivo, Editar, Ver, etc.) para ofrecer una interfaz más inmersiva y profesional.
- **Grilla de Productos**: Los resultados de búsqueda en el POS se muestran ahora en una grilla de 2 columnas para mejor lectura.

### ⚙️ Correcciones Técnicas
- **Persistencia de Descuentos**: Se arregló el problema que impedía escribir decimales en el campo de descuento.
- **Sincronización de Clientes**: Mejorada la selección y validación de clientes en tiempo real.
- **Validación de Caja**: Reforzada la lógica que impide cerrar la aplicación si la caja registradora sigue abierta.



# Actualización del Sistema - Version 1.2.4 19/12/2025

## 🚀 Resumen de Novedades

### 🔍 Busqueda Inteligente Profesional
- **Búsqueda Global Expandida**: Ahora puedes encontrar productos buscando por prácticamente cualquier campo:
    - **Nombre y Descripción** (Para búsquedas por palabras clave).
    - **Marca y Modelo** (Ideal para dispositivos electrónicos).
    - **Categoría y Suplidor** (Para filtrado rápido).
    - **Color y Capacidad** (Busca directamente "Azul" o "256GB").
    - **Serial / IMEI** (Busca una unidad específica instantáneamente).
- **Consistencia Total**: Estas mejoras aplican tanto al Punto de Venta (POS) como a la gestión de Inventario.



# Actualización del Sistema - Version 1.2.3 18/12/2025

## 🚀 Resumen de Novedades

### 📊 Rediseño de Arqueo de Caja
- **Cero Desplazamiento**: Nuevo diseño compacto que permite ver todas las denominaciones y el resumen en una sola pantalla sin necesidad de usar la barra de desplazamiento.
- **Grilla de Denominaciones**: Optimización a 5 columnas para un desglose más claro y rápido.
- **Mejor Legibilidad**: Se eliminaron los textos minúsculos, reemplazándolos por etiquetas de 10px y valores grandes y en negrita.
- **Pie de Página Inteligente**: Las notas ahora se integran horizontalmente con los botones de acción para ganar espacio vertical.

### 📱 Mejoras en Seguimiento de IMEI / Serial
- **Flexibilidad de Precios**: El campo "Precio Venta" principal ya no es obligatorio al activar el seguimiento individual, permitiendo trabajar exclusivamente con los precios de cada unidad.
- **Edición Fluida**: Se corrigió el comportamiento de los campos de costo/precio en la tabla de unidades; ahora permiten borrar valores y escribir con total libertad.
- **Corrección de Errores**: Solucionado el error "Too few parameter values" al actualizar productos con múltiples unidades.
- **Prioridad de Precios en POS**: El sistema ahora prioriza estrictamente el precio de la unidad seleccionada sobre el precio base del producto.
- **Interfaz de Selección**: El botón en el POS ahora es más intuitivo, mostrando "Seleccionar IMEI/SERIAL" con un icono representativo.



# Actualización del Sistema - Version 1.2.2 Diciembre 2025

## 🚀 Resumen de Novedades

### 1. Estabilidad y Diseño de Modales
*   **Layout Flexbox Robusto**: Se ha rediseñado la estructura interna de todos los formularios modales (`Productos`, `Clientes`, `Reparaciones`, etc.) usando Flexbox.
*   **Adiós al Desbordamiento**: Los botones de acción ya no se cortan ni se desbordan de la ventana, asegurando que siempre sean accesibles sin importar el tamaño del contenido.
*   **Corrección de Errores Críticos**: Se resolvieron fallos que causaban pantallas en blanco al intentar añadir productos o reparaciones nuevas debido a dependencias faltantes.


# Actualización del Sistema - Version 1.2.1 Diciembre 2025

## 🚀 Resumen de Novedades

### 1. Refinamiento en la Interfaz y Consistencia Visual
*   **Reubicación de Botones**: Los botones de acción ("Agregar Producto", "Nueva Reparación", etc.) se han movido a la sección de filtros. Esto despeja el encabezado y agrupa las acciones de búsqueda y creación en un solo lugar.
*   **Estandarización de Tamaños**: Todos los botones de acción ahora tienen un tamaño uniforme (`h-10`) que coincide con los campos de entrada, creando una línea visual limpia.
*   **Mejoras en Configuración**: Los botones de "Guardar Cambios" en la pantalla de configuración ahora se encuentran alineados a la derecha, siguiendo los estándares modernos de diseño de formularios.
*   **Consistencia en Punto de Venta**: Los botones de apertura y cierre de caja han sido estandarizados para coincidir con el resto de la interfaz, mejorando la coherencia visual en todo el sistema.
*   **Encabezados Informativos**: Se han restaurado y mejorado los encabezados de las páginas, incluyendo iconos descriptivos y contadores de elementos para una navegación más intuitiva.

---


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
