# Instalar ZIGZAG en Android (APK de pruebas)

Este ZIP contiene el código, NO el APK ya compilado. El APK se puede generar en GitHub Actions.

1. Crea una cuenta gratuita en https://github.com si no tienes una.
2. Crea un repositorio nuevo llamado `zigzag-android` (preferentemente **privado**).
3. Sube **el contenido de la carpeta `zigzag-app`**, incluyendo la carpeta oculta `.github`, a la raíz del repositorio. Si GitHub no permite cargar carpetas vacías, no importa.
4. Abre la pestaña **Actions**. Si GitHub solicita habilitar workflows, habilítalos.
5. Selecciona **Generar APK ZIGZAG** y pulsa **Run workflow**.
6. Cuando el proceso termine con éxito, abre su ejecución y descarga el artefacto **ZIGZAG-Android-APK-pruebas**. Dentro estará `app-debug.apk`.
7. Copia ese APK a tu teléfono Android, ábrelo y acepta instalarlo desde esa fuente cuando Android lo solicite.

**Importante:** este es un APK DEBUG solo para pruebas personales, NO sirve para publicar en Google Play. Para Play Console se necesitará un AAB firmado con clave de publicación y pruebas de cumplimiento.

No se ha ejecutado ni validado la compilación en este entorno porque no hay Android SDK y el acceso al registro de npm no funcionó. Si el workflow falla, copia el error para corregirlo. La disponibilidad gratuita de GitHub Actions depende de los límites de tu cuenta.
