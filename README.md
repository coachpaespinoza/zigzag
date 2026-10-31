# ZIGZAG — versión funcional multiplataforma v0.2

Aplicación React + TypeScript + Capacitor preparada para web, Android e iOS. Es una **versión inicial para pruebas**, no un producto listo para las tiendas.

## Ejecutar

Instalar Node.js 20 o superior y ejecutar:

```bash
npm install
npm run dev
```

Abrir la dirección que muestra Vite.

## Compilar web

```bash
npm run build
```

Los archivos web quedan en `dist/`.

## Android

Instalar Android Studio, Android SDK y Java compatibles con Capacitor 7. Luego:

```bash
npm run build
npx cap add android
npx cap sync android
npx cap open android
```

Desde Android Studio se genera el APK de pruebas o AAB firmado para Play Console. **El AAB no está incluido** y necesita firma y revisión de requisitos vigentes de Google Play.

## iOS

En un Mac con Xcode:

```bash
npm run build
npx cap add ios
npx cap sync ios
npx cap open ios
```

La distribución iOS requiere firma, Apple Developer y el proceso de App Store Connect. **No hay IPA firmada incluida**.

## Qué incluye

- Navegación Inicio, Mi día, Mi Manual y Mi espacio.
- Arranque, Mi Foco, Mi Mapa, Reset, Vuelve y Chispas.
- Mi día: tarjetas y línea de tiempo con escala proporcional.
- RADAR: detección básica de cruces de horario.
- Plan B: traslado de tareas flexibles con opción de deshacer.
- Tiempo Realista: estimaciones voluntarias.
- Preferencias de Mi Manual y superrecursos.
- Datos guardados en localStorage del dispositivo.

## Limitaciones importantes

- No incluye cuentas, sincronización, backend, cifrado, notificaciones push ni Ziggy con IA generativa.
- La detección de conflictos y la línea de tiempo son iniciales: falta mejorar eventos nocturnos, recurrencia, zonas horarias y disposición compleja de solapamientos.
- El almacenamiento local puede perderse si se borran datos de la aplicación.
- No debe distribuirse a menores ni utilizarse para datos sensibles sin revisión de privacidad, seguridad y cumplimiento legal.
- Antes de publicar, reemplazar el ID de paquete `cl.zigzag.app` por uno definitivo que controles, añadir iconos, splash, políticas, pruebas y firma.

## Novedades v0.2

Incluye PWA básica instalable con caché offline después de una primera carga conectada. Para producción, probar el comportamiento del service worker y sustituir el icono provisional por recursos Android/iOS adecuados. Ver `CHANGELOG.md`.
