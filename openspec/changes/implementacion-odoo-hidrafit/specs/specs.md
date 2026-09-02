# ADDED Requirements

## Requirement: CRM - Gestión de Clientes

El sistema SHALL proporcionar una base de datos centralizada de clientes con historial completo de servicios.

### Scenario: Base de datos centralizada de clientes
- **DADO QUE** HYDRAFIT tiene clientes registrados en correos y documentos dispersos
- **CUANDO** se registra un nuevo cliente en el CRM
- **ENTONCES** se crea un registro centralizado con todos los datos del cliente

### Scenario: Historial completo de servicios
- **DADO QUE** un cliente tiene servicios previos registrados
- **CUANDO** se consulta el historial del cliente
- **ENTONCES** se muestra el registro completo de todos los servicios prestados

### Scenario: Múltiples contactos por cliente
- **DADO QUE** un cliente tiene múltiples personas de contacto
- **CUANDO** se registra un contacto adicional
- **ENTONCES** se asocian múltiples contactos con roles diferenciados al mismo cliente

### Scenario: Seguimiento de oportunidades
- **DADO QUE** hay una oportunidad comercial potencial
- **CUANDO** se registra y da seguimiento a la oportunidad
- **ENTONCES** se puede rastrear su estado desde la captación hasta el cierre

---

## Requirement: Ventas - Gestión Comercial

El sistema SHALL gestionar cotizaciones formales y órdenes de venta de manera trazable.

### Scenario: Cotizaciones formales
- **DADO QUE** un cliente solicita un servicio
- **CUANDO** se genera una cotización
- **ENTONCES** se crea una cotización formal y profesional con formato estándar

### Scenario: Órdenes de venta trazables
- **DADO QUE** una cotización es aprobada
- **CUANDO** se convierte a orden de venta
- **ENTONTHEN** se genera una orden de venta vinculada a la cotización original

### Scenario: Seguimiento automático de propuestas
- **DADO QUE** se envía una propuesta al cliente
- **CUANDO** pasa el tiempo de seguimiento
- **ENTONCES** el sistema notifica el estado de la propuesta

---

## Requirement: Inventario - Control de Stock

El sistema SHALL controlar en tiempo real el stock de repuestos y materiales.

### Scenario: Control en tiempo real de stock
- **DADO QUE** se registra un movimiento de inventario
- **CUANDO** se actualiza el stock
- **ENTONCES** el inventario se actualiza en tiempo real

### Scenario: Alertas automáticas de stock bajo
- **DADO QUE** un producto está por debajo del stock mínimo
- **CUANDO** se consulta el inventario
- **ENTONCES** se muestra una alerta automática del producto

### Scenario: Historial de uso de materiales
- **DADO QUE** un servicio utiliza materiales
- **CUANDO** se completa el servicio
- **ENTONCES** se registra el historial de materiales utilizados

### Scenario: Costo automático de materiales
- **DADO QUE** un servicio utiliza materiales del inventario
- **CUANDO** se factura el servicio
- **ENTONCES** el costo de materiales se incluye automáticamente en la factura

---

## Requirement: Proyecto - Órdenes de Trabajo

El sistema SHALL gestionar órdenes de trabajo con asignación a técnicos y registro de tiempos.

### Scenario: Crear orden de trabajo
- **DADO QUE** un cliente solicita un servicio
- **CUANDO** se crea una orden de trabajo
- **ENTONCES** se asigna un técnico responsable a la orden

### Scenario: Registro de tareas y tiempos
- **DADO QUE** un técnico trabaja en una orden
- **CUANDO** registra sus tareas y tiempos
- **ENTONCES** se almacena el historial de trabajo realizado

### Scenario: Historial centralizado del servicio
- **DADO QUE** un servicio pasa por varias etapas
- **CUANDO** se consulta el historial
- **ENTONCES** se muestra diagnóstico, cotización y trabajo realizado en un solo lugar

---

## Requirement: Servicio Externo - Comunicación Integrada

El sistema SHALL centralizar todas las comunicaciones relacionadas con los servicios.

### Scenario: Chatter unificado
- **DADO QUE** hay comunicaciones sobre un servicio
- **CUANDO** se accede a la orden de trabajo
- **ENTONCES** todas las comunicaciones aparecen en un solo lugar (Chatter)

### Scenario: Subir fotos y documentos
- **DADO QUE** un técnico toma fotos o escanea documentos en campo
- **CUANDO** los sube al sistema
- **ENTONCES** se adjuntan al registro del servicio

### Scenario: Notas de llamadas y actividades
- **DADO QUE** se realiza una llamada o actividad con el cliente
- **CUANDO** se registra la nota
- **ENTONCES** se almacena en el historial del servicio

---

## Requirement: Compras - Gestión de Proveedores

El sistema SHALL gestionar órdenes de compra y control de materiales de proveedores.

### Scenario: Órdenes de compra automáticas
- **DADO QUE** un producto está por debajo del stock mínimo
- **CUANDO** se verifica el inventario
- **ENTONCES** se genera automáticamente una orden de compra al proveedor

### Scenario: Recepción y control de materiales
- **DADO QUE** se recibe material de un proveedor
- **CUANDO** se registra la recepción
- **ENTONTHEN** se actualiza el inventario automáticamente

### Scenario: Gestión de cuentas por pagar
- **DADO QUE** se recibe una factura de proveedor
- **CUANDO** se registra en el sistema
- **ENTONCES** se gestiona en las cuentas por pagar

---

## Requirement: Contabilidad - Gestión Financiera

El sistema SHALL centralizar la gestión financiera con reportes automáticos.

### Scenario: Libro de ventas automático
- **DADO QUE** se facturan servicios a clientes
- **CUANDO** se genera una factura
- **ENTONCES** se registra automáticamente en el libro de ventas

### Scenario: Libro de compras automático
- **DADO QUE** se reciben facturas de proveedores
- **CUANDO** se registra una compra
- **ENTONCES** se registra automáticamente en el libro de compras

### Scenario: Cuentas por cobrar y pagar
- **DADO QUE** hay facturas pendientes de cobro o pago
- **CUANDO** se consulta la contabilidad
- **ENTONCES** se muestran las cuentas por cobrar y pagar centralizadas

### Scenario: Estados financieros automáticos
- **DADO QUE** hay transacciones registradas
- **CUANDO** se genera un estado financiero
- **ENTONCES** se produce un reporte actualizado automáticamente

### Scenario: Reportes de rentabilidad por servicio
- **DADO QUE** se prestan diferentes tipos de servicios
- **CUANDO** se genera un reporte de rentabilidad
- **ENTONTHEN** se muestra la rentabilidad desglosada por tipo de servicio

### Scenario: Integración con contador externo
- **DADO QUE** HYDRAFIT tiene un contador externo
- **CUANDO** se configura el acceso
- **ENTONCES** el contador puede acceder a la información contable
