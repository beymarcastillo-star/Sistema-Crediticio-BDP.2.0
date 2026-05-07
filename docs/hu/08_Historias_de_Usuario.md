# 8. Historias de Usuario

> Numeración unificada según documento maestro HUs_Completas_v2 (Roger Huarachi).  
> Total: 12 HUs organizadas en 6 épicas funcionales.

---

## EP01 — Seguridad y Acceso

| ID | Actor | Historia de Usuario | Prioridad | Pareja |
|----|-------|---------------------|-----------|--------|
| HU-01 | Usuario del Sistema | Como usuario del sistema, quiero contar con un mecanismo de autenticación seguro basado en roles, para acceder únicamente a las funcionalidades autorizadas según mi perfil institucional. | Must | P1 Roger + Kevin |
| HU-02 | Auditor Institucional | Como auditor, quiero que el sistema registre de forma inalterable cada acción crítica ejecutada por los usuarios, para garantizar el cumplimiento normativo y la transparencia operacional. | Must | P2 Beymar + Abigail |

---

## EP02 — Gestión de Solicitudes

| ID | Actor | Historia de Usuario | Prioridad | Pareja |
|----|-------|---------------------|-----------|--------|
| HU-03 | Jefe de Comité de Crédito | Como Jefe de Comité, quiero revisar el expediente completo de una solicitud y emitir una resolución formal de aprobación o rechazo, para formalizar la decisión institucional de manera trazable y auditable. | Must | P3 Alcozer + Miguel |
| HU-04 | Analista de Crédito | Como analista, quiero cargar y almacenar documentos digitales del expediente para eliminar el uso de papel y centralizar la información documental de cada solicitud. | Must | P1 Roger + Kevin |
| HU-05 | Analista de Crédito | Como analista, quiero contar con un checklist inteligente de requisitos documentales para verificar que el expediente esté completo antes de avanzar a la siguiente etapa del proceso crediticio. | Must | P2 Beymar + Abigail |
| HU-12 | Oficial de Crédito / Analista Financiero | Como oficial de crédito, quiero registrar y gestionar las garantías asociadas a cada solicitud de crédito, para respaldar formalmente el riesgo crediticio asumido por el banco. | Must | P3 Alcozer + Miguel |

---

## EP03 — Evaluación Técnica

| ID | Actor | Historia de Usuario | Prioridad | Pareja |
|----|-------|---------------------|-----------|--------|
| HU-06 | Analista Agropecuario | Como analista agropecuario, quiero proyectar el ciclo de vida del hato ganadero del solicitante para determinar su capacidad de pago basada en indicadores productivos reales. | Must | P3 Alcozer + Miguel |
| HU-07 | Analista Agrícola | Como analista agrícola, quiero simular distintos escenarios productivos (variaciones de precios, rendimiento o clima) mediante la funcionalidad de supuestos, para evaluar la resiliencia financiera del proyecto bajo condiciones adversas. | Should | P1 Roger + Kevin |

---

## EP04 — Integraciones Inteligentes

| ID | Actor | Historia de Usuario | Prioridad | Pareja |
|----|-------|---------------------|-----------|--------|
| HU-08 | Sistema / Analista de Crédito | Como sistema, quiero conectarme a la API de la Fintech aliada para obtener automáticamente el scoring crediticio del solicitante y enriquecer el expediente con información externa de riesgo. | Must | P2 Beymar + Abigail |
| HU-09 | Sistema | Como sistema, quiero sincronizar datos relevantes de las solicitudes aprobadas con el CORE bancario institucional vía API REST, para garantizar la coherencia de la información entre ambas plataformas. | Must | P3 Alcozer + Miguel |

---

## EP05 — Movilidad y Trabajo de Campo

| ID | Actor | Historia de Usuario | Prioridad | Pareja |
|----|-------|---------------------|-----------|--------|
| HU-10 | Analista de Campo | Como analista de campo, quiero registrar datos e información del solicitante desde zonas rurales sin conectividad a internet, para sincronizarlos automáticamente con el servidor central al recuperar la señal. | Must | P1 Roger + Kevin |

---

## EP06 — Salidas, Reportes y Monitoreo

| ID | Actor | Historia de Usuario | Prioridad | Pareja |
|----|-------|---------------------|-----------|--------|
| HU-11 | Oficial de Crédito / Jefe de Cartera | Como Oficial de Crédito, quiero monitorear en tiempo real el estado de los créditos activos de mi cartera y recibir alertas automáticas ante vencimientos próximos o incumplimientos, para tomar acciones preventivas oportunas y reducir la mora. | Must | P2 Beymar + Abigail |

---

## Tabla Resumen

| ID | Épica | Nombre | Actor | Prioridad | Pareja |
|----|-------|--------|-------|-----------|--------|
| HU-01 | EP01 – Seguridad y Acceso | Control de Acceso y Roles | Usuario del Sistema | Must | P1 Roger + Kevin |
| HU-02 | EP01 – Seguridad y Acceso | Trazabilidad y Auditoría | Auditor Institucional | Must | P2 Beymar + Abigail |
| HU-03 | EP02 – Gestión de Solicitudes | Aprobar / Rechazar en Comité | Jefe de Comité | Must | P3 Alcozer + Miguel |
| HU-04 | EP02 – Gestión de Solicitudes | Digitalización de Documentos | Analista de Crédito | Must | P1 Roger + Kevin |
| HU-05 | EP02 – Gestión de Solicitudes | Validación Documental | Analista de Crédito | Must | P2 Beymar + Abigail |
| HU-06 | EP03 – Evaluación Técnica | Proyección Ganadera | Analista Agropecuario | Must | P3 Alcozer + Miguel |
| HU-07 | EP03 – Evaluación Técnica | Simulación de Escenarios Agrícolas | Analista Agrícola | Should | P1 Roger + Kevin |
| HU-08 | EP04 – Integraciones Inteligentes | Scoring Crediticio (API Fintech) | Sistema / Analista | Must | P2 Beymar + Abigail |
| HU-09 | EP04 – Integraciones Inteligentes | Sincronización con CORE Bancario | Sistema | Must | P3 Alcozer + Miguel |
| HU-10 | EP05 – Movilidad y Campo | Trabajo de Campo sin Conexión | Analista de Campo | Must | P1 Roger + Kevin |
| HU-11 | EP06 – Reportes y Monitoreo | Monitoreo de Créditos y Alertas | Oficial de Crédito | Must | P2 Beymar + Abigail |
| HU-12 | EP02 – Gestión de Solicitudes | Registro y Gestión de Garantías | Oficial de Crédito | Must | P3 Alcozer + Miguel |
