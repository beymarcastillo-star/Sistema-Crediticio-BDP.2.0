# Plataforma Virtual para la Digitalización del Proceso Crediticio Pyme y Banca Empresa

## 1. Resumen Ejecutivo

### 1.1 Ficha del Proyecto

| **Concepto** | **Descripción** |
|--------|-------------|
| **Nombre del Proyecto** | CONSULTORÍA PARA LA PROVISIÓN DE SOFTWARE PARA PYME Y BE |
| **Problema a Resolver** | El Banco de Desarrollo Productivo (BDP S.A.M.) presenta un proceso crediticio para Pyme y Banca Empresa que requiere mayor agilidad, eficiencia y digitalización. Actualmente, el proceso implica múltiples formularios físicos, evaluaciones manuales y tiempos prolongados de análisis, lo que genera demoras en la aprobación de créditos, mayor carga operativa y una limitada trazabilidad de la información. Además, se necesita integrar herramientas tecnológicas como scoring crediticio, monitoreo de transacciones y conexión con el sistema CORE bancario, garantizando seguridad, confidencialidad y cumplimiento normativo. |
| **Objetivo Principal** | Desarrollar e implementar una plataforma virtual que digitalice y optimice el proceso crediticio para Pyme y Banca Empresa del BDP S.A.M., permitiendo una gestión más ágil, segura y eficiente, integrada al sistema CORE del banco y alineada a las tendencias tecnológicas actuales. |


### 1.2 Matriz de Stakeholders

| **Rol** | **Nombre/Cargo** | **Nivel de Influencia** | **Expectativa Principal** |
|--------|----------------|------------------------|---------------------------|
| Cliente / Patrocinador | Alta Gerencia del BDP S.A.M. | Alto | Que el proyecto se implemente en el plazo establecido, dentro del presupuesto y que mejore radicalmente la eficiencia del proceso crediticio. |
| Usuario Final | Analistas de crédito y Funcionarios | Medio | Contar con una plataforma fácil de usar que agilice la evaluación, reduzca la carga operativa manual y evite el uso de hojas de cálculo externas. |
| Equipo Técnico | Miguel Angel Chura Condori (Gestor de Pilas) <br> Norma Mendoza Layme (Dev) <br> Nicole Abigail Arratia Chipana (Dev) <br> Roger Huarachi Rojas (Dev) <br> Kevin Jhonatan Rocha (Dev) <br> Beymar Castillo Cordova (Dev) | Alto | Contar con requerimientos claros, acceso a los ambientes de prueba a tiempo, y entregar un software de alta calidad que cumpla con el cronograma. |


## 2. Antecedentes y Problema (El "Por qué")

**Contexto:** El BDP S.A.M. es una sociedad de economía mixta que funciona como un banco de primer y segundo piso. El proyecto está enfocado en el área crediticia productiva.  

**Problema actual:** El proceso crediticio requiere mayor agilidad para evitar cuellos de botella operativos en las agencias.

### 2.1 La Complejidad del Sector Productivo

- **El Ciclo de Vida (Pecuario):** El software debe proyectar el desarrollo del hato ganadero (nacimientos, recría, engorde, venta) para automatizar el cálculo de ingresos.  
- **La Estacionalidad (Agrícola):** El sistema debe permitir simulación mediante supuestos (precio de soya, rendimiento por hectárea).  
- **Gestión de Garantías:** Conexión dinámica entre valor de garantías y capacidad de pago.

### 2.2 Riesgos de un Software Genérico

- Riesgos de crédito  
- Cuellos de botella operativos  

**Triple Impacto:**
- El productor recibe el crédito a tiempo  
- El banco asegura su cartera  
- El país produce más alimentos  


## 3. Alcance del Proyecto (El "Qué")

**Funcionalidades principales:**

- Registro inicial único de datos  
- Checklists inteligentes  
- Calculadoras automatizadas  
- Generación de reportes ejecutivos  
- Selector dinámico de perfil  

**Restricción de Alcance:**  
No se desarrollará aplicación móvil nativa independiente.

## 4. Requerimientos Funcionales y Técnicos

### 4.1 Requerimientos Funcionales

| **ID** | **Descripción** | **HU** | **Prioridad** |
|------|-------------|------|------------|
| RF-01 | Control de acceso y roles con JWT — bloqueo tras 3 intentos fallidos | HU-01 | Must |
| RF-02 | Auditoría WORM con encadenamiento SHA-256 — registros inalterables | HU-02 | Must |
| RF-03 | Aprobación o rechazo de solicitudes en comité con resolución formal | HU-03 | Must |
| RF-04 | Carga y almacenamiento de documentos digitales (PDF, JPG, PNG) | HU-04 | Must |
| RF-05 | Checklist inteligente de validación documental por tipo de crédito | HU-05 | Must |
| RF-06 | Gestión de garantías asociadas a cada solicitud de crédito | HU-12 | Must |
| RF-07 | Proyección ganadera: nacimientos, mortalidad, recría y engorde | HU-06 | Must |
| RF-08 | Simulación de escenarios agrícolas con motor de reglas parametrizable | HU-07 | Should |
| RF-09 | Scoring crediticio desde API Fintech con clasificación de riesgo A/B/C/D | HU-08 | Must |
| RF-10 | Sincronización con CORE bancario vía API REST con reintentos automáticos | HU-09 | Must |
| RF-11 | Trabajo de campo sin conexión mediante PWA e IndexedDB | HU-10 | Must |
| RF-12 | Monitoreo de cartera activa y alertas de vencimiento via cron job | HU-11 | Must |


### 4.2 Requerimientos No Funcionales

| **ID** | **Categoría** | **Descripción** |
|------|-------------|-------------|
| RNF-01 | Offline-First | Funcionamiento sin internet |
| RNF-02 | Escalabilidad | Soporte 500 usuarios |
| RNF-03 | Parametrización | Motor de reglas dinámico |
| RNF-04 | Integración | API segura |
| RNF-05 | Seguridad | Cifrado + WORM |


## 5. Estrategia de Implementación

- Metodologías ágiles  
- Capacitación en Sandbox  
- Control de cambios por ambientes  


## 6. Propiedad y Confidencialidad

- Código fuente propiedad del BDP  
- Información confidencial  


## 7. Cronograma

**Total: 190 días hábiles · Inicio: 06/04/2026 · Cierre: 02/01/2027**

| Fase | Descripción | Días | Fecha Límite |
|------|-------------|------|-------------|
| Fase 1 | Plan de Dirección y Arquitectura Base | 30 días | 16/05/2026 |
| Fase 2 | Plataforma Alpha — Módulos Core | 80 días | 07/09/2026 |
| Fase 3 | Fase Beta — Riesgo, Seguridad y Validación | 50 días | 14/11/2026 |
| Fase 4 | Go-Live, Transferencia Tecnológica y Cierre | 30 días | 02/01/2027 |
| **TOTAL** | | **190 días hábiles** | |


## 8. Presupuesto

| **Hito** | **Monto (Bs.)** | **%** |
|--------|---------------|------|
| H-1 — Plan de Dirección y Arquitectura | 90,000 | 20% |
| H-2 — Plataforma Alpha (Módulos Core) | 157,500 | 35% |
| H-3 — Fase Beta (Integración y Seguridad) | 112,500 | 25% |
| H-4 — Go-Live y Cierre | 90,000 | 20% |
| **TOTAL** | **450,000** | **100%** |
