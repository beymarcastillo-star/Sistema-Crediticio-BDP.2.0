# 6. Requerimientos Funcionales

> Los requerimientos funcionales están alineados con las 12 Historias de Usuario (HU-01 a HU-12)  
> organizadas en las 6 épicas del sistema.

---

## EP01 — Seguridad y Acceso

| ID | Descripción | HU Relacionada | Prioridad |
|----|-------------|----------------|-----------|
| RF-01 | El sistema debe validar credenciales de usuario y controlar el acceso según roles (administrador, analista, comité, auditor). Bloqueo automático tras 3 intentos fallidos. Tokens JWT con expiración configurable. | HU-01 | Must |
| RF-02 | El sistema debe registrar de forma inalterable (WORM) cada acción crítica: usuario, timestamp, módulo, tipo de operación e IP. Los registros no pueden ser eliminados ni modificados. Encadenamiento SHA-256 entre registros. | HU-02 | Must |

---

## EP02 — Gestión de Solicitudes

| ID | Descripción | HU Relacionada | Prioridad |
|----|-------------|----------------|-----------|
| RF-03 | El sistema debe permitir al Jefe de Comité revisar el expediente completo (datos del solicitante, análisis técnico, scoring y garantías) y registrar una resolución formal (APROBADO / RECHAZADO) con condiciones o motivos. | HU-03 | Must |
| RF-04 | El sistema debe permitir cargar y almacenar documentos digitales (PDF, JPG, PNG, máx. 10 MB) vinculados al expediente del cliente, con previsualización desde la interfaz. | HU-04 | Must |
| RF-05 | El sistema debe mostrar un checklist dinámico de documentos obligatorios y opcionales según el tipo de crédito, bloqueando el avance si falta documentación obligatoria. | HU-05 | Must |
| RF-06 | El sistema debe permitir registrar, consultar y actualizar las garantías asociadas a cada solicitud de crédito, incluyendo tipo, valor, descripción y estado. | HU-12 | Must |

---

## EP03 — Evaluación Técnica

| ID | Descripción | HU Relacionada | Prioridad |
|----|-------------|----------------|-----------|
| RF-07 | El sistema debe calcular automáticamente proyecciones del hato ganadero (nacimientos, mortalidad, recría, engorde) a partir de parámetros ingresados, mostrando resultados en tablas y gráficos. | HU-06 | Must |
| RF-08 | El sistema debe permitir crear y comparar múltiples escenarios de simulación agrícola (variaciones de precio, rendimiento y clima) mediante un motor de reglas parametrizable sin modificar código fuente. | HU-07 | Should |

---

## EP04 — Integraciones Inteligentes

| ID | Descripción | HU Relacionada | Prioridad |
|----|-------------|----------------|-----------|
| RF-09 | El sistema debe consumir la API de la Fintech aliada para obtener el scoring crediticio del solicitante, mostrando el puntaje con clasificación de riesgo (A, B, C, D) y manejando errores de forma controlada. | HU-08 | Must |
| RF-10 | El sistema debe sincronizar automáticamente los datos de solicitudes aprobadas con el CORE bancario vía API REST, con reintentos automáticos (máximo 3) y registro de fallos. | HU-09 | Must |

---

## EP05 — Movilidad y Trabajo de Campo

| ID | Descripción | HU Relacionada | Prioridad |
|----|-------------|----------------|-----------|
| RF-11 | El sistema debe operar en modo offline mediante tecnología PWA con almacenamiento en IndexedDB, sincronizando automáticamente los datos al recuperar conectividad e indicando visualmente el modo de operación. | HU-10 | Must |

---

## EP06 — Salidas, Reportes y Monitoreo

| ID | Descripción | HU Relacionada | Prioridad |
|----|-------------|----------------|-----------|
| RF-12 | El sistema debe monitorear en tiempo real el estado de los créditos activos mediante un cron job (cada 60 segundos) que detecte vencimientos próximos y genere alertas automáticas visibles en el dashboard del oficial de crédito. | HU-11 | Must |

---

## Tabla Resumen

| ID | Épica | Descripción Corta | HU | Prioridad |
|----|-------|-------------------|----|-----------|
| RF-01 | EP01 | Control de acceso y roles con JWT | HU-01 | Must |
| RF-02 | EP01 | Auditoría WORM con SHA-256 | HU-02 | Must |
| RF-03 | EP02 | Aprobación en comité | HU-03 | Must |
| RF-04 | EP02 | Digitalización de documentos | HU-04 | Must |
| RF-05 | EP02 | Checklist de validación documental | HU-05 | Must |
| RF-06 | EP02 | Gestión de garantías | HU-12 | Must |
| RF-07 | EP03 | Proyección ganadera | HU-06 | Must |
| RF-08 | EP03 | Simulación de escenarios agrícolas | HU-07 | Should |
| RF-09 | EP04 | Scoring crediticio (API Fintech) | HU-08 | Must |
| RF-10 | EP04 | Sincronización con CORE bancario | HU-09 | Must |
| RF-11 | EP05 | Trabajo de campo sin conexión (PWA) | HU-10 | Must |
| RF-12 | EP06 | Monitoreo y alertas de vencimiento | HU-11 | Must |
