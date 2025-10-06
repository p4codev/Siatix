# 📘 Siatix – Ticketera Organizacional de Clientes

> **Documentación oficial del sistema de ticketera digital desarrollado por Alexander Coral para Siatigroup.**

---

## 🌐 Sitio web de la documentación

🔗 **Accede a la documentación completa en línea:**
👉 [https://p4codev.github.io/Siatix/](https://p4codev.github.io/Siatix/)

---

## 🧩 Descripción general

**Siatix** es una plataforma desarrollada sobre **Microsoft Power Platform** (Power Apps + Power Automate + SharePoint + Power BI) que centraliza la gestión de requerimientos, incidencias y solicitudes de clientes de **Siatigroup**, empresa especializada en soluciones integrales de **importación y exportación**.

La ticketera permite registrar, asignar, monitorear y resolver casos de atención mediante flujos automatizados, con notificaciones y métricas de seguimiento.

---

## 🎯 Objetivos principales

- Centralizar la gestión de requerimientos de clientes.  
- Mejorar la trazabilidad y comunicación entre áreas.  
- Reducir los tiempos de respuesta mediante automatización.  
- Generar reportes de SLA y productividad en Power BI.  
- Estandarizar la atención de postventa dentro de Siatigroup.

---

## ⚙️ Tecnologías utilizadas

| Herramienta | Uso principal |
|--------------|---------------|
| **Power Apps** | Interfaz del sistema (registro y consulta de tickets) |
| **Power Automate** | Flujos automáticos de correo y Teams |
| **SharePoint Online** | Base de datos y control de permisos |
| **Power BI** | Dashboards de indicadores y métricas |
| **Teams / Outlook** | Canales de notificación y comunicación |
| **Docsify + GitHub Pages** | Portal web de documentación |

---

## 🧱 Arquitectura general

```mermaid
graph TD
A[Cliente / Colaborador] -->|Crea Ticket| B[Power Apps]
B --> C[SharePoint - Tickets]
C --> D[Power Automate - Flujos]
D --> E[Outlook / Teams - Notificaciones]
C --> F[Power BI - Reportes SLA]
