# 🔄 Flujos de Power Automate

## Flujo: Creación de ticket
- **Disparador:** Al crear un nuevo elemento en "Tickets".
- **Acciones:**
  - Enviar correo de confirmación al cliente.
  - Notificar al responsable del departamento.
  - Crear registro de seguimiento.

## Flujo: SLA Recordatorio
- **Disparador:** Programado cada 24h.
- **Condición:** Ticket en estado “Nuevo” por más de 24 horas.
- **Acción:** Enviar recordatorio automático al responsable y gerente.

## Flujo: Cierre automático
- **Disparador:** Cuando un ticket está “Resuelto” durante más de 48h.
- **Acción:** Cambiar estado a “Cerrado” automáticamente y enviar notificación.

## Flujo: Eliminación responsable
- **Disparador:** Al eliminar un registro en “ResponsableTickets”.
- **Acción:** Enviar correo de aviso → eliminar del sistema → registrar en lista de auditoría.
