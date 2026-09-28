# Taller de Automatización con n8n — Retos 11 al 17

Repositorio correspondiente a la segunda parte del taller práctico de **automatización de procesos con n8n**, donde se desarrollan diferentes workflows orientados a facturación, validación de datos, alertas, aprobación de solicitudes, gestión de registros e informes ejecutivos.

## 👨‍💻 Autor

**Manuel Amado**

## 🛠️ Tecnologías utilizadas

- n8n
- Google Sheets
- Google Drive
- Gmail
- Webhooks
- HTTP Request
- APIs REST
- Modelos de Inteligencia Artificial
- JavaScript
- Git y GitHub

## 📂 Retos desarrollados

### Reto 11 — Procesamiento de facturas

Automatización para procesar información de una factura y registrar sus datos utilizando servicios de Google.

El workflow permite trabajar con información como:

- Número de factura
- Empresa
- NIT
- Valores de la factura
- Registro en Google Sheets
- Almacenamiento de información en Google Drive

---

### Reto 12 — Detección de duplicados

Workflow encargado de validar si un registro ya existe antes de continuar con su procesamiento.

Se implementan condiciones para diferenciar entre:

- Registros nuevos
- Registros duplicados

Esto permite evitar información repetida y mantener la integridad de los datos almacenados.

---

### Reto 13 — Alertas por vencimiento

Automatización para analizar fechas de vencimiento y generar alertas dependiendo del tiempo restante.

Se trabajan diferentes escenarios, como:

- Elementos vencidos
- Elementos próximos a vencer
- Elementos que todavía se encuentran dentro del plazo establecido

El workflow utiliza lógica condicional para determinar qué acción debe realizarse en cada caso.

---

### Reto 14 — Solicitudes mediante Webhook

Implementación de un **Webhook** para recibir información de una solicitud desde un sistema externo.

El flujo procesa datos relacionados con una compra, incluyendo:

- Solicitante
- Valor
- Información de la solicitud
- Estado inicial

La solicitud queda preparada para continuar hacia un proceso de aprobación.

---

### Reto 15 — Flujo de aprobación

Automatización conectada con el Reto 14 para gestionar la aprobación o rechazo de una solicitud.

Dependiendo de la decisión recibida, el workflow actualiza el estado correspondiente y ejecuta las acciones definidas para cada resultado.

Se manejan escenarios como:

- Solicitud aprobada
- Solicitud rechazada

---

### Reto 16 — Registro y validación de información

Workflow para recibir y procesar información estructurada de una persona o empresa.

Entre los datos procesados se encuentran:

- Nombre
- Apellido
- Correo electrónico
- Teléfono
- Empresa
- NIT
- Ciudad
- Fecha

El flujo incluye validaciones y detección de registros duplicados antes de almacenar la información.

---

### Reto 17 — Informe ejecutivo diario

Automatización que consolida información proveniente de diferentes áreas de una organización para generar un **informe ejecutivo diario**.

El workflow integra información de:

- Ventas
- Soporte
- Operaciones

Se calculan indicadores como:

- Valor total de ventas
- Negocios cerrados
- Tickets abiertos
- Tickets cerrados
- Tickets vencidos
- Procesos ejecutados
- Procesos fallidos

Los indicadores son calculados directamente por el workflow antes de utilizar Inteligencia Artificial.

Posteriormente, un modelo de IA interpreta los KPIs para generar:

- Resumen ejecutivo
- Riesgos detectados
- Temas que requieren atención

Finalmente, el informe es enviado por correo electrónico y registrado para mantener un histórico de los reportes generados.

## 🧠 Conceptos aplicados

Durante los retos se trabajan conceptos fundamentales de automatización con n8n:

- Triggers
- Webhooks
- Ejecuciones programadas
- Integración con APIs
- HTTP Request
- Condiciones con IF
- Procesamiento de datos
- Código JavaScript
- Integración entre workflows
- Google Sheets
- Google Drive
- Gmail
- Agregación de información
- Merge de múltiples fuentes
- Inteligencia Artificial aplicada a datos previamente procesados

## 📁 Estructura del repositorio

```text
Taller_n8n_Manuel_Amado_2_y_3/
│
├── Reto 11 - ...
├── Reto 12 - ...
├── Reto 13 - ...
├── Reto 14 - ...
├── Reto 15 - ...
├── Reto 16 - ...
├── Reto 17 - Informe ejecutivo diario.json
│
└── README.md
```

Los archivos `.json` contienen los workflows exportados desde **n8n** y pueden importarse nuevamente en una instancia compatible.

## 🔐 Seguridad

Las credenciales, API Keys, tokens y demás secretos utilizados durante las pruebas **no deben almacenarse directamente en el repositorio**.

Para ejecutar los workflows en otro entorno es necesario configurar las credenciales correspondientes dentro de n8n.

Ejemplos:

- Credenciales de Google
- Gmail
- Google Sheets
- Google Drive
- APIs externas
- Servicios de Inteligencia Artificial

## 🚀 Importar un workflow

1. Abrir n8n.
2. Crear un nuevo workflow.
3. Seleccionar la opción para importar desde archivo.
4. Elegir el archivo `.json` correspondiente al reto.
5. Configurar las credenciales necesarias.
6. Revisar los identificadores de documentos, hojas y recursos externos.
7. Ejecutar el workflow y realizar las pruebas correspondientes.

## 📌 Objetivo

El objetivo de estos ejercicios es aplicar conceptos de **automatización de procesos empresariales**, integrando diferentes servicios y fuentes de información mediante n8n.

Los retos avanzan desde automatizaciones basadas en validaciones y procesamiento de datos hasta workflows que consolidan información de varias áreas y utilizan Inteligencia Artificial para generar información útil para la toma de decisiones.

---

**Taller de Automatización con n8n**  
**Manuel Amado — 2026**