# Caso de Estudio: Plataforma de Ventas de Autoservicio (B2B)

## 概要 (Resumen del Proyecto)

Este repositorio documenta el diseño, la arquitectura y el impacto de una aplicación de escritorio desarrollada en Python (Tkinter) que funciona como un **canal de ventas de autoservicio para clientes B2B**. La herramienta fue creada desde cero para delegar estratégicamente el trabajo de presupuestar a los propios clientes, liberando a la fuerza de ventas para que se enfoque en cuentas de mayor valor.

**Actualmente, esta plataforma es responsable de generar el 14% de la facturación total de la empresa.**

---

## 🎯 El Desafío: Maximizar las Ventas con Recursos Limitados

Frente a un escenario de reducción de personal, la empresa enfrentaba un dilema estratégico: los vendedores, un recurso escaso y de alto valor, invertían un tiempo desproporcionado en la elaboración de presupuestos para clientes de menor volumen.

Los puntos críticos de dolor eran:
*   **Costo de Oportunidad:** Cada minuto dedicado a un presupuesto pequeño era un minuto que no se dedicaba a cerrar una gran cuenta.
*   **Tiempos de Respuesta Lentos:** Los clientes más pequeños sufrían demoras, afectando su experiencia y arriesgando la pérdida de esas ventas.
*   **Riesgo de Seguridad:** No existía una forma segura de compartir listas de precios sin exponer información comercial sensible (costos, márgenes, proveedores).

---

## 🛠️ Mi Solución: Una Herramienta de Delegación Estratégica

Diseñé y desarrollé una aplicación de escritorio (`.exe` autocontenido) que se distribuye a clientes seleccionados, transformándolos de receptores pasivos a participantes activos en el proceso de venta.

### Características Principales:

*   **Canal de Ventas Autónomo 24/7:** La aplicación funciona como un "vendedor virtual", permitiendo al cliente buscar productos, armar su propio pedido y recibir una confirmación sin intervención humana.
*   **Motor de Búsqueda Inteligente:** Implementé un motor de búsqueda tolerante a errores que interpreta entradas parciales y desordenadas (ej: "osch 11 olador" encuentra "Amoladora Bosch 11 1/4"), eliminando la fricción para el cliente.
*   **Gestión Segura y Ofuscada de Datos:** La aplicación descarga la lista de precios maestra pero la **ofusca localmente en la PC del cliente**, permitiéndoles trabajar con el catálogo completo sin jamás tener acceso a costos o nombres de proveedores.
*   **Control de Rentabilidad Remoto:** La herramienta se conecta a una Google Sheet controlada internamente que define el margen de ganancia, permitiendo a la gerencia ajustar la rentabilidad del canal en tiempo real.
*   **Integración Directa con el ERP:** La aplicación genera y envía por mail un archivo Excel formateado, listo para ser importado directamente en el ERP (Global Blue Point), reduciendo la carga de datos a un solo clic.

---

## 🚀 Impacto Cuantificable en el Negocio

*   **Generación del 13.6% de la Facturación Total:** La herramienta generó **$3.000.000 ARS en ventas directas** en un período de dos meses.
*   **Liberación de Recursos de Alto Valor:** Se eliminó el ciclo de 2-3 horas de trabajo manual por presupuesto, permitiendo que el equipo de ventas se enfocara 100% en cuentas estratégicas.
*   **Blindaje de la Propiedad Intelectual:** La ofuscación de datos protegió el activo más importante de la empresa: su cadena de suministro.
*   **Creación de un Activo Estratégico Escalable:** Se estableció un "vendedor virtual" que opera 24/7 sin costos de personal asociados.

---

## 💻 Stack Tecnológico

*   **Lenguaje:** Python
*   **Interfaz Gráfica (GUI):** Tkinter
*   **Manejo de Datos:** Pandas
*   **Integraciones:** Google Sheets API, Google Drive API
*   **Empaquetado:** PyInstaller
