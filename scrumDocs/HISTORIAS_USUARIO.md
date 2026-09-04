# Historias de Usuario -- simulador quimico

_Generado automaticamente el 2026-09-04T13:59:48.821Z -- no editar a mano, se sobreescribe en cada publicacion._

## HU-01: Simulación de Disoluciones (C1*V1 = C2*V2)

Como usuario, quiero acceder a una opción de disoluciones que me muestre un recipiente (ej. vaso de precipitados), donde pueda ingresar tres de las cuatro variables (Concentración 1, Volumen 1, Concentración 2, Volumen 2) y el sistema calcule la restante usando la fórmula C1*V1=C2*V2, para así también poder visualizar gráficamente la reacción (agregación o evaporación de agua) en tiempo real en el recipiente.

### Criterios de Aceptacion

- La interfaz debe presentar una opción o menú exclusivo para "Disoluciones".
- Debe existir una representación visual de un recipiente (como un vaso de precipitados).
- Se deben proveer campos de entrada para Concentración inicial (C1), Volumen inicial (V1), Concentración final (C2) y Volumen final (V2).
- El sistema debe calcular automáticamente la variable faltante si se completan las otras tres.
- La representación visual del recipiente debe actualizarse reflejando la acción que está ocurriendo (animación de agregación de agua si el volumen aumenta, o evaporación si el volumen disminuye).
