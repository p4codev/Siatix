# 📋 Estructura de Listas SharePoint

## Lista: Tickets
| Campo | Tipo | Descripción |
|-------|------|-------------|
| ID_Ticket | Número | Identificador único |
| Departamento | Elección | Tráfico, Ventas, Marketing, etc. |
| ÁreaServicio | Elección | Subáreas según el departamento |
| TipoRequerimiento | Elección | Consulta, Reclamo, Solicitud |
| NombreCliente | Texto | Nombre del cliente |
| CorreoCliente | Correo | Dirección de contacto |
| RUCCliente | Texto | Identificación fiscal |
| Asunto | Texto | Breve título del ticket |
| Descripción | Texto multilínea | Detalle del requerimiento |
| Prioridad | Elección | Sin prioridad, Baja, Media, Alta, Crítica |
| Estado | Elección | Sin asignar, Nuevo, En progreso, Pausado, Resuelto, Cerrado |
| FechaCreación | Fecha | Creación automática |
| ResponsableArea | Usuario | Usuario asignado al ticket |

## Lista: ComentarioUsuario
| Campo | Tipo | Descripción |
|-------|------|-------------|
| ID_Ticket | Número | Ticket relacionado |
| comentarioAsignacion | Texto | Comentario del usuario |
| usuarioSeguimiento | Usuario | Autor del comentario |
| fechaSeguimiento | Fecha | Fecha y hora del comentario |

## Lista: SolicitudEstados
| Campo | Tipo | Descripción |
|-------|------|-------------|
| Título | Texto | ID del ticket asociado |
| solicitudEstado | Elección | Estado solicitado |
| solicitudComentario | Texto | Motivo del cambio |
| solicitudFecha | Fecha | Fecha de la solicitud |
