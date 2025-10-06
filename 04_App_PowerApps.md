# 🖥️ Aplicación Power Apps

## Estructura de la app
- **Pantalla principal:** Dashboard de tickets por estado.
- **Pantalla detalle:** Información del ticket seleccionado.
- **Pantalla de comentarios:** Seguimiento del caso.
- **Pantalla de administración:** Gestión de responsables y roles.

## Componentes clave
- **Galerías:** Visualización dinámica de tickets.
- **Containers:** Agrupan secciones de detalle y formularios.
- **Formularios:** Registro y edición de tickets.
- **Variables globales:** 
  - `varRegistroSeleccionado`
  - `varRolComparacion`
  - `varctMostrarLoading`

## Ejemplo de fórmula de color por estado
```powerapps
Switch(
    ThisItem.Estado.Value,
    "Sin asignar", ColorValue("#9E9E9E"),
    "Nuevo", ColorValue("#2962FF"),
    "En Progreso", ColorValue("#FF6D00"),
    "Pausado", ColorValue("#D50000"),
    "Resuelto", ColorValue("#00C853"),
    "Cerrado", ColorValue("#212121")
)
```
