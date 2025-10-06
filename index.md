---
title: Siatix - Ticketera Organizacional de Clientes
description: Documentación oficial del sistema de ticketera digital de Siatigroup, desarrollada por Alexander Coral.
---

# 💼 Siatix – Ticketera Organizacional de Clientes

> **Versión:** 1.0  
> **Autor:** Alexander Coral  
> **Empresa:** [Siatigroup](https://siatigroup.com)  
> **Repositorio:** [p4codev/Siatix](https://github.com/p4codev/Siatix)  
> **Sitio Web:** [https://p4codev.github.io/Siatix/](https://p4codev.github.io/Siatix/)

---

## 🧩 Descripción general

**Siatix** es una solución empresarial desarrollada con **Microsoft Power Platform** para la gestión de requerimientos y atención al cliente dentro de **Siatigroup**, empresa líder en soluciones integrales de **comercio exterior, importaciones y exportaciones**.

La plataforma centraliza el ciclo de vida de los tickets desde su creación hasta su resolución, automatizando las notificaciones, aprobaciones y reportes mediante **Power Apps**, **Power Automate**, **SharePoint** y **Power BI**.

---

## 🚀 Objetivos del sistema

- Centralizar la gestión de requerimientos de clientes.  
- Reducir los tiempos de respuesta.  
- Mejorar la trazabilidad de casos entre departamentos.  
- Estandarizar la atención al cliente.  
- Generar métricas automáticas de desempeño (SLA).  
- Integrarse de forma nativa con Teams y Outlook.  

---

## ⚙️ Arquitectura general

```mermaid
graph TD
A[Usuario Cliente] -->|Formulario Power Apps| B[SharePoint - Tickets]
B --> C[Power Automate - Flujos]
C --> D[Outlook / Teams - Notificaciones]
B --> E[Power BI - Reportes]
C --> F[SharePoint - SolicitudEstados]
C --> G[SharePoint - ComentarioUsuario]
