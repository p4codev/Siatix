# ⚙️ Arquitectura Técnica

## Diagrama general
El sistema sigue una arquitectura modular basada en servicios de Microsoft 365:

```
Usuario → Power Apps → SharePoint (Tickets, Comentarios, Asignaciones)
             ↓
        Power Automate → Outlook / Teams / Power BI
```

## Componentes principales
- **Front-end:** Power Apps Canvas App.
- **Back-end:** Listas de SharePoint (modelo relacional).
- **Automatización:** Flujos de Power Automate.
- **Reportes:** Dashboard Power BI conectado a SharePoint.
- **Notificaciones:** Envíos automáticos a Outlook y Teams.

## Entorno y licencias
- Entorno: Producción (Siatigroup)
- Licencias requeridas:
  - Microsoft 365 E3 o superior.
  - Power Automate Premium (para conexiones externas opcionales).

## Seguridad y control de acceso
- Autenticación por Azure AD.
- Roles definidos en SharePoint y Power Apps.
- Permisos de lectura/escritura según grupo de usuario.
