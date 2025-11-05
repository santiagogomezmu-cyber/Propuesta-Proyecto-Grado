# Validación y Verificación – Gestor de Inventario

## ¿Qué es validación y verificación?

- **Validación**: ¿Estoy construyendo el producto correcto?
- **Verificación**: ¿Estoy construyendo el producto correctamente?

## Casos de Uso Identificados

---

### 1 – Registrar Producto

- **Actor**: Administrador
- **Descripción**: El usuario registra un nuevo producto con información básica.
- **Validación**: Todos los campos deben ser completados correctamente.
- **Verificación**:
  - Código único.
  - Precio y cantidad positivos.
  - Datos almacenados correctamente.

---

### 2 – Editar Producto

- **Actor**: Administrador
- **Descripción**: Actualiza la información de un producto.
- **Validación**: Solo personal autorizado puede editar.
- **Verificación**:
  - Cambios guardados correctamente.
  - Código único permanece sin duplicados.

---

### 3 – Eliminar Producto

- **Actor**: Administrador
- **Descripción**: Elimina un producto del inventario.
- **Validación**: No debe permitir eliminar productos con historial de ventas (opcional).
- **Verificación**:
  - Eliminación efectiva.
  - Sin errores en relaciones (ventas, reportes).

---

### 4 – Registrar Venta

- **Actor**: Empleado / Administrador
- **Descripción**: Registra una venta y actualiza el stock.
- **Validación**:
  - Productos existentes.
  - Stock suficiente.
- **Verificación**:
  - Stock actualizado.
  - Venta registrada correctamente.

---

### 5 – Generar Reporte de Inventario

- **Actor**: Administrador
- **Descripción**: Genera reportes de stock y movimientos.
- **Validación**: Permitir filtros básicos (fecha, producto).
- **Verificación**:
  - Datos correctos.
  - Reporte legible (PDF/Excel/HTML).

---

### 6 – Alerta de Stock Mínimo

- **Actor**: Sistema
- **Descripción**: Notifica cuando un producto llega a su stock mínimo.
- **Validación**: Definición previa de stock mínimo por producto.
- **Verificación**:
  - Alerta activa cuando se cumple la condición.
  - Notificación visible (panel, email, etc.).

