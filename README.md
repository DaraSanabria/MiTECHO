# Mockup — Comunicaciones TECHO

Prototipo navegable del módulo de **Comunicaciones** de la plataforma de TECHO, para revisión y feedback de los países.

> ⚠️ Es un **mockup con datos de ejemplo**. No envía correos, no cobra pagos y no está conectado a la base real. Sirve para validar la experiencia y los flujos antes de desarrollar.

## Pantallas

| Archivo | Pantalla | Qué muestra |
|---|---|---|
| `index.html` | **Nueva comunicación** | Segmentador de audiencia con alcance en vivo, envío gradual y (en WhatsApp) calculadora de costo + pago con Stripe. |
| `comunicaciones-enviadas.html` | **Comunicaciones enviadas** | Historial con estado de envío (en proceso, detenido, culminado, en cola, falló), métricas de apertura/clic y panel de detalle por comunicación. |

Se navega entre ambas desde el menú lateral (Comunicaciones → Nueva comunicación / Comunicaciones enviadas).

## Cómo verlo

- **En vivo (recomendado):** abrir la URL de GitHub Pages (ver más abajo).
- **Local:** descargar la carpeta y abrir `index.html` en el navegador. Funciona sin servidor.

## Qué queremos que revisen los países

1. ¿Los **filtros de segmentación** cubren cómo piensan sus bases (voluntariado, socios, base histórica, alumni, equipos)?
2. ¿El flujo de **costo + pago de WhatsApp** tiene sentido para su operación?
3. ¿Los **estados de envío** y las **métricas** (aperturas, clics, conversión, rebotes) son las que necesitan ver?
4. ¿Falta algún dato en el **registro de segmentación** o en el **dashboard de resultados**?

Feedback: [completar con canal — mail / issue de GitHub / formulario].

## Notas técnicas (para el equipo de desarrollo)

- Envío real previsto sobre **Amazon SES** (ya en uso), con métricas vía *Configuration Sets* (open/click/bounce).
- WhatsApp: costo por conversación de marketing de Meta, cobrado con **Stripe (cuenta central)**.
- Tarifas y series de datos son de ejemplo; reemplazar por valores reales.

---
Hecho para TECHO · *Mucho más que un techo.*
