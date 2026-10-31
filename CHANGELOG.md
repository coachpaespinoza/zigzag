## 0.3.9 — Ziggy paso a paso
- Guías para Empezar, Foco, Reset y Volver, con una indicación a la vez.
- Escucha del paso actual en modo Audio; mantiene selección de voz es-CL si está disponible.
- Navegación libre, sin temporizadores, con opción de salir.
- Notas opcionales guardadas localmente en zigzag-guide-notes.

## 0.3.8 — Audio por fragmentos

- Toca un párrafo, título o instrucción para seleccionarlo y escucharlo individualmente.
- Control de velocidad: lenta, normal y rápida.
- Se mantiene el modo escrito y la lectura de pantalla completa.
- Prioridad a voces es-CL si el dispositivo las tiene.
- La lectura es opcional, local y no requiere subir texto a un servidor propio.

## 0.3.7 — Lectura escrita o en audio
- Selector persistente Escrito / Audio visible en bienvenida y aplicación.
- Lectura en voz alta del contenido principal de la pantalla, con control para detener.
- Preferencia por voces del dispositivo es-CL (Chile); aviso claro cuando solo hay otra voz en español o voz predeterminada.
- Audio opcional, sin subir textos a un servidor de ZIGZAG. La disponibilidad y el procesamiento de voz dependen del sistema del dispositivo.

# ZIGZAG — cambios v0.2

- Manifiesto PWA, icono inicial y service worker para uso sin conexión tras la primera carga.
- Se conserva la vista Tarjetas / Línea de tiempo elegida entre sesiones.
- Fecha local corregida para evitar desfases por zona horaria.
- Validación estricta de duración entre 5 y 480 minutos.
- La edición de tareas conserva estado y recordatorio existentes.
- Se elimina un bloque duplicado de superrecursos.
- Mejora de foco visible, objetivos táctiles y metadatos móviles.

**Pendiente:** pruebas en dispositivo, íconos rasterizados específicos de tiendas, cuentas, sincronización, notificaciones reales, seguridad y cumplimiento de requisitos de publicación. El icono es provisional.

## 0.3.3 — Vuelve y Ziggy contextual
- Vuelve muestra todas las actividades pendientes con puntos de regreso, no solo la primera.
- Retomar, editar el punto o dejar para después sin borrar información.
- Ziggy respeta las preferencias de inicio, energía, temporizador y nivel de presencia.
- La preferencia de Ziggy mínimo evita mostrar el saludo automático.
- Pendiente: validar npm run build y pruebas en dispositivo antes de GitHub.

## 0.3.4 — Mi día
- Navegación entre días con flechas y regreso a Hoy.
- Resumen de actividades pendientes y completadas.
- Marcar actividades como realizadas desde tarjetas sin abrir edición.
- Sección de actividades completadas con opción Reabrir.
- Estados vacíos amables para agenda y actividades flexibles.


## 0.3.5 — Inicio y sistema visual
- Inicio con resumen real de actividades de hoy y barra de progreso accesible.
- Nueva cabecera, portada editorial, tarjetas diferenciadas y navegación móvil.
- Mejora de estados de foco, contraste y presentación en pantallas pequeñas.
- Conserva datos existentes en almacenamiento local y módulos 0.3.4.

## 0.3.6
- Bienvenida de cinco pasos opcionales, sin registro ni diagnóstico.
- Preferencias de inicio, concentración, presencia de Ziggy y baja estimulación.
- Persistencia local y acceso posterior a la aplicación.

## 0.4.0 — Camino conectado
- Recorrido de una actividad: Arranque → Mi Foco → Vuelve.
- Punto de regreso compartido entre herramientas y guardado localmente.
- Acceso al recorrido desde Inicio, Mi Mapa y Mi Foco.
- Acciones para guardar, enfocar, pausar, completar y cambiar de actividad.

## 0.4.1 — Respaldo y estabilidad
- Exportar e importar datos locales con validación básica y confirmación antes de reemplazar.
- Proteger lectura de notas guardadas frente a JSON malformado.
- Corregir GitHub Actions: evitar caché npm sin lockfile y actualizar setup-android a v4.
- Pendiente: compilación e instalación real en Android.
