# 1. Resumen Ejecutivo

## 1.1. Ficha del Proyecto

| Concepto | Descripción |
|----------|-------------|
| **Nombre del Proyecto** | Sistema de Gestión Crediticia Agropecuaria — BDP Crédito |
| **Cliente** | Banco de Desarrollo Productivo (BDP S.A.M.) |
| **Área** | Unidad PyME y Banca Empresa |
| **Objetivo Principal** | Digitalizar y optimizar el proceso crediticio agropecuario mediante una plataforma web que integre evaluación técnica, scoring crediticio, auditoría WORM y conexión con el CORE bancario |
| **Metodología** | Scrum + MoSCoW |
| **Total de HUs** | 12 Historias de Usuario (HU-01 a HU-12) |
| **Arquitectura** | Monolítica Modular |
| **Año** | 2026 |


## 1.2. Equipo de Desarrollo

| Integrante | Rol | Pareja | HUs Asignadas |
|-----------|-----|--------|---------------|
| Roger Huarachi Rojas | Dev | P1 | HU-01, HU-04, HU-07, HU-10 |
| Kevin Jhonatan Rocha | Dev | P1 | HU-01, HU-04, HU-07, HU-10 |
| Beymar Castillo Cordova | Dev | P2 | HU-02, HU-05, HU-08, HU-11 |
| Nicole Abigail Arratia Chipana | Dev | P2 | HU-02, HU-05, HU-08, HU-11 |
| Norma Mendoza Layme (Alcozer) | Dev | P3 | HU-03, HU-06, HU-09, HU-12 |
| Miguel Angel Chura Condori | Dev | P3 | HU-03, HU-06, HU-09, HU-12 |


## 1.3. Stack Tecnológico

| Capa | Tecnología | Librerías Clave |
|------|-----------|-----------------|
| Frontend | React 18 + Vite | axios, recharts, jsPDF, jspdf-autotable |
| Backend | Node.js + Express | jsonwebtoken, bcrypt, pg, node-cron, ExcelJS |
| Base de Datos | PostgreSQL | — |
| Seguridad | JWT + bcrypt + SHA-256 WORM | — |
| Offline | PWA + IndexedDB | — |


## 1.4. Épicas del Sistema

| Épica | Nombre | HUs |
|-------|--------|-----|
| EP01 | Seguridad y Acceso | HU-01, HU-02 |
| EP02 | Gestión de Solicitudes | HU-03, HU-04, HU-05, HU-12 |
| EP03 | Evaluación Técnica | HU-06, HU-07 |
| EP04 | Integraciones Inteligentes | HU-08, HU-09 |
| EP05 | Movilidad y Trabajo de Campo | HU-10 |
| EP06 | Salidas, Reportes y Monitoreo | HU-11 |


## 1.5. Objetivo del Sistema

Desarrollar una plataforma web que permita al BDP S.A.M. gestionar de forma digital, segura y eficiente el proceso crediticio agropecuario, cubriendo desde el registro inicial del cliente hasta la aprobación en comité, el desembolso y el monitoreo de cartera activa.
